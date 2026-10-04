---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 22
api_specs:
- filename: amazon-iot-fleetwise-aws-iot-fleetwise-api-openapi.yml
  format: yaml
  label: Amazon IoT FleetWise AWS IoT FleetWise API
  slug: amazon-iot-fleetwise-aws-iot-fleetwise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/openapi/amazon-iot-fleetwise-aws-iot-fleetwise-api-openapi.yml
consequence_counts:
  read: 22
  safety-critical: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 28
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Iot Fleetwise Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.AssociateVehicleFleet
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.BatchCreateVehicle
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.BatchUpdateVehicle
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateCampaign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateDecoderManifest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateFleet
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateModelManifest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateSignalCatalog
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateVehicle
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteCampaign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteDecoderManifest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteFleet
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteModelManifest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteSignalCatalog
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteVehicle
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.DisassociateVehicleFleet
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.ImportDecoderManifest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.ImportSignalCatalog
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.PutLoggingOptions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.RegisterAccount
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.TagResource
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.UntagResource
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.UpdateCampaign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.UpdateDecoderManifest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=IoTAutobahnControlPlane.UpdateFleet
operation_count: 50
overview: 'Amazon IoT FleetWise exposes 50 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 28 safety-critical.


  28 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
slug: amazon-iot-fleetwise-agentic-access
source_filename: amazon-iot-fleetwise-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-associatevehiclefleet-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-batchcreatevehicle-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-batchupdatevehicle-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-createcampaign-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-createdecodermanifest-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-createfleet-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-createmodelmanifest-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-createsignalcatalog-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-createvehicle-api-openapi.yml,\n\
  \  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-deletecampaign-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-deletedecodermanifest-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-deletefleet-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-deletemodelmanifest-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-deletesignalcatalog-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-deletevehicle-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-disassociatevehiclefleet-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-getcampaign-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-getdecodermanifest-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-getfleet-api-openapi.yml,\n\
  \  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-getloggingoptions-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-getmodelmanifest-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-getregisteraccountstatus-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-getsignalcatalog-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-getvehicle-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-getvehiclestatus-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-importdecodermanifest-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-importsignalcatalog-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listcampaigns-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listdecodermanifestnetworkinterfaces-api-openapi.yml,\n\
  \  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listdecodermanifests-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listdecodermanifestsignals-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listfleets-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listfleetsforvehicle-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listmodelmanifestnodes-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listmodelmanifests-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listsignalcatalognodes-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listsignalcatalogs-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listtagsforresource-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listvehicles-api-openapi.yml,\n\
  \  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-listvehiclesinfleet-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-putloggingoptions-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-registeraccount-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-tagresource-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-untagresource-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-updatecampaign-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-updatedecodermanifest-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-updatefleet-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-updatemodelmanifest-api-openapi.yml,\n  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-updatesignalcatalog-api-openapi.yml,\n\
  \  openapi/amazon-iot-fleetwise-x-amz-target-iotautobahncontrolplane-updatevehicle-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    acting: 28\n    connected: 22\n  by_consequence:\n    safety-critical: 28\n    read: 22\n  human_in_the_loop_required: 28\noperations:\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.AssociateVehicleFleet\n  method: post\n  operationId: AssociateVehicleFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.BatchCreateVehicle\n\
  \  method: post\n  operationId: BatchCreateVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.BatchUpdateVehicle\n  method: post\n  operationId: BatchUpdateVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateCampaign\n  method: post\n  operationId: CreateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateDecoderManifest\n  method: post\n  operationId: CreateDecoderManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateFleet\n  method: post\n  operationId: CreateFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateModelManifest\n  method: post\n  operationId: CreateModelManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateSignalCatalog\n  method: post\n  operationId: CreateSignalCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.CreateVehicle\n\
  \  method: post\n  operationId: CreateVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteCampaign\n  method: post\n  operationId: DeleteCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteDecoderManifest\n  method: post\n  operationId: DeleteDecoderManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteFleet\n  method: post\n  operationId: DeleteFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteModelManifest\n  method: post\n  operationId: DeleteModelManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteSignalCatalog\n  method: post\n  operationId: DeleteSignalCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.DeleteVehicle\n  method: post\n  operationId: DeleteVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.DisassociateVehicleFleet\n\
  \  method: post\n  operationId: DisassociateVehicleFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.GetCampaign\n  method: post\n  operationId: GetCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.GetDecoderManifest\n  method: post\n  operationId: GetDecoderManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.GetFleet\n  method: post\n  operationId: GetFleet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.GetLoggingOptions\n  method: post\n  operationId: GetLoggingOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.GetModelManifest\n  method: post\n  operationId: GetModelManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.GetRegisterAccountStatus\n  method: post\n  operationId: GetRegisterAccountStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.GetSignalCatalog\n  method: post\n\
  \  operationId: GetSignalCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.GetVehicle\n  method: post\n  operationId: GetVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.GetVehicleStatus\n  method: post\n  operationId: GetVehicleStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ImportDecoderManifest\n  method: post\n  operationId: ImportDecoderManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ImportSignalCatalog\n  method: post\n  operationId: ImportSignalCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListCampaigns\n  method: post\n  operationId: ListCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListDecoderManifestNetworkInterfaces\n  method: post\n  operationId: ListDecoderManifestNetworkInterfaces\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListDecoderManifests\n  method: post\n  operationId: ListDecoderManifests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListDecoderManifestSignals\n  method: post\n  operationId: ListDecoderManifestSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListFleets\n  method: post\n  operationId: ListFleets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListFleetsForVehicle\n  method: post\n  operationId: ListFleetsForVehicle\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListModelManifestNodes\n  method: post\n  operationId: ListModelManifestNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListModelManifests\n  method: post\n  operationId: ListModelManifests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListSignalCatalogNodes\n  method: post\n  operationId: ListSignalCatalogNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListSignalCatalogs\n\
  \  method: post\n  operationId: ListSignalCatalogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListTagsForResource\n  method: post\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListVehicles\n  method: post\n  operationId: ListVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.ListVehiclesInFleet\n  method: post\n  operationId: ListVehiclesInFleet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.PutLoggingOptions\n\
  \  method: post\n  operationId: PutLoggingOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.RegisterAccount\n  method: post\n  operationId: RegisterAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.TagResource\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.UntagResource\n  method: post\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.UpdateCampaign\n  method: post\n  operationId: UpdateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.UpdateDecoderManifest\n  method: post\n  operationId: UpdateDecoderManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.UpdateFleet\n  method: post\n  operationId: UpdateFleet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.UpdateModelManifest\n  method: post\n  operationId:\
  \ UpdateModelManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.UpdateSignalCatalog\n  method: post\n  operationId: UpdateSignalCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=IoTAutobahnControlPlane.UpdateVehicle\n  method: post\n  operationId: UpdateVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/agentic-access/amazon-iot-fleetwise-agentic-access.yml
summary_line: 50 operations · 28 acting · 28 human-in-the-loop
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
---
