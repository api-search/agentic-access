---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 14
api_specs:
- filename: zaptec-chargehistory-api-openapi.yml
  format: yaml
  label: Zaptec Charge History API
  slug: zaptec-chargehistory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-chargehistory-api-openapi.yml
- filename: zaptec-charger-api-openapi.yml
  format: yaml
  label: Zaptec Charger API
  slug: zaptec-charger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-charger-api-openapi.yml
- filename: zaptec-chargerfirmware-api-openapi.yml
  format: yaml
  label: Zaptec Charger Firmware API
  slug: zaptec-chargerfirmware-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-chargerfirmware-api-openapi.yml
- filename: zaptec-constants-api-openapi.yml
  format: yaml
  label: Zaptec Constants API
  slug: zaptec-constants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-constants-api-openapi.yml
- filename: zaptec-installation-api-openapi.yml
  format: yaml
  label: Zaptec Installation API
  slug: zaptec-installation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-installation-api-openapi.yml
- filename: zaptec-session-api-openapi.yml
  format: yaml
  label: Zaptec Session API
  slug: zaptec-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-session-api-openapi.yml
- filename: zaptec-user-group-api-openapi.yml
  format: yaml
  label: Zaptec User Group API
  slug: zaptec-user-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-user-group-api-openapi.yml
consequence_counts:
  physical: 3
  read: 14
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zaptec Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargehistory/installationreport
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargers/{id}/sendCommand/{commandId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargers/{id}/update
operation_count: 19
overview: 'Zaptec exposes 19 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 2 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zaptec
provider_slug: zaptec
slug: zaptec-agentic-access
source_filename: zaptec-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/api_zaptec_swagger.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 14\n    acting: 5\n  by_consequence:\n    read: 14\n    physical: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/chargehistory\n  method: get\n  operationId: api_chargehistory_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargehistory/installationreport\n  method: get\n  operationId: api_chargehistory_installationreport_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/chargehistory/installationreport\n  method: post\n  operationId: api_chargehistory_installationreport_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers\n  method: get\n  operationId: api_chargers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{id}\n  method: get\n  operationId: api_chargers_{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{id}/update\n  method: post\n  operationId:\
  \ api_chargers_{id}_update_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{id}/state\n  method: get\n  operationId: api_chargers_{id}_state_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{id}/sendCommand/{commandId}\n  method: post\n  operationId: api_chargers_{id}_sendcommand_{commandid}_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargerFirmware/installation/{installationId}\n  method: get\n  operationId: api_chargerfirmware_installation_{installationid}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/constants\n  method: get\n  operationId: api_constants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/installation\n  method: get\n  operationId: api_installation_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/installation/{id}\n  method: get\n  operationId: api_installation_{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/installation/{id}/messagingConnectionDetails\n  method: get\n  operationId: api_installation_{id}_messagingconnectiondetails_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/installation/{id}/update\n  method: post\n  operationId: api_installation_{id}_update_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/installation/{id}/hierarchy\n  method: get\n  operationId: api_installation_{id}_hierarchy_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sessions/archived\n  method: get\n \
  \ operationId: api_sessions_archived_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/session/{id}\n  method: get\n  operationId: api_session_{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/session/{id}/priority\n  method: post\n  operationId: api_session_{id}_priority_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/userGroups/{id}/messagingConnectionDetails\n  method: get\n  operationId: api_usergroups_{id}_messagingconnectiondetails_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/zaptec/agentic-access/zaptec-agentic-access.yml
summary_line: 19 operations · 5 acting
tags:
- Company
- EV Charging
- Smart Charging
- Energy
- Sustainability
- Platform
---
