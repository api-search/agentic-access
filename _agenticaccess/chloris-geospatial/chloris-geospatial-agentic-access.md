---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 10
api_specs:
- filename: chloris-geospatial-aoi-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Aoi API
  slug: chloris-geospatial-aoi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-aoi-api-openapi.yml
- filename: chloris-geospatial-boundary-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Boundary API
  slug: chloris-geospatial-boundary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-boundary-api-openapi.yml
- filename: chloris-geospatial-collection-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Collection API
  slug: chloris-geospatial-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-collection-api-openapi.yml
- filename: chloris-geospatial-info-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Info API
  slug: chloris-geospatial-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-info-api-openapi.yml
- filename: chloris-geospatial-invite-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Invite API
  slug: chloris-geospatial-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-invite-api-openapi.yml
- filename: chloris-geospatial-mgrstiles-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Mgrs Tiles API
  slug: chloris-geospatial-mgrstiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-mgrstiles-api-openapi.yml
- filename: chloris-geospatial-organization-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Organization API
  slug: chloris-geospatial-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-organization-api-openapi.yml
- filename: chloris-geospatial-reportingunit-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Reporting Unit API
  slug: chloris-geospatial-reportingunit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-reportingunit-api-openapi.yml
- filename: chloris-geospatial-user-api-openapi.yml
  format: yaml
  label: Chloris Geospatial User API
  slug: chloris-geospatial-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-user-api-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chloris Geospatial Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invite
operation_count: 15
overview: 'Chloris Geospatial exposes 15 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chloris Geospatial
provider_slug: chloris-geospatial
slug: chloris-geospatial-agentic-access
source_filename: chloris-geospatial-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: generated\nsource: openapi/chloris-geospatial-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 10\n    acting: 5\n  by_consequence:\n    read: 10\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /info\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization\n  method: post\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/usage\n\
  \  method: post\n  operationId: listOrganizationUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reportingUnit\n  method: put\n  operationId: putReportingUnit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reportingUnit\n  method: post\n  operationId: listReportingUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reportingUnit\n  method: delete\n  operationId: deleteReportingUnit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mgrsTiles\n  method: get\n  operationId: getMgrsTilesFromBoundary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mgrsTiles/{id}\n  method: get\n  operationId: getMgrsTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method: post\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invite\n  method: post\n  operationId: sendInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boundary\n  method: post\n  operationId: uploadBoundary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boundary\n  method: get\n  operationId: getBoundaryUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collection\n  method: put\n  operationId: putCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /aoi/submit\n  method: get\n  operationId: submitAoiToSandbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aoi/healthz\n  method: get\n  operationId: sandboxHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/agentic-access/chloris-geospatial-agentic-access.yml
summary_line: 15 operations · 5 acting
tags:
- Company
- Geospatial
- Carbon
- Data
- Environmental
---
