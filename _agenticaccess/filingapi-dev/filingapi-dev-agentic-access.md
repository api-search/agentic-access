---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 28
api_specs:
- filename: filingapi-dev-admin-api-openapi.yml
  format: yaml
  label: FilingAPI Admin API
  slug: filingapi-dev-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-admin-api-openapi.yml
- filename: filingapi-dev-calendar-api-openapi.yml
  format: yaml
  label: FilingAPI Calendar API
  slug: filingapi-dev-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-calendar-api-openapi.yml
- filename: filingapi-dev-checkout-api-openapi.yml
  format: yaml
  label: FilingAPI Checkout API
  slug: filingapi-dev-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-checkout-api-openapi.yml
- filename: filingapi-dev-company-api-openapi.yml
  format: yaml
  label: FilingAPI Company API
  slug: filingapi-dev-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-company-api-openapi.yml
- filename: filingapi-dev-earnings-filings-api-api-openapi.yml
  format: yaml
  label: FilingAPI Earnings & Filings API
  slug: filingapi-dev-earnings-filings-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-earnings-filings-api-api-openapi.yml
- filename: filingapi-dev-favicon-ico-api-openapi.yml
  format: yaml
  label: FilingAPI Favicon.ico API
  slug: filingapi-dev-favicon-ico-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-favicon-ico-api-openapi.yml
- filename: filingapi-dev-filings-api-openapi.yml
  format: yaml
  label: FilingAPI Filings API
  slug: filingapi-dev-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-filings-api-openapi.yml
- filename: filingapi-dev-health-api-openapi.yml
  format: yaml
  label: FilingAPI Health API
  slug: filingapi-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-health-api-openapi.yml
- filename: filingapi-dev-insiders-api-openapi.yml
  format: yaml
  label: FilingAPI Insiders API
  slug: filingapi-dev-insiders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-insiders-api-openapi.yml
- filename: filingapi-dev-mcp-api-openapi.yml
  format: yaml
  label: FilingAPI MCP API
  slug: filingapi-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-mcp-api-openapi.yml
- filename: filingapi-dev-model-api-openapi.yml
  format: yaml
  label: FilingAPI Model API
  slug: filingapi-dev-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-model-api-openapi.yml
- filename: filingapi-dev-sectors-api-openapi.yml
  format: yaml
  label: FilingAPI Sectors API
  slug: filingapi-dev-sectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-sectors-api-openapi.yml
- filename: filingapi-dev-signals-api-openapi.yml
  format: yaml
  label: FilingAPI Signals API
  slug: filingapi-dev-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-signals-api-openapi.yml
- filename: filingapi-dev-signup-api-openapi.yml
  format: yaml
  label: FilingAPI Signup API
  slug: filingapi-dev-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-signup-api-openapi.yml
- filename: filingapi-dev-transcripts-api-openapi.yml
  format: yaml
  label: FilingAPI Transcripts API
  slug: filingapi-dev-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-transcripts-api-openapi.yml
- filename: filingapi-dev-verify-api-openapi.yml
  format: yaml
  label: FilingAPI Verify API
  slug: filingapi-dev-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-verify-api-openapi.yml
- filename: filingapi-dev-webhooks-api-openapi.yml
  format: yaml
  label: FilingAPI Webhooks API
  slug: filingapi-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingapi-dev/openapi/filingapi-dev-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 28
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Filingapi Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout
operation_count: 36
overview: 'FilingAPI exposes 36 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 7 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FilingAPI
provider_slug: filingapi-dev
slug: filingapi-dev-agentic-access
source_filename: filingapi-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/filingapi-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 28\n    acting: 8\n  by_consequence:\n    read: 28\n    physical: 1\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/checkout\n  method: get\n  operationId: create_checkout_v1_checkout_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout\n  method: post\n  operationId: create_checkout_v1_checkout_get\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/success\n  method: get\n  operationId: checkout_success_v1_checkout_success_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/stripe\n  method: post\n  operationId: stripe_webhook_v1_webhooks_stripe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signup/free\n  method: get\n  operationId: free_signup_v1_signup_free_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signup/free\n  method: post\n  operationId: free_signup_v1_signup_free_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify\n  method: get\n  operationId: verify_email_v1_verify_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/metrics\n  method: get\n  operationId: admin_metrics_v1_admin_metrics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/reddit-post\n  method: post\n  operationId: add_reddit_post_v1_admin_reddit_post_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/reddit-post/{post_id}\n  method: delete\n  operationId: delete_reddit_post_v1_admin_reddit_post__post_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/todo\n  method: post\n  operationId: add_todo_v1_admin_todo_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/admin/todo/{todo_id}/toggle\n  method: patch\n  operationId: toggle_todo_v1_admin_todo__todo_id__toggle_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/todo/{todo_id}\n  method: delete\n  operationId: delete_todo_v1_admin_todo__todo_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/dashboard\n  method: get\n  operationId: admin_dashboard_admin_dashboard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insiders/{ticker}\n  method: get\n  operationId: get_insider_transactions_v1_insiders__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insiders/{ticker}/summary\n  method: get\n  operationId: get_insider_summary_v1_insiders__ticker__summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model\n  method: get\n  operationId: model_page_model_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /favicon.ico\n\
  \  method: get\n  operationId: favicon_favicon_ico_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: get\n  operationId: mcp_redirect_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings/{ticker}\n  method: get\n  operationId: get_filings_v1_filings__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings/{ticker}/guidance\n  method: get\n  operationId: get_guidance_v1_filings__ticker__guidance_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings/{ticker}/{accession}\n  method: get\n  operationId: get_filing_detail_v1_filings__ticker___accession__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings\n  method: get\n  operationId: search_filings_v1_filings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendar/earnings\n  method: get\n  operationId: get_earnings_calendar_v1_calendar_earnings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcripts/{ticker}\n  method: get\n  operationId: get_transcripts_v1_transcripts__ticker__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sectors\n  method: get\n  operationId: list_sectors_v1_sectors_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sectors/{sector}\n  method: get\n  operationId: get_sector_tickers_v1_sectors__sector__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sectors/{sector}/filings\n  method: get\n  operationId: get_sector_filings_v1_sectors__sector__filings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sectors/{sector}/guidance\n  method: get\n  operationId: get_sector_guidance_v1_sectors__sector__guidance_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/{ticker}\n  method: get\n  operationId: get_company_info_v1_company__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcripts/{ticker}/fetch\n  method: get\n  operationId: fetch_transcripts_on_demand_v1_transcripts__ticker__fetch_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/latest\n  method: get\n  operationId: get_latest_signals_v1_signals_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendar/macro\n  method: get\n  operationId: get_macro_calendar_v1_calendar_macro_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendar/macro/history\n  method: get\n  operationId: get_macro_history_v1_calendar_macro_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/filingapi-dev/agentic-access/filingapi-dev-agentic-access.yml
summary_line: 36 operations · 8 acting
tags:
- Financial Data
- SEC Filings
- Earnings
- Macro Economic
- Sentiment Analysis
- Quantitative Finance
- MCP Server
- REST API
---
