---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: cove.tool-authentication-token-api-openapi.yml
  format: yaml
  label: Cove.Tool Authentication Token API
  slug: cove.tool-authentication-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-authentication-token-api-openapi.yml
- filename: cove.tool-daylight-analysis-api-openapi.yml
  format: yaml
  label: Cove.Tool Daylight Analysis API
  slug: cove.tool-daylight-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-daylight-analysis-api-openapi.yml
- filename: cove.tool-energy-codes-api-openapi.yml
  format: yaml
  label: Cove.Tool Energy Codes API
  slug: cove.tool-energy-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-energy-codes-api-openapi.yml
- filename: cove.tool-profiles-api-openapi.yml
  format: yaml
  label: Cove.Tool Profiles API
  slug: cove.tool-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-profiles-api-openapi.yml
- filename: cove.tool-project-geometry-api-openapi.yml
  format: yaml
  label: Cove.Tool Project Geometry API
  slug: cove.tool-project-geometry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-project-geometry-api-openapi.yml
- filename: cove.tool-projects-api-openapi.yml
  format: yaml
  label: Cove.Tool Projects API
  slug: cove.tool-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-projects-api-openapi.yml
- filename: cove.tool-user-api-openapi.yml
  format: yaml
  label: Cove.Tool User API
  slug: cove.tool-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-user-api-openapi.yml
consequence_counts:
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cove.Tool Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Cove.Tool exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cove.Tool
provider_slug: cove.tool
slug: cove.tool-agentic-access
source_filename: cove.tool-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/cove.tool-authentication-token-api-openapi.yml, openapi/cove.tool-daylight-analysis-api-openapi.yml,\n  openapi/cove.tool-energy-codes-api-openapi.yml, openapi/cove.tool-profiles-api-openapi.yml,\n  openapi/cove.tool-project-geometry-api-openapi.yml, openapi/cove.tool-projects-api-openapi.yml,\n  openapi/cove.tool-user-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 7\n    connected: 7\n  by_consequence:\n    write: 7\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /get-token\n  method: post\n  operationId: postGetToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis\n  method: post\n  operationId: postAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/{project_id}\n  method: get\n  operationId: getAnalysisByProjectId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/{project_id}/status\n  method: get\n  operationId: getAnalysisByProjectIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /analysis/{project_id}/stop\n  method: get\n  operationId: getAnalysisByProjectIdStop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /energy-codes\n  method: get\n  operationId: getEnergyCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}\n  method: get\n  operationId: getProfilesByProfileId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /run-values\n  method: post\n  operationId: postRunValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /projects/{project_id}/geometry\n  method: post\n  operationId: postProjectsByProjectIdGeometry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: get\n  operationId: getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/\n  method: post\n  operationId: postProjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/\n  method: get\n  operationId:\
  \ getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: put\n  operationId: putProjectsByProjectId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/signup\n  method: post\n  operationId: postAuthSignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/agentic-access/cove.tool-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Company
- Building Performance
- Energy Modeling
- Daylight Analysis
- Sustainability
- Architecture
- AEC
- Simulation
- Embodied Carbon
- Building Design
---
