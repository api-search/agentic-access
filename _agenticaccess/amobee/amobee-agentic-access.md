---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: amobee-env-vars-test-controller-api-openapi.yml
  format: yaml
  label: Amobee Env Vars Test Controller API
  slug: amobee-env-vars-test-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-env-vars-test-controller-api-openapi.yml
- filename: amobee-gateway-swagger-controller-api-openapi.yml
  format: yaml
  label: Amobee Gateway Swagger Controller API
  slug: amobee-gateway-swagger-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-gateway-swagger-controller-api-openapi.yml
- filename: amobee-health-check-api-openapi.yml
  format: yaml
  label: Amobee Health Check API
  slug: amobee-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-health-check-api-openapi.yml
- filename: amobee-ip-controller-api-openapi.yml
  format: yaml
  label: Amobee Ip Controller API
  slug: amobee-ip-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-ip-controller-api-openapi.yml
- filename: amobee-tcf-disclosure-controller-api-openapi.yml
  format: yaml
  label: Amobee Tcf Disclosure Controller API
  slug: amobee-tcf-disclosure-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/openapi/amobee-tcf-disclosure-controller-api-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Amobee Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /swagger-config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /swagger-config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /swagger-config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /swagger-config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /swagger-resources
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /swagger-resources
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /swagger-resources
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /swagger-resources
operation_count: 19
overview: 'Amobee exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amobee
provider_slug: amobee
slug: amobee-agentic-access
source_filename: amobee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/amobee-env-vars-test-controller-api-openapi.yml, openapi/amobee-gateway-swagger-controller-api-openapi.yml,\n  openapi/amobee-health-check-api-openapi.yml, openapi/amobee-ip-controller-api-openapi.yml,\n  openapi/amobee-tcf-disclosure-controller-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 11\n    acting: 8\n  by_consequence:\n    read: 11\n    safety-critical: 8\n  human_in_the_loop_required: 8\noperations:\n- path: /env-vars-test\n  method: get\n  operationId: getVars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swagger-resources\n\
  \  method: get\n  operationId: swaggerResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swagger-resources\n  method: put\n  operationId: swaggerResources_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /swagger-resources\n  method: post\n  operationId: swaggerResources_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /swagger-resources\n\
  \  method: delete\n  operationId: swaggerResources_3\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /swagger-resources\n  method: options\n  operationId: swaggerResources_6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swagger-resources\n  method: head\n  operationId: swaggerResources_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swagger-resources\n  method: patch\n  operationId: swaggerResources_4\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /swagger-config\n  method: get\n  operationId: swaggerConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swagger-config\n  method: put\n  operationId: swaggerConfig_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /swagger-config\n  method: post\n  operationId: swaggerConfig_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /swagger-config\n  method: delete\n  operationId: swaggerConfig_3\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /swagger-config\n  method: options\n  operationId: swaggerConfig_6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swagger-config\n  method: head\n  operationId: swaggerConfig_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /swagger-config\n  method: patch\n  operationId: swaggerConfig_4\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /healthcheck/status\n  method: get\n  operationId: getAppname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ip\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/TCFDisclosure.json\n  method: get\n  operationId: getTCFDisclosure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/TCFDisclosure\n  method: get\n  operationId: getTCFDisclosure_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/agentic-access/amobee-agentic-access.yml
summary_line: 19 operations · 8 acting · 8 human-in-the-loop
tags:
- Digital Advertising
- DSP
- Programmatic
- Campaign Management
- Audience Targeting
- Data Management Platform
- AdTech
- Samsung Ads
---
