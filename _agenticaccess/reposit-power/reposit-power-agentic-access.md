---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 28
api_specs:
- filename: reposit-power-auth-api-openapi.yml
  format: yaml
  label: Reposit Power Auth API
  slug: reposit-power-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-auth-api-openapi.yml
- filename: reposit-power-battery-api-openapi.yml
  format: yaml
  label: Reposit Power Battery API
  slug: reposit-power-battery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-battery-api-openapi.yml
- filename: reposit-power-curtailment-api-openapi.yml
  format: yaml
  label: Reposit Power Curtailment API
  slug: reposit-power-curtailment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-curtailment-api-openapi.yml
- filename: reposit-power-deployment-api-openapi.yml
  format: yaml
  label: Reposit Power Deployment API
  slug: reposit-power-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-deployment-api-openapi.yml
- filename: reposit-power-dispatch-api-openapi.yml
  format: yaml
  label: Reposit Power Dispatch API
  slug: reposit-power-dispatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-dispatch-api-openapi.yml
- filename: reposit-power-inverter-api-openapi.yml
  format: yaml
  label: Reposit Power Inverter API
  slug: reposit-power-inverter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-inverter-api-openapi.yml
- filename: reposit-power-network-api-openapi.yml
  format: yaml
  label: Reposit Power Network API
  slug: reposit-power-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-network-api-openapi.yml
- filename: reposit-power-node-api-openapi.yml
  format: yaml
  label: Reposit Power Node API
  slug: reposit-power-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-node-api-openapi.yml
- filename: reposit-power-power-station-api-openapi.yml
  format: yaml
  label: Reposit Power Power Station API
  slug: reposit-power-power-station-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-power-station-api-openapi.yml
- filename: reposit-power-solar-api-openapi.yml
  format: yaml
  label: Reposit Power Solar API
  slug: reposit-power-solar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-solar-api-openapi.yml
- filename: reposit-power-users-api-openapi.yml
  format: yaml
  label: Reposit Power Users API
  slug: reposit-power-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/openapi/reposit-power-users-api-openapi.yml
consequence_counts:
  read: 28
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Reposit Power Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/dispatches
operation_count: 39
overview: 'Reposit Power exposes 39 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 10 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Reposit Power
provider_slug: reposit-power
slug: reposit-power-agentic-access
source_filename: reposit-power-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/reposit-power-customer-api-openapi.yml, openapi/reposit-power-market-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 11\n    connected: 28\n  by_consequence:\n    write: 10\n    read: 28\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v2/auth/login/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/refresh/\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/userkeys/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{userkey}/components\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{userkey}/battery/capacity\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{userkey}/generation/historical/p\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{userkey}/inverter/historical/p\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{userkey}/house/historical\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{userkey}/battery/historical/soc\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{userkey}/meter/historical/p\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{userkey}/gridcredits/historical\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nodes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nodes/{nodeId}/address\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nodes/{nodeId}/network\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nodes/{nodeId}/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nodes/{nodeId}/namePlate\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nodes/{nodeId}/events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/powerstations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/powerstations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/powerstations/{powerstationId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/powerstations/{powerstationId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/powerstations/{powerstationId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/powerstations/{powerstationId}/data\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/powerstations/{powerstationId}/data/raw\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/powerstations/{powerstationId}/data/latest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/constraints/curtailments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/curtailments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/curtailments\n  method: post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/curtailments/{curtailmentId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/curtailments/{curtailmentId}/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/curtailments/setpoint\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/curtailments/setpoint\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/curtailments/heartbeat\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dispatches\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dispatches\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/dispatches/{dispatchId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/capabilities\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reposit-power/refs/heads/main/agentic-access/reposit-power-agentic-access.yml
summary_line: 39 operations · 11 acting · 1 human-in-the-loop
tags:
- Energy
- Australia
- Utilities
- Electricity
- Batteries
- DER
- Virtual Power Plant
- Demand Response
- Solar
- Grid
- Energy Markets
- Smart Metering
- Storage
- Flexibility
---
