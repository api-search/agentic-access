---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: dillilabs-com-analyze-api-openapi.yml
  format: yaml
  label: Dilli Labs Analyze API
  slug: dillilabs-com-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-analyze-api-openapi.yml
- filename: dillilabs-com-health-api-openapi.yml
  format: yaml
  label: Dilli Labs Health API
  slug: dillilabs-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-health-api-openapi.yml
- filename: dillilabs-com-privacy-api-openapi.yml
  format: yaml
  label: Dilli Labs Privacy API
  slug: dillilabs-com-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-privacy-api-openapi.yml
- filename: dillilabs-com-purchase-api-openapi.yml
  format: yaml
  label: Dilli Labs Purchase API
  slug: dillilabs-com-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-purchase-api-openapi.yml
- filename: dillilabs-com-user-api-openapi.yml
  format: yaml
  label: Dilli Labs User API
  slug: dillilabs-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-user-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dillilabs Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase/verify/{device_id}
operation_count: 5
overview: 'Dilli Labs exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dilli Labs
provider_slug: dillilabs-com
slug: dillilabs-com-agentic-access
source_filename: dillilabs-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dillilabs-com-mind-your-tongue-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    write: 1\n    read: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /analyze\n  method: post\n  operationId: analyze_text_analyze_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{device_id}\n  method: get\n  operationId: get_user_info_user__device_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchase/verify/{device_id}\n  method: post\n  operationId: verify_purchase_purchase_verify__device_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /privacy\n  method: get\n  operationId: get_privacy_policy_privacy_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dillilabs-com/agentic-access/dillilabs-com-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Company
- Email Verification
- IP Geolocation
- IP Validation
- Profanity Detection
- MCP
- Software-as-a-Service
- Web Hosting
- Software Development
---
