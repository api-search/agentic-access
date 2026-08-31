---
acting_count: 60
action_class_counts:
  acting: 60
  connected: 14
api_specs:
- filename: bell-canada-cancelserviceorder-api-openapi.yml
  format: yaml
  label: Bell Canada Cancel Service Order API
  slug: bell-canada-cancelserviceorder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-cancelserviceorder-api-openapi.yml
- filename: bell-canada-changerequest-api-openapi.yml
  format: yaml
  label: Bell Canada Change Request API
  slug: bell-canada-changerequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-changerequest-api-openapi.yml
- filename: bell-canada-events-subscription-api-openapi.yml
  format: yaml
  label: Bell Canada events subscription API
  slug: bell-canada-events-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-events-subscription-api-openapi.yml
- filename: bell-canada-logicalresource-api-openapi.yml
  format: yaml
  label: Bell Canada Logical Resource API
  slug: bell-canada-logicalresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-logicalresource-api-openapi.yml
- filename: bell-canada-notification-listeners-client-side-api-openapi.yml
  format: yaml
  label: Bell Canada notification listeners (client side) API
  slug: bell-canada-notification-listeners-client-side-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-notification-listeners-client-side-api-openapi.yml
- filename: bell-canada-physicalresource-api-openapi.yml
  format: yaml
  label: Bell Canada Physical Resource API
  slug: bell-canada-physicalresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-physicalresource-api-openapi.yml
- filename: bell-canada-resource-api-openapi.yml
  format: yaml
  label: Bell Canada Resource API
  slug: bell-canada-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-resource-api-openapi.yml
- filename: bell-canada-serviceorder-api-openapi.yml
  format: yaml
  label: Bell Canada Service Order API
  slug: bell-canada-serviceorder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-serviceorder-api-openapi.yml
- filename: bell-canada-troubleticket-api-openapi.yml
  format: yaml
  label: Bell Canada Trouble Ticket API
  slug: bell-canada-troubleticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-troubleticket-api-openapi.yml
consequence_counts:
  physical: 15
  read: 14
  write: 45
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bell Canada Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cancelServiceOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/cancelServiceOrderCreateEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/cancelServiceOrderInformationRequiredEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/cancelServiceOrderStateChangeEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderAttributeValueChangeEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderCreateEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderDeleteEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderFailureEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderInformationRequiredEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderJeopardyEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderMilestoneEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderStateChangeEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /serviceOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /serviceOrder/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /serviceOrder/{id}
operation_count: 74
overview: 'Bell Canada exposes 74 API operations that an AI agent could call, of which 60 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 45 write, and 15 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bell Canada
provider_slug: bell-canada
slug: bell-canada-agentic-access
source_filename: bell-canada-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/bell-canada-change-management-api-openapi.json, openapi/bell-canada-resource-inventory-api-openapi.json,\n  openapi/bell-canada-service-order-api-openapi.json, openapi/bell-canada-trouble-ticket-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 74\n  by_action_class:\n    connected: 14\n    acting: 60\n  by_consequence:\n    read: 14\n    write: 45\n    physical: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /changeRequest\n  method: get\n  operationId: listChangeRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changeRequest\n  method: post\n\
  \  operationId: createChangeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /changeRequest/{id}\n  method: get\n  operationId: retrieveChangeRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changeRequest/{id}\n  method: patch\n  operationId: patchChangeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /changeRequest/{id}\n  method: delete\n  operationId: deleteChangeRequest\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub\n  method: post\n  operationId: registerListener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/{id}\n  method: delete\n  operationId: unregisterListener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/changeRequestCreateEvent\n  method:\
  \ post\n  operationId: listenToChangeRequestCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/changeRequestStatusChangeEvent\n  method: post\n  operationId: listenToChangeRequestStatusChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/changeRequestDeleteEvent\n  method: post\n  operationId: listenToChangeRequestDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/changeRequestAttributeValueChangeEvent\n  method: post\n  operationId: listenToChangeRequestAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/changeRequestApprovalRequiredEvent\n  method: post\n  operationId: listenToChangeRequestApprovalRequiredEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/changeRequestFailureEvent\n  method: post\n  operationId:\
  \ listenToChangeRequestFailureEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logicalResource\n  method: get\n  operationId: listLogicalResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logicalResource\n  method: post\n  operationId: createLogicalResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logicalResource/executeJSONPatch\n  method: patch\n  operationId: executePatchResource\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logicalResource/{id}\n  method: get\n  operationId: retrieveLogicalResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logicalResource/{id}\n  method: put\n  operationId: updateLogicalResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logicalResource/{id}\n  method: patch\n  operationId: patchLogicalResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logicalResource/{id}\n  method: delete\n  operationId: deleteLogicalResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /physicalResource\n  method: get\n  operationId: listPhysicalResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /physicalResource\n  method: post\n  operationId: createPhysicalResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /physicalResource/{id}\n  method: get\n  operationId: retrievePhysicalResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /physicalResource/{id}\n  method: patch\n  operationId: patchPhysicalResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /physicalResource/{id}\n  method: delete\n  operationId: deletePhysicalResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resource\n  method: get\n  operationId: listResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource\n  method: post\n  operationId: createResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resource/{id}\n  method: get\n  operationId: retrieveResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/{id}\n  method: patch\n  operationId: patchResource\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resource/{id}\n  method: delete\n  operationId: deleteResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub\n  method: post\n  operationId: registerListener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/{id}\n  method: delete\n  operationId: unregisterListener\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/resourceCreateEvent\n  method: post\n  operationId: listenToResourceCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/resourceAttributeValueChangeEvent\n  method: post\n  operationId: listenToResourceAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /listener/resourceStateChangeEvent\n  method: post\n  operationId: listenToResourceStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/resourceDeleteEvent\n  method: post\n  operationId: listenToResourceDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/physicalResourceCreateEvent\n  method: post\n  operationId: listenToPhysicalResourceCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/physicalResourceAttributeValueChangeEvent\n  method: post\n  operationId: listenToPhysicalResourceAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/physicalResourceStateChangeEvent\n  method: post\n  operationId: listenToPhysicalResourceStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /listener/physicalResourceDeleteEvent\n  method: post\n  operationId: listenToPhysicalResourceDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancelServiceOrder\n  method: get\n  operationId: listCancelServiceOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cancelServiceOrder\n  method: post\n  operationId: createCancelServiceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /cancelServiceOrder/{id}\n  method: get\n  operationId: retrieveCancelServiceOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serviceOrder\n  method: get\n  operationId: listServiceOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serviceOrder\n  method: post\n  operationId: createServiceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serviceOrder/{id}\n  method: get\n  operationId: retrieveServiceOrder\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serviceOrder/{id}\n  method: patch\n  operationId: patchServiceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serviceOrder/{id}\n  method: delete\n  operationId: deleteServiceOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub\n  method: post\n\
  \  operationId: registerListener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/{id}\n  method: delete\n  operationId: unregisterListener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/serviceOrderCreateEvent\n  method: post\n  operationId: listenToServiceOrderCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/serviceOrderAttributeValueChangeEvent\n  method: post\n  operationId: listenToServiceOrderAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/serviceOrderStateChangeEvent\n  method: post\n  operationId: listenToServiceOrderStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /listener/serviceOrderDeleteEvent\n  method: post\n  operationId: listenToServiceOrderDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/serviceOrderInformationRequiredEvent\n  method: post\n  operationId: listenToServiceOrderInformationRequiredEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/serviceOrderMilestoneEvent\n  method: post\n  operationId: listenToServiceOrderMilestoneEvent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/serviceOrderJeopardyEvent\n  method: post\n  operationId: listenToServiceOrderJeopardyEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/cancelServiceOrderCreateEvent\n  method: post\n  operationId: listenToCancelServiceOrderCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/cancelServiceOrderStateChangeEvent\n  method: post\n  operationId: listenToCancelServiceOrderStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/cancelServiceOrderInformationRequiredEvent\n  method: post\n  operationId: listenToCancelServiceOrderInformationRequiredEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/serviceOrderFailureEvent\n  method: post\n  operationId: listenToServiceOrderFailureEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /troubleTicket\n  method: get\n  operationId: listTroubleTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /troubleTicket\n  method: post\n  operationId: createTroubleTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /troubleTicket/{id}\n  method: get\n  operationId: retrieveTroubleTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /troubleTicket/{id}\n  method: patch\n  operationId: patchTroubleTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /troubleTicket/{id}\n  method: delete\n  operationId: deleteTroubleTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub\n  method: post\n  operationId: registerListener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/{id}\n  method: delete\n  operationId: unregisterListener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketCreateEvent\n  method: post\n  operationId: listenToTroubleTicketCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketAttributeValueChangeEvent\n  method: post\n  operationId: listenToTroubleTicketAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketStatusChangeEvent\n  method: post\n  operationId: listenToTroubleTicketStatusChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /listener/troubleTicketDeleteEvent\n  method: post\n  operationId: listenToTroubleTicketDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketResolvedEvent\n  method: post\n  operationId: listenToTroubleTicketResolvedEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketInformationRequiredEvent\n  method: post\n  operationId: listenToTroubleTicketInformationRequiredEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/agentic-access/bell-canada-agentic-access.yml
summary_line: 74 operations · 60 acting
tags:
- Telecommunications
- Canada
- Mobile Network Operator
- Broadband
- 5G
- IoT
- TM Forum
- BSS
- OSS
- Network APIs
- CAMARA
- Open Gateway
- Identity Verification
- SIM Swap
- Enterprise
---
