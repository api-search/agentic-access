---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 21
api_specs:
- filename: edlink-agents-api-openapi.yml
  format: yaml
  label: Edlink Agents API
  slug: edlink-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-agents-api-openapi.yml
- filename: edlink-classes-api-openapi.yml
  format: yaml
  label: Edlink Classes API
  slug: edlink-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-classes-api-openapi.yml
- filename: edlink-courses-api-openapi.yml
  format: yaml
  label: Edlink Courses API
  slug: edlink-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-courses-api-openapi.yml
- filename: edlink-districts-api-openapi.yml
  format: yaml
  label: Edlink Districts API
  slug: edlink-districts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-districts-api-openapi.yml
- filename: edlink-enrollments-api-openapi.yml
  format: yaml
  label: Edlink Enrollments API
  slug: edlink-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-enrollments-api-openapi.yml
- filename: edlink-events-api-openapi.yml
  format: yaml
  label: Edlink Events API
  slug: edlink-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-events-api-openapi.yml
- filename: edlink-graph-api-openapi.yml
  format: yaml
  label: Edlink Graph API
  slug: edlink-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-graph-api-openapi.yml
- filename: edlink-integrations-api-openapi.yml
  format: yaml
  label: Edlink Integrations API
  slug: edlink-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-integrations-api-openapi.yml
- filename: edlink-people-api-openapi.yml
  format: yaml
  label: Edlink People API
  slug: edlink-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-people-api-openapi.yml
- filename: edlink-schools-api-openapi.yml
  format: yaml
  label: Edlink Schools API
  slug: edlink-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-schools-api-openapi.yml
- filename: edlink-sections-api-openapi.yml
  format: yaml
  label: Edlink Sections API
  slug: edlink-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-sections-api-openapi.yml
- filename: edlink-sso-api-openapi.yml
  format: yaml
  label: Edlink SSO API
  slug: edlink-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-sso-api-openapi.yml
consequence_counts:
  read: 21
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Edlink Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Edlink exposes 22 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Edlink
provider_slug: edlink
slug: edlink-agentic-access
source_filename: edlink-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/edlink-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 21\n    acting: 1\n  by_consequence:\n    read: 21\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /graph/people\n  method: get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/people/{id}\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/classes\n  method: get\n  operationId:\
  \ listClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/classes/{id}\n  method: get\n  operationId: getClass\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/classes/{id}/enrollments\n  method: get\n  operationId: listClassEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/enrollments\n  method: get\n  operationId: listEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/enrollments/{id}\n  method: get\n  operationId: getEnrollment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/schools\n  method: get\n  operationId: listSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/schools/{id}\n  method: get\n  operationId: getSchool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/districts\n  method: get\n  operationId: listDistricts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/districts/{id}\n  method: get\n  operationId: getDistrict\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/courses\n  method: get\n  operationId: listCourses\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/courses/{id}\n  method: get\n  operationId: getCourse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/sections\n  method: get\n  operationId: listSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/sections/{id}\n  method: get\n  operationId: getSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/agents/{id}\n\
  \  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graph/integrations/{id}\n  method: get\n  operationId: getIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta/integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /my/profile\n  method: get\n  operationId: getMyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/token\n  method: post\n  operationId: createOauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/agentic-access/edlink-agentic-access.yml
summary_line: 22 operations · 1 acting
tags:
- Education
- EdTech
- Rostering
- SIS
- LMS
- Integration
- Unified-API
---
