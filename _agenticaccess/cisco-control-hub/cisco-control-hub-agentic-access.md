---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 11
api_specs:
- filename: openapi.json
  format: json
  label: Webex Admin API
  slug: webex-admin-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Calling API
  slug: webex-calling-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Devices API
  slug: webex-devices-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Workspaces API
  slug: webex-workspaces-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex People API
  slug: webex-people-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Organizations API
  slug: webex-organizations-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Licenses API
  slug: webex-licenses-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Locations API
  slug: webex-locations-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
- filename: openapi.json
  format: json
  label: Webex Reports API
  slug: webex-reports-api
  spec_type: OpenAPI
  url: https://developer.webex.com/docs/api/v1/openapi.json
consequence_counts:
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cisco Control Hub Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Cisco Control Hub exposes 17 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cisco Control Hub
provider_slug: cisco-control-hub
slug: cisco-control-hub-agentic-access
source_filename: cisco-control-hub-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cisco-control-hub-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 11\n    acting: 6\n  by_consequence:\n    read: 11\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /adminAuditEvents\n  method: get\n  operationId: listAdminAuditEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{orgId}\n\
  \  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{orgId}\n  method: delete\n  operationId: deleteOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people\n  method: get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people\n  method: post\n  operationId: createPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{personId}\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{personId}\n  method: put\n  operationId: updatePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{personId}\n  method: delete\n  operationId: deletePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /licenses\n  method: get\n  operationId: listLicenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licenses/{licenseId}\n  method: get\n  operationId: getLicense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: post\n  operationId: createLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}\n\
  \  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}\n  method: put\n  operationId: updateLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/agentic-access/cisco-control-hub-agentic-access.yml
summary_line: 17 operations · 6 acting
tags:
- Administration
- Calling
- Collaboration
- Communications
- Device Management
- Identity Management
- Licenses
- Reporting
- Webex
---
