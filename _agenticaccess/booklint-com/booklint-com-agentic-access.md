---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: booklint-com-booklint-api-openapi.yml
  format: yaml
  label: booklint-com Booklint API
  slug: booklint-com-booklint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-booklint-api-openapi.yml
- filename: booklint-com-check-accounts-tieout-api-openapi.yml
  format: yaml
  label: booklint-com Check Accounts Tieout API
  slug: booklint-com-check-accounts-tieout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-accounts-tieout-api-openapi.yml
- filename: booklint-com-check-api-openapi.yml
  format: yaml
  label: booklint-com Check API
  slug: booklint-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-api-openapi.yml
- filename: booklint-com-check-budget-variance-api-openapi.yml
  format: yaml
  label: booklint-com Check Budget Variance API
  slug: booklint-com-check-budget-variance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-budget-variance-api-openapi.yml
- filename: booklint-com-check-invoice-api-openapi.yml
  format: yaml
  label: booklint-com Check Invoice API
  slug: booklint-com-check-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-invoice-api-openapi.yml
- filename: booklint-com-check-quote-math-api-openapi.yml
  format: yaml
  label: booklint-com Check Quote Math API
  slug: booklint-com-check-quote-math-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-check-quote-math-api-openapi.yml
- filename: booklint-com-health-api-openapi.yml
  format: yaml
  label: booklint-com Health API
  slug: booklint-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-health-api-openapi.yml
- filename: booklint-com-keys-api-openapi.yml
  format: yaml
  label: booklint-com Keys API
  slug: booklint-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-keys-api-openapi.yml
- filename: booklint-com-llms-txt-api-openapi.yml
  format: yaml
  label: booklint-com Llms.txt API
  slug: booklint-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-llms-txt-api-openapi.yml
- filename: booklint-com-mcp-api-openapi.yml
  format: yaml
  label: booklint-com MCP API
  slug: booklint-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-mcp-api-openapi.yml
- filename: booklint-com-openapi-json-api-openapi.yml
  format: yaml
  label: booklint-com Openapi.json API
  slug: booklint-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-openapi-json-api-openapi.yml
- filename: booklint-com-plans-api-openapi.yml
  format: yaml
  label: booklint-com Plans API
  slug: booklint-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-plans-api-openapi.yml
- filename: booklint-com-privacy-api-openapi.yml
  format: yaml
  label: booklint-com Privacy API
  slug: booklint-com-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-privacy-api-openapi.yml
- filename: booklint-com-sample-api-openapi.yml
  format: yaml
  label: booklint-com Sample API
  slug: booklint-com-sample-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-sample-api-openapi.yml
- filename: booklint-com-terms-api-openapi.yml
  format: yaml
  label: booklint-com Terms API
  slug: booklint-com-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/booklint-com/openapi/booklint-com-terms-api-openapi.yml
consequence_counts:
  physical: 6
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Booklint Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mcp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/check_accounts_tieout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/check_budget_variance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/check_invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/check_quote_math
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/keys
operation_count: 16
overview: 'booklint-com exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 1 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: booklint-com
provider_slug: booklint-com
slug: booklint-com-agentic-access
source_filename: booklint-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/booklint-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 9\n    acting: 7\n  by_consequence:\n    read: 9\n    write: 1\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: get_llms_txt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId:\
  \ get_openapi_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: get_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans\n  method: get\n  operationId: get_v1_plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sample\n  method: get\n  operationId: get_v1_sample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check\n  method: post\n  operationId: post_v1_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys\n  method: post\n  operationId: post_v1_keys\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/{session}\n  method: get\n  operationId: get_v1_keys_session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: post_mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/check_invoice\n  method: post\n  operationId: post_v1_check_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/check_quote_math\n  method: post\n  operationId: post_v1_check_quote_math\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/check_budget_variance\n\
  \  method: post\n  operationId: post_v1_check_budget_variance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/check_accounts_tieout\n  method: post\n  operationId: post_v1_check_accounts_tieout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terms\n  method: get\n  operationId: get_terms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /privacy\n  method: get\n  operationId: get_privacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/booklint-com/agentic-access/booklint-com-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- Finance
- Spending
- Automation
- Guardrails
- Software-as-a-Service
---
