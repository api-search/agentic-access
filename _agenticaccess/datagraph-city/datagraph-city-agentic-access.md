---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 22
api_specs:
- filename: datagraph-city-admin-api-openapi.yml
  format: yaml
  label: DataGraph.city Admin API
  slug: datagraph-city-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-admin-api-openapi.yml
- filename: datagraph-city-analytics-api-openapi.yml
  format: yaml
  label: DataGraph.city Analytics API
  slug: datagraph-city-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-analytics-api-openapi.yml
- filename: datagraph-city-api-key-api-openapi.yml
  format: yaml
  label: DataGraph.city Api Key API
  slug: datagraph-city-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-api-key-api-openapi.yml
- filename: datagraph-city-authorize-api-openapi.yml
  format: yaml
  label: DataGraph.city Authorize API
  slug: datagraph-city-authorize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-authorize-api-openapi.yml
- filename: datagraph-city-billing-api-openapi.yml
  format: yaml
  label: DataGraph.city Billing API
  slug: datagraph-city-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-billing-api-openapi.yml
- filename: datagraph-city-cities-api-openapi.yml
  format: yaml
  label: DataGraph.city Cities API
  slug: datagraph-city-cities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-cities-api-openapi.yml
- filename: datagraph-city-datasets-api-openapi.yml
  format: yaml
  label: DataGraph.city Datasets API
  slug: datagraph-city-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-datasets-api-openapi.yml
- filename: datagraph-city-health-api-openapi.yml
  format: yaml
  label: DataGraph.city Health API
  slug: datagraph-city-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-health-api-openapi.yml
- filename: datagraph-city-mcp-api-openapi.yml
  format: yaml
  label: DataGraph.city MCP API
  slug: datagraph-city-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-mcp-api-openapi.yml
- filename: datagraph-city-me-api-openapi.yml
  format: yaml
  label: DataGraph.city Me API
  slug: datagraph-city-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-me-api-openapi.yml
- filename: datagraph-city-metrics-api-openapi.yml
  format: yaml
  label: DataGraph.city Metrics API
  slug: datagraph-city-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-metrics-api-openapi.yml
- filename: datagraph-city-query-api-openapi.yml
  format: yaml
  label: DataGraph.city Query API
  slug: datagraph-city-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-query-api-openapi.yml
- filename: datagraph-city-resend-api-key-api-openapi.yml
  format: yaml
  label: DataGraph.city Resend Api Key API
  slug: datagraph-city-resend-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-resend-api-key-api-openapi.yml
- filename: datagraph-city-schema-api-openapi.yml
  format: yaml
  label: DataGraph.city Schema API
  slug: datagraph-city-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-schema-api-openapi.yml
- filename: datagraph-city-signup-api-openapi.yml
  format: yaml
  label: DataGraph.city Signup API
  slug: datagraph-city-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-signup-api-openapi.yml
- filename: datagraph-city-token-api-openapi.yml
  format: yaml
  label: DataGraph.city Token API
  slug: datagraph-city-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-token-api-openapi.yml
- filename: datagraph-city-usage-api-openapi.yml
  format: yaml
  label: DataGraph.city Usage API
  slug: datagraph-city-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-usage-api-openapi.yml
- filename: datagraph-city-webhooks-api-openapi.yml
  format: yaml
  label: DataGraph.city Webhooks API
  slug: datagraph-city-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-webhooks-api-openapi.yml
- filename: datagraph-city-well-known-api-openapi.yml
  format: yaml
  label: DataGraph.city .well Known API
  slug: datagraph-city-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagraph-city/openapi/datagraph-city-well-known-api-openapi.yml
consequence_counts:
  physical: 1
  read: 22
  safety-critical: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Datagraph City Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api-key/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api-key/reset-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /resend-api-key
operation_count: 33
overview: 'DataGraph.city exposes 33 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 8 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DataGraph.city
provider_slug: datagraph-city
slug: datagraph-city-agentic-access
source_filename: datagraph-city-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/datagraph-city-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 22\n    acting: 11\n  by_consequence:\n    read: 22\n    write: 8\n    physical: 1\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /.well-known/oauth-protected-resource/mcp\n  method: get\n  operationId: well_known_protected_resource__well_known_oauth_protected_resource_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: well_known_protected_resource__well_known_oauth_protected_resource_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: well_known_authorization_server__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorize\n  method: get\n  operationId: authorize_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorize/email\n  method: post\n  operationId: authorize_email_authorize_email_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /authorize/verify\n  method: get\n  operationId: authorize_verify_authorize_verify_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorize/approve\n  method: post\n  operationId: authorize_approve_authorize_approve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token\n  method: post\n  operationId: token_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signup\n  method: post\n  operationId: signup_signup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/update-tier\n  method: post\n  operationId: update_user_tier_admin_update_tier_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/list-users\n  method: get\n  operationId: list_all_users_admin_list_users_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/update-rate-limit\n  method: post\n  operationId: update_user_rate_limit_endpoint_admin_update_rate_limit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resend-api-key\n  method: post\n  operationId: resend_api_key_resend_api_key_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n\
  \  operationId: get_current_user_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: get_usage_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cities\n  method: get\n  operationId: list_cities_cities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: get\n  operationId: list_datasets_datasets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{locality}/schema\n  method: get\n  operationId: get_locality_schema_api__locality__schema_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{locality}/query\n  method: post\n  operationId: query_locality_data_api__locality__query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp_handler_mcp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/daily\n  method: get\n  operationId: daily_metrics_metrics_daily_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/tiers\n  method: get\n  operationId: tier_metrics_metrics_tiers_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/weekly\n  method: get\n  operationId: weekly_summary_metrics_weekly_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/queries/insights\n  method: get\n  operationId: query_insights_analytics_queries_insights_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/queries/top\n  method: get\n  operationId: top_queries_analytics_queries_top_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/queries/unanswered\n  method: get\n  operationId: unanswered_queries_analytics_queries_unanswered_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/queries/export\n  method: get\n  operationId: export_queries_analytics_queries_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-key/reset-request\n  method: post\n  operationId: request_api_key_reset_api_key_reset_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api-key/view\n  method: get\n  operationId: view_api_key_api_key_view_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-key/reset\n  method: post\n  operationId: reset_api_key_api_key_reset_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /billing/portal\n  method: post\n  operationId: get_billing_portal_billing_portal_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/stripe\n  method: post\n  operationId: stripe_webhook_webhooks_stripe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/datagraph-city/agentic-access/datagraph-city-agentic-access.yml
summary_line: 33 operations · 11 acting · 2 human-in-the-loop
tags:
- Urban Data
- Artificial Intelligence
- MCP
- Graph RAG
- Private Beta
---
