---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: claroty-authenticate-api-openapi.yml
  format: yaml
  label: Claroty Authenticate API
  slug: claroty-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-authenticate-api-openapi.yml
- filename: claroty-health-api-openapi.yml
  format: yaml
  label: Claroty Health API
  slug: claroty-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-health-api-openapi.yml
- filename: claroty-is-key-registered-api-openapi.yml
  format: yaml
  label: Claroty Is Key Registered API
  slug: claroty-is-key-registered-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-is-key-registered-api-openapi.yml
- filename: claroty-jwks-api-openapi.yml
  format: yaml
  label: Claroty Jwks API
  slug: claroty-jwks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-jwks-api-openapi.yml
- filename: claroty-jwthenticator-api-openapi.yml
  format: yaml
  label: Claroty JW Thenticator API
  slug: claroty-jwthenticator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-jwthenticator-api-openapi.yml
- filename: claroty-refresh-api-openapi.yml
  format: yaml
  label: Claroty Refresh API
  slug: claroty-refresh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-refresh-api-openapi.yml
- filename: claroty-register-key-api-openapi.yml
  format: yaml
  label: Claroty Register Key API
  slug: claroty-register-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-register-key-api-openapi.yml
- filename: claroty-validate-api-openapi.yml
  format: yaml
  label: Claroty Validate API
  slug: claroty-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-validate-api-openapi.yml
- filename: claroty-validate-request-api-openapi.yml
  format: yaml
  label: Claroty Validate Request API
  slug: claroty-validate-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/openapi/claroty-validate-request-api-openapi.yml
consequence_counts:
  read: 4
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Claroty Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Claroty exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Claroty
provider_slug: claroty
slug: claroty-agentic-access
source_filename: claroty-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/claroty-jwthenticator-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 4\n    acting: 5\n  by_consequence:\n    read: 4\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: check_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: check_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /register_key\n  method: post\n  operationId:\
  \ register_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /is_key_registered\n  method: post\n  operationId: is_key_registered\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authenticate\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /refresh\n  method: post\n  operationId: refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate\n  method: post\n  operationId: validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate_request\n  method: get\n  operationId: validate_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jwks\n  method: get\n  operationId: jwks\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claroty/refs/heads/main/agentic-access/claroty-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- Company
- Cybersecurity
- OT Security
- Cyber-Physical Systems
- IoT Security
- Industrial Control Systems
- Threat Detection
- Exposure Management
- Healthcare Security
---
