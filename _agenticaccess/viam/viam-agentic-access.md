---
acting_count: 189
action_class_counts:
  acting: 189
api_specs:
- filename: viam-fleet-management-api-openapi.yml
  format: yaml
  label: Viam Fleet Management API
  slug: viam-fleet-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-fleet-management-api-openapi.yml
- filename: viam-machine-management-api-openapi.yml
  format: yaml
  label: Viam Machine Management API
  slug: viam-machine-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-machine-management-api-openapi.yml
- filename: viam-data-client-api-openapi.yml
  format: yaml
  label: Viam Data Client API
  slug: viam-data-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-data-client-api-openapi.yml
- filename: viam-data-sync-api-openapi.yml
  format: yaml
  label: Viam Data Sync API
  slug: viam-data-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-data-sync-api-openapi.yml
- filename: viam-ml-training-api-openapi.yml
  format: yaml
  label: Viam ML Training API
  slug: viam-ml-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-ml-training-api-openapi.yml
- filename: viam-ml-inference-api-openapi.yml
  format: yaml
  label: Viam ML Inference API
  slug: viam-ml-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-ml-inference-api-openapi.yml
- filename: viam-billing-api-openapi.yml
  format: yaml
  label: Viam Billing API
  slug: viam-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-billing-api-openapi.yml
- filename: viam-motion-service-api-openapi.yml
  format: yaml
  label: Viam Motion Service API
  slug: viam-motion-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-motion-service-api-openapi.yml
- filename: viam-vision-service-api-openapi.yml
  format: yaml
  label: Viam Vision Service API
  slug: viam-vision-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-vision-service-api-openapi.yml
- filename: viam-slam-service-api-openapi.yml
  format: yaml
  label: Viam SLAM Service API
  slug: viam-slam-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-slam-service-api-openapi.yml
- filename: viam-ml-model-service-api-openapi.yml
  format: yaml
  label: Viam ML Model Service API
  slug: viam-ml-model-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-ml-model-service-api-openapi.yml
- filename: viam-component-apis-openapi.yml
  format: yaml
  label: Viam Component APIs
  slug: viam-component-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-component-apis-openapi.yml
- filename: viam-data-pipelines-api-openapi.yml
  format: yaml
  label: Viam Data Pipelines API
  slug: viam-data-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-data-pipelines-api-openapi.yml
- filename: viam-provisioning-api-openapi.yml
  format: yaml
  label: Viam Provisioning API
  slug: viam-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/openapi/viam-provisioning-api-openapi.yml
consequence_counts:
  physical: 11
  safety-critical: 8
  write: 170
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Viam Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /viam.app.datapipelines.v1.DataPipelinesService/DisableDataPipeline
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /viam.component.arm.v1.ArmService/Stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /viam.component.base.v1.BaseService/Stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /viam.component.encoder.v1.EncoderService/ResetPosition
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /viam.component.motor.v1.MotorService/Stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /viam.robot.v1.RobotService/Shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /viam.robot.v1.RobotService/StopAll
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /viam.service.motion.v1.MotionService/StopPlan
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.app.v1.BillingService/ChargeOrganization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.app.v1.BillingService/CreateInvoiceAndChargeImmediately
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.app.v1.BillingService/GetInvoicePdf
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.app.v1.BillingService/GetInvoicesSummary
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.app.v1.BillingService/SendPaymentRequiredEmail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.provisioning.v1.ProvisioningService/ExitProvisioning
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.provisioning.v1.ProvisioningService/GetNetworkList
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.provisioning.v1.ProvisioningService/GetSmartMachineStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.provisioning.v1.ProvisioningService/SetNetworkCredentials
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.provisioning.v1.ProvisioningService/SetSmartMachineCredentials
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /viam.robot.v1.RobotService/SendSessionHeartbeat
operation_count: 189
overview: 'Viam exposes 189 API operations that an AI agent could call, of which 189 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 170 write, 11 physical, and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Viam
provider_slug: viam
slug: viam-agentic-access
source_filename: viam-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/viam-billing-api-openapi.yml, openapi/viam-component-apis-openapi.yml, openapi/viam-data-client-api-openapi.yml,\n  openapi/viam-data-pipelines-api-openapi.yml, openapi/viam-data-sync-api-openapi.yml, openapi/viam-fleet-management-api-openapi.yml,\n  openapi/viam-machine-management-api-openapi.yml, openapi/viam-ml-inference-api-openapi.yml,\n  openapi/viam-ml-model-service-api-openapi.yml, openapi/viam-ml-training-api-openapi.yml, openapi/viam-motion-service-api-openapi.yml,\n  openapi/viam-provisioning-api-openapi.yml, openapi/viam-slam-service-api-openapi.yml, openapi/viam-vision-service-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 189\n  by_action_class:\n    acting:\
  \ 189\n  by_consequence:\n    write: 170\n    physical: 11\n    safety-critical: 8\n  human_in_the_loop_required: 8\noperations:\n- path: /viam.app.v1.BillingService/GetCurrentMonthUsage\n  method: post\n  operationId: getCurrentMonthUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/GetOrgBillingInformation\n  method: post\n  operationId: getOrgBillingInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/GetInvoicesSummary\n  method: post\n  operationId:\
  \ getInvoicesSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/GetInvoicePdf\n  method: post\n  operationId: getInvoicePdf\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/SendPaymentRequiredEmail\n  method: post\n  operationId: sendPaymentRequiredEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/GetAvailableBillingTiers\n  method: post\n  operationId: getAvailableBillingTiers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/UpdateOrganizationBillingTier\n  method: post\n  operationId: updateOrganizationBillingTier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/GetLocationBillingOrganization\n  method: post\n  operationId: getLocationBillingOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/UpdateLocationBillingOrganization\n  method: post\n  operationId: updateLocationBillingOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/ChargeOrganization\n  method: post\n  operationId: chargeOrganization\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.v1.BillingService/CreateInvoiceAndChargeImmediately\n  method: post\n  operationId: createInvoiceAndChargeImmediately\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.arm.v1.ArmService/GetEndPosition\n  method: post\n  operationId: armGetEndPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.arm.v1.ArmService/MoveToPosition\n  method: post\n  operationId: armMoveToPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.arm.v1.ArmService/GetJointPositions\n  method: post\n  operationId: armGetJointPositions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.arm.v1.ArmService/MoveToJointPositions\n  method:\
  \ post\n  operationId: armMoveToJointPositions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.arm.v1.ArmService/Stop\n  method: post\n  operationId: armStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /viam.component.base.v1.BaseService/MoveStraight\n  method: post\n  operationId: baseMoveStraight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.base.v1.BaseService/Spin\n  method: post\n  operationId: baseSpin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.base.v1.BaseService/SetPower\n  method: post\n  operationId: baseSetPower\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.base.v1.BaseService/SetVelocity\n  method: post\n  operationId: baseSetVelocity\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.base.v1.BaseService/Stop\n  method: post\n  operationId: baseStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /viam.component.board.v1.BoardService/SetGPIO\n  method: post\n  operationId: boardSetGPIO\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /viam.component.board.v1.BoardService/GetGPIO\n  method: post\n  operationId: boardGetGPIO\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.board.v1.BoardService/SetPWM\n  method: post\n  operationId: boardSetPWM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.board.v1.BoardService/ReadAnalogReader\n  method: post\n  operationId: boardReadAnalogReader\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.board.v1.BoardService/StreamTicks\n  method: post\n  operationId: boardStreamTicks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.button.v1.ButtonService/Push\n  method: post\n  operationId: buttonPush\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.camera.v1.CameraService/GetImages\n  method: post\n\
  \  operationId: cameraGetImages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.camera.v1.CameraService/GetPointCloud\n  method: post\n  operationId: cameraGetPointCloud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.camera.v1.CameraService/GetProperties\n  method: post\n  operationId: cameraGetProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.encoder.v1.EncoderService/GetPosition\n  method: post\n  operationId: encoderGetPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.encoder.v1.EncoderService/ResetPosition\n  method: post\n  operationId: encoderResetPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /viam.component.gantry.v1.GantryService/MoveToPosition\n  method: post\n  operationId:\
  \ gantryMoveToPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.gantry.v1.GantryService/Home\n  method: post\n  operationId: gantryHome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.gripper.v1.GripperService/Open\n  method: post\n  operationId: gripperOpen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /viam.component.gripper.v1.GripperService/Grab\n  method: post\n  operationId: gripperGrab\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.gripper.v1.GripperService/IsHoldingSomething\n  method: post\n  operationId: gripperIsHoldingSomething\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.motor.v1.MotorService/SetPower\n  method: post\n  operationId: motorSetPower\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.motor.v1.MotorService/GoFor\n  method: post\n  operationId: motorGoFor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.motor.v1.MotorService/GoTo\n  method: post\n  operationId: motorGoTo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.motor.v1.MotorService/SetRPM\n\
  \  method: post\n  operationId: motorSetRPM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.motor.v1.MotorService/Stop\n  method: post\n  operationId: motorStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /viam.component.motor.v1.MotorService/IsPowered\n  method: post\n  operationId: motorIsPowered\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.movementsensor.v1.MovementSensorService/GetPosition\n  method: post\n  operationId: movementSensorGetPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.movementsensor.v1.MovementSensorService/GetLinearVelocity\n  method: post\n  operationId: movementSensorGetLinearVelocity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.movementsensor.v1.MovementSensorService/GetAngularVelocity\n\
  \  method: post\n  operationId: movementSensorGetAngularVelocity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.movementsensor.v1.MovementSensorService/GetCompassHeading\n  method: post\n  operationId: movementSensorGetCompassHeading\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.movementsensor.v1.MovementSensorService/GetOrientation\n  method: post\n  operationId: movementSensorGetOrientation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.powersensor.v1.PowerSensorService/GetVoltage\n  method: post\n  operationId: powerSensorGetVoltage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.powersensor.v1.PowerSensorService/GetCurrent\n  method: post\n  operationId: powerSensorGetCurrent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.powersensor.v1.PowerSensorService/GetPower\n\
  \  method: post\n  operationId: powerSensorGetPower\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.sensor.v1.SensorService/GetReadings\n  method: post\n  operationId: sensorGetReadings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.servo.v1.ServoService/Move\n  method: post\n  operationId: servoMove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.servo.v1.ServoService/GetPosition\n  method: post\n  operationId: servoGetPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.switch.v1.SwitchService/SetPosition\n  method: post\n  operationId: switchSetPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.switch.v1.SwitchService/GetPosition\n  method: post\n  operationId: switchGetPosition\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.audioin.v1.AudioInService/GetAudio\n  method: post\n  operationId: audioInGetAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.component.audioout.v1.AudioOutService/Play\n  method: post\n  operationId: audioOutPlay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /viam.component.generic.v1.GenericService/DoCommand\n  method: post\n  operationId: genericDoCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/TabularDataByFilter\n  method: post\n  operationId: tabularDataByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/TabularDataBySQL\n  method: post\n  operationId: tabularDataBySQL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/TabularDataByMQL\n  method: post\n  operationId: tabularDataByMQL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/ExportTabularData\n  method: post\n  operationId: exportTabularData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/GetLatestTabularData\n  method:\
  \ post\n  operationId: getLatestTabularData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/DeleteTabularData\n  method: post\n  operationId: deleteTabularData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/BinaryDataByFilter\n  method: post\n  operationId: binaryDataByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/BinaryDataByIDs\n  method: post\n  operationId: binaryDataByIDs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/DeleteBinaryDataByFilter\n  method: post\n  operationId: deleteBinaryDataByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/DeleteBinaryDataByIDs\n  method: post\n  operationId: deleteBinaryDataByIDs\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/CreateBinaryDataSignedURL\n  method: post\n  operationId: createBinaryDataSignedURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/AddTagsToBinaryDataByIDs\n  method: post\n  operationId: addTagsToBinaryDataByIDs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/RemoveTagsFromBinaryDataByIDs\n  method: post\n  operationId: removeTagsFromBinaryDataByIDs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/TagsByFilter\n  method: post\n  operationId: tagsByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/AddBoundingBoxToImageByID\n  method: post\n  operationId: addBoundingBoxToImageByID\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/RemoveBoundingBoxFromImageByID\n  method: post\n  operationId: removeBoundingBoxFromImageByID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/AddBinaryDataToDatasetByIDs\n  method: post\n  operationId: addBinaryDataToDatasetByIDs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/RemoveBinaryDataFromDatasetByIDs\n  method: post\n  operationId: removeBinaryDataFromDatasetByIDs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/CreateSavedQuery\n  method: post\n  operationId: createSavedQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/ListSavedQueries\n  method: post\n  operationId: listSavedQueries\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/GetSavedQuery\n  method: post\n  operationId: getSavedQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/UpdateSavedQuery\n  method: post\n  operationId: updateSavedQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/DeleteSavedQuery\n\
  \  method: post\n  operationId: deleteSavedQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/CreateSequence\n  method: post\n  operationId: createSequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viam.app.data.v1.DataService/ListSequences\n  method: post\n  operationId: listSequences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-lo\n\n# --- truncated\
  \ at 32 KB (70 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/agentic-access/viam-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viam/refs/heads/main/agentic-access/viam-agentic-access.yml
summary_line: 189 operations · 189 acting · 8 human-in-the-loop
tags:
- Robotics
- Edge AI
- Fleet Management
- Computer Vision
- Machine Learning
- IoT
- Embedded
- gRPC
---
