---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 20
api_specs:
- filename: shiftmove-custom-fields-api-openapi.yml
  format: yaml
  label: Shiftmove Custom fields API
  slug: shiftmove-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-custom-fields-api-openapi.yml
- filename: shiftmove-driver-assignments-api-openapi.yml
  format: yaml
  label: Shiftmove Driver assignments API
  slug: shiftmove-driver-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-driver-assignments-api-openapi.yml
- filename: shiftmove-drivers-api-openapi.yml
  format: yaml
  label: Shiftmove Drivers API
  slug: shiftmove-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-drivers-api-openapi.yml
- filename: shiftmove-invoices-api-openapi.yml
  format: yaml
  label: Shiftmove Invoices API
  slug: shiftmove-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-invoices-api-openapi.yml
- filename: shiftmove-organizations-api-openapi.yml
  format: yaml
  label: Shiftmove Organizations API
  slug: shiftmove-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-organizations-api-openapi.yml
- filename: shiftmove-vehicle-assignments-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicle assignments API
  slug: shiftmove-vehicle-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicle-assignments-api-openapi.yml
- filename: shiftmove-vehicle-financing-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicle financing API
  slug: shiftmove-vehicle-financing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicle-financing-api-openapi.yml
- filename: shiftmove-vehicle-license-plates-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicle license plates API
  slug: shiftmove-vehicle-license-plates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicle-license-plates-api-openapi.yml
- filename: shiftmove-vehicle-usages-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicle usages API
  slug: shiftmove-vehicle-usages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicle-usages-api-openapi.yml
- filename: shiftmove-vehicles-api-openapi.yml
  format: yaml
  label: Shiftmove Vehicles API
  slug: shiftmove-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/openapi/shiftmove-vehicles-api-openapi.yml
consequence_counts:
  read: 20
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shiftmove Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'Shiftmove exposes 40 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shiftmove
provider_slug: shiftmove
slug: shiftmove-agentic-access
source_filename: shiftmove-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/shiftmove-custom-fields-api-openapi.yml, openapi/shiftmove-driver-assignments-api-openapi.yml,\n  openapi/shiftmove-drivers-api-openapi.yml, openapi/shiftmove-invoices-api-openapi.yml, openapi/shiftmove-organizations-api-openapi.yml,\n  openapi/shiftmove-vehicle-assignments-api-openapi.yml, openapi/shiftmove-vehicle-financing-api-openapi.yml,\n  openapi/shiftmove-vehicle-license-plates-api-openapi.yml, openapi/shiftmove-vehicle-usages-api-openapi.yml,\n  openapi/shiftmove-vehicles-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 20\n    acting: 20\n  by_consequence:\n    read: 20\n    write: 20\n  human_in_the_loop_required: 0\n\
  operations:\n- path: /v1/customFields/drivers\n  method: get\n  operationId: getDriverCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customFields/vehicles\n  method: get\n  operationId: getVehicleCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drivers/{uuid}/assignments\n  method: get\n  operationId: findDriverAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drivers/{uuid}/assignments\n  method: post\n  operationId: createDriverAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drivers/{uuid}/assignments/query\n  method: post\n  operationId: queryDriverAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drivers/{uuid}/assignments/{assignmentUuid}\n  method: delete\n  operationId: deleteDriverAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drivers/{uuid}/assignments/{assignmentUuid}/duration\n  method: post\n  operationId: updateDriverAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drivers\n  method: get\n  operationId: getAllDrivers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drivers\n  method: post\n  operationId: createDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drivers/query\n  method: post\n  operationId: queryDrivers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drivers/{uuid}\n  method: get\n  operationId: findDriverByUuid\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drivers/{uuid}\n  method: post\n  operationId: updateDriverByUuid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drivers/{uuid}/customFieldValues/{customFieldUuid}\n  method: post\n  operationId: setDriverCustomFieldValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/drivers/{uuid}/stateHistory\n  method: post\n  operationId: setDriverState\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoices\n  method: get\n  operationId: getAllInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/query\n  method: post\n  operationId: queryInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/{invoiceUuid}/items\n  method: get\n  operationId: getAllInvoicesItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/{invoiceUuid}/rawFile\n  method: get\n  operationId: getInvoiceRawFileUpload\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations\n  method: get\n  operationId: getAllOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{uuid}/assignments\n  method: get\n  operationId: findVehicleAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{uuid}/assignments\n  method: post\n  operationId: createVehicleAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{uuid}/assignments/query\n\
  \  method: post\n  operationId: queryVehicleAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{uuid}/assignments/{assignmentUuid}\n  method: delete\n  operationId: deleteVehicleAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{uuid}/assignments/{assignmentUuid}/duration\n  method: post\n  operationId: updateVehicleAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/vehicles/{uuid}/financing/current\n  method: get\n  operationId: getVehicleCurrentFinancing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{uuid}/licensePlates\n  method: get\n  operationId: findVehicleLicensePlates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{uuid}/licensePlates\n  method: post\n  operationId: createVehicleLicensePlates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{uuid}/licensePlates/{licensePlateUuid}\n  method: delete\n  operationId: deleteVehicleLicensePlates\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{uuid}/licensePlates/{licensePlateUuid}/duration\n  method: post\n  operationId: updateVehicleLicensePlates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{uuid}/usages\n  method: get\n  operationId: findVehicleUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{uuid}/usages\n  method: post\n  operationId: createVehicleUsage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles\n  method: get\n  operationId: getAllVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles\n  method: post\n  operationId: createVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/query\n  method: post\n  operationId: queryVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{uuid}\n  method: get\n  operationId: findVehicleByUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vehicles/{uuid}\n  method: post\n  operationId: updateVehicleByUuid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{uuid}/archive\n  method: post\n  operationId: archiveVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{uuid}/costCenter\n\
  \  method: post\n  operationId: updateVehicleCostCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{uuid}/customFieldValues/{customFieldUuid}\n  method: post\n  operationId: setVehicleCustomFieldValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicles/{uuid}/subCompany\n  method: post\n  operationId: createVehicleSubCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiftmove/refs/heads/main/agentic-access/shiftmove-agentic-access.yml
summary_line: 40 operations · 20 acting
tags:
- Company
- Fleet Management
- Mobility
- Automotive
- Telematics
- Vehicles
- Fleet API
- Software-as-a-Service
---
