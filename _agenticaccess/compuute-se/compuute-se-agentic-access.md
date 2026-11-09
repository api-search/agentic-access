---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 8
api_specs:
- filename: compuute-se-auth-api-openapi.yml
  format: yaml
  label: compuute-se Auth API
  slug: compuute-se-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-auth-api-openapi.yml
- filename: compuute-se-billing-api-openapi.yml
  format: yaml
  label: compuute-se Billing API
  slug: compuute-se-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-billing-api-openapi.yml
- filename: compuute-se-health-api-openapi.yml
  format: yaml
  label: compuute-se Health API
  slug: compuute-se-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-health-api-openapi.yml
- filename: compuute-se-scan-api-openapi.yml
  format: yaml
  label: compuute-se Scan API
  slug: compuute-se-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-scan-api-openapi.yml
- filename: compuute-se-scan-x402-api-openapi.yml
  format: yaml
  label: compuute-se Scan X402 API
  slug: compuute-se-scan-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-scan-x402-api-openapi.yml
- filename: compuute-se-search-api-openapi.yml
  format: yaml
  label: compuute-se Search API
  slug: compuute-se-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-search-api-openapi.yml
- filename: compuute-se-subscribe-api-openapi.yml
  format: yaml
  label: compuute-se Subscribe API
  slug: compuute-se-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-subscribe-api-openapi.yml
- filename: compuute-se-usage-api-openapi.yml
  format: yaml
  label: compuute-se Usage API
  slug: compuute-se-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-usage-api-openapi.yml
- filename: compuute-se-validate-api-openapi.yml
  format: yaml
  label: compuute-se Validate API
  slug: compuute-se-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-validate-api-openapi.yml
- filename: compuute-se-x402-api-openapi.yml
  format: yaml
  label: compuute-se X402 API
  slug: compuute-se-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compuute-se/openapi/compuute-se-x402-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Compuute Se Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/auth/key
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 17
overview: 'compuute-se exposes 17 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 7 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: compuute-se
provider_slug: compuute-se
slug: compuute-se-agentic-access
source_filename: compuute-se-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/leads-compuute-se-openapi.json, openapi/scan-compuute-se-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 9\n    connected: 8\n  by_consequence:\n    write: 7\n    safety-critical: 1\n    read: 8\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/auth/register\n  method: post\n  operationId: register_v1_auth_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/key\n\
  \  method: delete\n  operationId: revoke_key_v1_auth_key_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: health_check_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: post\n  operationId: search_leads_v1_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validate\n  method: post\n  operationId: validate_leads_v1_validate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscribe\n  method: post\n  operationId: create_subscription_v1_subscribe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions\n  method: get\n  operationId: list_subscriptions_v1_subscriptions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions/{subscription_id}\n  method: delete\n  operationId: cancel_subscription_v1_subscriptions__subscription_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/checkout\n  method: post\n  operationId: create_checkout_v1_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: customer_portal_v1_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/billing/status\n  method: get\n  operationId: billing_status_v1_billing_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: get_usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search/pay\n  method: post\n  operationId: search_with_x402_payment_v1_search_pay_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scan\n  method: post\n  operationId: scan_endpoint_v1_scan_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scan/info\n  method: get\n  operationId: scan_info_v1_scan_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scan/pay\n  method: post\n  operationId: scan_with_x402_v1_scan_pay_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: health_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/compuute-se/agentic-access/compuute-se-agentic-access.yml
summary_line: 17 operations · 9 acting · 1 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Security
- MCP
- Compliance
- Sweden
- AI Agents
---
