---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 7
api_specs:
- filename: treblle-analytics-api-openapi.yml
  format: yaml
  label: Treblle Analytics API
  slug: treblle-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-analytics-api-openapi.yml
- filename: treblle-endpoints-api-openapi.yml
  format: yaml
  label: Treblle Endpoints API
  slug: treblle-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-endpoints-api-openapi.yml
- filename: treblle-governance-api-openapi.yml
  format: yaml
  label: Treblle Governance API
  slug: treblle-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-governance-api-openapi.yml
- filename: treblle-members-api-openapi.yml
  format: yaml
  label: Treblle Members API
  slug: treblle-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-members-api-openapi.yml
- filename: treblle-projects-api-openapi.yml
  format: yaml
  label: Treblle Projects API
  slug: treblle-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-projects-api-openapi.yml
- filename: treblle-requests-api-openapi.yml
  format: yaml
  label: Treblle Requests API
  slug: treblle-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/openapi/treblle-requests-api-openapi.yml
consequence_counts:
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Treblle Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Treblle exposes 12 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Treblle
provider_slug: treblle
slug: treblle-agentic-access
source_filename: treblle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/treblle-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 7\n    acting: 5\n  by_consequence:\n    read: 7\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}\n  method: put\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /projects/{projectId}/requests\n  method: get\n  operationId: listRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/requests/{requestId}\n  method: get\n  operationId: getRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/analytics\n  method: get\n  operationId: getProjectAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/endpoints\n  method: get\n  operationId: listEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/governance\n  method: post\n \
  \ operationId: runGovernanceCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/members\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/members\n  method: post\n  operationId: inviteMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treblle/refs/heads/main/agentic-access/treblle-agentic-access.yml
summary_line: 12 operations · 5 acting
tags:
- Analytics
- Artificial Intelligence
- Developer Experience
- Documentation
- Governance
- Insights
- Observability
- Platform
- Security
- Testing
---
