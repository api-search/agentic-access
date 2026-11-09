---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 8
api_specs:
- filename: intencheck-com-analyze-api-openapi.yml
  format: yaml
  label: intencheck-com Analyze API
  slug: intencheck-com-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-analyze-api-openapi.yml
- filename: intencheck-com-api-keys-api-openapi.yml
  format: yaml
  label: intencheck-com API Keys API
  slug: intencheck-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-api-keys-api-openapi.yml
- filename: intencheck-com-checkout-api-openapi.yml
  format: yaml
  label: intencheck-com Checkout API
  slug: intencheck-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-checkout-api-openapi.yml
- filename: intencheck-com-demo-api-openapi.yml
  format: yaml
  label: intencheck-com Demo API
  slug: intencheck-com-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-demo-api-openapi.yml
- filename: intencheck-com-docs-api-openapi.yml
  format: yaml
  label: intencheck-com Docs API
  slug: intencheck-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-docs-api-openapi.yml
- filename: intencheck-com-mcp-api-openapi.yml
  format: yaml
  label: intencheck-com MCP API
  slug: intencheck-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-mcp-api-openapi.yml
- filename: intencheck-com-reply-api-openapi.yml
  format: yaml
  label: intencheck-com Reply API
  slug: intencheck-com-reply-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-reply-api-openapi.yml
- filename: intencheck-com-report-error-api-openapi.yml
  format: yaml
  label: intencheck-com Report Error API
  slug: intencheck-com-report-error-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-report-error-api-openapi.yml
- filename: intencheck-com-transactions-api-openapi.yml
  format: yaml
  label: intencheck-com Transactions API
  slug: intencheck-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-transactions-api-openapi.yml
- filename: intencheck-com-webhooks-api-openapi.yml
  format: yaml
  label: intencheck-com Webhooks API
  slug: intencheck-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Intencheck Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/checkout
operation_count: 21
overview: 'intencheck-com exposes 21 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 11 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: intencheck-com
provider_slug: intencheck-com
slug: intencheck-com-agentic-access
source_filename: intencheck-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/intencheck-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 8\n    acting: 13\n  by_consequence:\n    read: 8\n    write: 11\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/mcp/status\n  method: get\n  operationId: mcp_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analyze/batch\n  method: post\n  operationId: create_batch_analyze_api_v1_analyze_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/analyze/batch\n  method: get\n  operationId: list_batch_jobs_api_v1_analyze_batch_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analyze/batch/{job_id}\n  method: get\n  operationId: get_batch_job_status_api_v1_analyze_batch__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analyze/batch/{job_id}/results\n  method: get\n  operationId: get_batch_job_results_api_v1_analyze_batch__job_id__results_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/analyze\n  method: post\n  operationId: analyze_text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/demo/analyze\n  method: post\n  operationId: demo_analyze_text_api_v1_demo_analyze_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/analyze/bulk\n  method: post\n  operationId: analyze_text_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/analyze/sentiment\n  method: post\n  operationId: analyze_sentiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reply\n  method: post\n  operationId: generate_reply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/demo/reply\n  method: post\n  operationId: demo_generate_reply_api_v1_demo_reply_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions\n  method: get\n  operationId: get_transactions_api_v1_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/checkout\n  method: post\n  operationId: process_checkout_api_v1_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/stripe\n  method: post\n  operationId: stripe_webhook_api_v1_webhooks_stripe_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/report-error\n  method: post\n  operationId: report_error_api_v1_report_error_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/keys/usage\n  method: get\n  operationId: get_user_usage_stats_api_v1_keys_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys\n  method: get\n  operationId: list_api_keys_api_v1_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys\n  method: post\n  operationId: create_api_key_api_v1_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/keys/{key_id}\n  method: delete\n  operationId: revoke_api_key_api_v1_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/keys/{key_id}/rotate\n  method: post\n  operationId: rotate_api_key_api_v1_keys__key_id__rotate_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /developers\n  method: get\n  operationId: developers_page_developers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/intencheck-com/agentic-access/intencheck-com-agentic-access.yml
summary_line: 21 operations · 13 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Natural Language Processing
- Text Analysis
- Sentiment
- Emotion
---
