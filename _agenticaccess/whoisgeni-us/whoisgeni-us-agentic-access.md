---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 30
api_specs:
- filename: whoisgeni-us-account-api-openapi.yml
  format: yaml
  label: whoisgeni-us Account API
  slug: whoisgeni-us-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-account-api-openapi.yml
- filename: whoisgeni-us-analysis-api-openapi.yml
  format: yaml
  label: whoisgeni-us Analysis API
  slug: whoisgeni-us-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-analysis-api-openapi.yml
- filename: whoisgeni-us-authentication-api-openapi.yml
  format: yaml
  label: whoisgeni-us Authentication API
  slug: whoisgeni-us-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-authentication-api-openapi.yml
- filename: whoisgeni-us-billing-api-openapi.yml
  format: yaml
  label: whoisgeni-us Billing API
  slug: whoisgeni-us-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-billing-api-openapi.yml
- filename: whoisgeni-us-byok-api-openapi.yml
  format: yaml
  label: whoisgeni-us Byok API
  slug: whoisgeni-us-byok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-byok-api-openapi.yml
- filename: whoisgeni-us-correlation-api-openapi.yml
  format: yaml
  label: whoisgeni-us Correlation API
  slug: whoisgeni-us-correlation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-correlation-api-openapi.yml
- filename: whoisgeni-us-domains-api-openapi.yml
  format: yaml
  label: whoisgeni-us Domains API
  slug: whoisgeni-us-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-domains-api-openapi.yml
- filename: whoisgeni-us-entities-api-openapi.yml
  format: yaml
  label: whoisgeni-us Entities API
  slug: whoisgeni-us-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-entities-api-openapi.yml
- filename: whoisgeni-us-health-api-openapi.yml
  format: yaml
  label: whoisgeni-us Health API
  slug: whoisgeni-us-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-health-api-openapi.yml
- filename: whoisgeni-us-jobs-api-openapi.yml
  format: yaml
  label: whoisgeni-us Jobs API
  slug: whoisgeni-us-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-jobs-api-openapi.yml
- filename: whoisgeni-us-mcp-api-openapi.yml
  format: yaml
  label: whoisgeni-us MCP API
  slug: whoisgeni-us-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-mcp-api-openapi.yml
- filename: whoisgeni-us-schema-templates-api-openapi.yml
  format: yaml
  label: whoisgeni-us Schema Templates API
  slug: whoisgeni-us-schema-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-schema-templates-api-openapi.yml
- filename: whoisgeni-us-webhooks-api-openapi.yml
  format: yaml
  label: whoisgeni-us Webhooks API
  slug: whoisgeni-us-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-webhooks-api-openapi.yml
consequence_counts:
  physical: 4
  read: 30
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Whoisgeni Us Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /auth/keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /billing/auto-recharge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/auto-recharge/setup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/credits/checkout
operation_count: 52
overview: 'whoisgeni-us exposes 52 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 17 write, 4 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: whoisgeni-us
provider_slug: whoisgeni-us
slug: whoisgeni-us-agentic-access
source_filename: whoisgeni-us-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/whoisgeni-us-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 30\n    acting: 22\n  by_consequence:\n    read: 30\n    write: 17\n    safety-critical: 1\n    physical: 4\n  human_in_the_loop_required: 1\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: get\n  operationId: version_version_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /health/ready\n  method: get\n  operationId: readiness_check_health_ready_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/auth\n  method: get\n  operationId: auth_pipeline_check_health_auth_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/verify-token\n  method: post\n  operationId: verify_token_auth_verify_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/me\n  method: get\n  operationId: get_me_auth_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/me\n  method: delete\n  operationId: delete_me_auth_me_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/keys\n  method: get\n  operationId: list_api_keys_auth_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/keys\n  method: post\n  operationId: create_api_key_auth_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /auth/session-key\n  method: post\n  operationId: create_session_key_auth_session_key_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/keys/{key_id}\n  method: delete\n  operationId: revoke_api_key_auth_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/email-preferences\n  method: get\n  operationId: get_email_preferences_auth_email_preferences_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/email-preferences\n  method: patch\n  operationId: update_email_preferences_auth_email_preferences_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/me/export\n  method: get\n  operationId: export_me_auth_me_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/checkout\n  method: post\n  operationId: create_checkout_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/portal\n  method: get\n  operationId: get_portal_billing_portal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/subscription\n  method: get\n  operationId: get_subscription_billing_subscription_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/credits/checkout\n  method: post\n  operationId: create_credit_checkout_billing_credits_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /billing/credits\n  method: get\n  operationId: get_credits_billing_credits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/ledger\n  method: get\n  operationId: get_credit_ledger_billing_ledger_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/auto-recharge\n  method: get\n  operationId: get_auto_recharge_billing_auto_recharge_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/auto-recharge\n  method: put\n  operationId: update_auto_recharge_billing_auto_recharge_put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/auto-recharge/setup\n  method: post\n  operationId: setup_auto_recharge_card_billing_auto_recharge_setup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/usage\n  method: get\n  operationId: get_usage_dashboard_billing_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/llm-keys\n  method: get\n  operationId: list_byok_keys_account_llm_keys_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/llm-keys\n  method: post\n  operationId: save_byok_key_account_llm_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/llm-keys/{provider}\n  method: delete\n  operationId: delete_byok_key_account_llm_keys__provider__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyze\n  method: post\n  operationId: submit_analysis_analyze_post\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyze/batch\n  method: post\n  operationId: submit_batch_analysis_analyze_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyze/bulk\n  method: post\n  operationId: submit_bulk_analysis_analyze_bulk_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /jobs\n  method: get\n  operationId: list_jobs_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}\n  method: get\n  operationId: get_job_status_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/signals\n  method: get\n  operationId: get_job_signals_jobs__job_id__signals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/subdomains\n  method: get\n  operationId: get_job_subdomains_jobs__job_id__subdomains_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/certificate\n\
  \  method: get\n  operationId: get_job_certificate_jobs__job_id__certificate_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{job_id}/status\n  method: get\n  operationId: get_webhook_status_webhooks__job_id__status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/secret\n  method: post\n  operationId: create_webhook_secret_webhooks_secret_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/secret\n  method: get\n  operationId: get_webhook_secret_webhooks_secret_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/dead-letter/{delivery_id}/retry\n  method: post\n  operationId: retry_dead_letter_webhook_webhooks_dead_letter__delivery_id__retry_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/dead-letter\n  method: get\n  operationId: list_dead_letter_webhooks_webhooks_dead_letter_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}/history\n  method: get\n  operationId: get_domain_history_domains__domain__history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}/portfolio\n  method: get\n  operationId: get_domain_portfolio_domains__domain__portfolio_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/search\n  method: get\n  operationId: search_entities_entities_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/{name}/portfolio\n  method: get\n  operationId: get_entity_portfolio_entities__name__portfolio_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /correlate\n  method: post\n  operationId: submit_correlation_correlate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /correlate/{correlation_id}\n  method: get\n  operationId: get_correlation_status_correlate__correlation_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/templates\n  method: post\n  operationId: create_template_schemas_templates_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas/templates\n  method: get\n  operationId: list_templates_schemas_templates_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/templates/{template_id}\n  method: get\n  operationId: get_template_schemas_templates__template_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/templates/{template_id}\n  method: put\n  operationId: update_template_schemas_templates__template_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schemas/templates/{template_id}\n  method: delete\n  operationId: delete_template_schemas_templates__template_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp_endpoint_mcp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/whoisgeni-us/agentic-access/whoisgeni-us-agentic-access.yml
summary_line: 52 operations · 22 acting · 1 human-in-the-loop
tags:
- Company
- Domain Intelligence
- Security
- Compliance
- Data Enrichment
---
