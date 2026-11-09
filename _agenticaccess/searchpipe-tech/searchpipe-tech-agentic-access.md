---
acting_count: 34
action_class_counts:
  acting: 34
  connected: 82
api_specs:
- filename: searchpipe-tech-account-api-openapi.yml
  format: yaml
  label: searchpipe-tech Account API
  slug: searchpipe-tech-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-account-api-openapi.yml
- filename: searchpipe-tech-admin-api-openapi.yml
  format: yaml
  label: searchpipe-tech Admin API
  slug: searchpipe-tech-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-admin-api-openapi.yml
- filename: searchpipe-tech-agent-setup-api-openapi.yml
  format: yaml
  label: searchpipe-tech Agent Setup API
  slug: searchpipe-tech-agent-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-agent-setup-api-openapi.yml
- filename: searchpipe-tech-api-keys-api-openapi.yml
  format: yaml
  label: searchpipe-tech API Keys API
  slug: searchpipe-tech-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-api-keys-api-openapi.yml
- filename: searchpipe-tech-auth-api-openapi.yml
  format: yaml
  label: searchpipe-tech Auth API
  slug: searchpipe-tech-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-auth-api-openapi.yml
- filename: searchpipe-tech-billing-api-openapi.yml
  format: yaml
  label: searchpipe-tech Billing API
  slug: searchpipe-tech-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-billing-api-openapi.yml
- filename: searchpipe-tech-dashboard-api-openapi.yml
  format: yaml
  label: searchpipe-tech Dashboard API
  slug: searchpipe-tech-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-dashboard-api-openapi.yml
- filename: searchpipe-tech-extract-api-openapi.yml
  format: yaml
  label: searchpipe-tech Extract API
  slug: searchpipe-tech-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-extract-api-openapi.yml
- filename: searchpipe-tech-feedback-api-openapi.yml
  format: yaml
  label: searchpipe-tech Feedback API
  slug: searchpipe-tech-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-feedback-api-openapi.yml
- filename: searchpipe-tech-healthz-api-openapi.yml
  format: yaml
  label: searchpipe-tech Healthz API
  slug: searchpipe-tech-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-healthz-api-openapi.yml
- filename: searchpipe-tech-messages-api-openapi.yml
  format: yaml
  label: searchpipe-tech Messages API
  slug: searchpipe-tech-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-messages-api-openapi.yml
- filename: searchpipe-tech-payments-api-openapi.yml
  format: yaml
  label: searchpipe-tech Payments API
  slug: searchpipe-tech-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-payments-api-openapi.yml
- filename: searchpipe-tech-search-api-openapi.yml
  format: yaml
  label: searchpipe-tech Search API
  slug: searchpipe-tech-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-search-api-openapi.yml
- filename: searchpipe-tech-seo-api-openapi.yml
  format: yaml
  label: searchpipe-tech Seo API
  slug: searchpipe-tech-seo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-seo-api-openapi.yml
- filename: searchpipe-tech-site-api-openapi.yml
  format: yaml
  label: searchpipe-tech Site API
  slug: searchpipe-tech-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-site-api-openapi.yml
- filename: searchpipe-tech-usage-api-openapi.yml
  format: yaml
  label: searchpipe-tech Usage API
  slug: searchpipe-tech-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-usage-api-openapi.yml
- filename: searchpipe-tech-verify-api-openapi.yml
  format: yaml
  label: searchpipe-tech Verify API
  slug: searchpipe-tech-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/searchpipe-tech/openapi/searchpipe-tech-verify-api-openapi.yml
consequence_counts:
  physical: 11
  read: 82
  safety-critical: 3
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Searchpipe Tech Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dashboard/reset-password
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /auth/resend-verification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /dashboard/resend-verification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/orders/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/orders/{order_id}/confirm-failed
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/orders/{order_id}/confirm-paid
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/orders/{order_id}/resume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/subscription/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/subscription/resume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/webhooks/{provider}
operation_count: 116
overview: 'searchpipe-tech exposes 116 API operations that an AI agent could call, of which 34 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 82 read, 20 write, 11 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: searchpipe-tech
provider_slug: searchpipe-tech
slug: searchpipe-tech-agentic-access
source_filename: searchpipe-tech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/searchpipe-tech-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 116\n  by_action_class:\n    connected: 82\n    acting: 34\n  by_consequence:\n    read: 82\n    write: 20\n    safety-critical: 3\n    physical: 11\n  human_in_the_loop_required: 3\noperations:\n- path: /robots.txt\n  method: get\n  operationId: robots_txt_robots_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  operationId: sitemap_xml_sitemap_xml_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms_txt_llms_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: landing__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /terms\n  method: get\n  operationId: terms_page_terms_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /privacy\n  method: get\n  operationId: privacy_page_privacy_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search-api\n  method: get\n  operationId: search_api_page_search_api_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs\n  method: get\n  operationId: public_docs_docs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/search\n  method: get\n  operationId: docs_search_reference_docs_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/extract\n  method: get\n  operationId: docs_extract_reference_docs_extract_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/verify\n  method: get\n  operationId: docs_verify_reference_docs_verify_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /docs/mcp\n  method: get\n  operationId: docs_mcp_reference_docs_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp-server\n  method: get\n  operationId: mcp_server_page_mcp_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents\n  method: get\n  operationId: agents_setup_page_agents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: pricing_page_pricing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web-search-mcp\n  method: get\n  operationId: web_search_mcp_page_web_search_mcp_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web-search-api-for-ai-agents\n  method: get\n  operationId: web_search_api_for_agents_page_web_search_api_for_ai_agents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compare\n  method: get\n  operationId: compare_page_compare_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify-api\n  method: get\n  operationId: verify_api_page_verify_api_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faq\n  method: get\n  operationId: faq_page_faq_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /benchmarks\n  method: get\n  operationId: benchmarks_page_benchmarks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extract-api\n  method: get\n  operationId: extract_api_page_extract_api_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations\n  method: get\n  operationId: integrations_page_integrations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blog\n  method: get\n  operationId: blog_index_page_blog_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /blog/search-api-benchmarks-2026\n  method: get\n  operationId: blog_benchmark_article_page_blog_search_api_benchmarks_2026_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact\n  method: get\n  operationId: contact_page_contact_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/register\n  method: post\n  operationId: register_auth_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login\n  method: post\n  operationId: login_auth_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/refresh\n  method: post\n  operationId: refresh_auth_refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/forgot-password\n  method: post\n  operationId: forgot_password_auth_forgot_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/reset-password\n  method: post\n  operationId:\
  \ reset_password_auth_reset_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/oauth/github\n  method: get\n  operationId: oauth_github_auth_oauth_github_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/github/callback\n  method: get\n  operationId: oauth_github_callback_auth_oauth_github_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/google\n  method: get\n  operationId: oauth_google_auth_oauth_google_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/google/callback\n  method: get\n  operationId: oauth_google_callback_auth_oauth_google_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/verify-email\n  method: get\n  operationId: verify_email_auth_verify_email_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/resend-verification\n  method: post\n  operationId: resend_verification_auth_resend_verification_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /auth/me\n  method: get\n  operationId: me_auth_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys\n  method: post\n  operationId: create_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-keys\n  method: get\n  operationId: list_all_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/reveal\n  method: get\n  operationId: reveal_default_api_keys_reveal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/{key_id}/reveal\n  method: get\n  operationId: reveal_one_api_keys__key_id__reveal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/{key_id}\n  method: delete\n  operationId: revoke_api_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /billing/balance\n  method: get\n  operationId: balance_billing_balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/transactions\n  method:\
  \ get\n  operationId: transactions_billing_transactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/plans\n  method: get\n  operationId: plans_billing_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/balance\n  method: get\n  operationId: account_balance_v1_account_balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/catalog\n  method: get\n  operationId: catalog_payments_catalog_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/packages\n  method: get\n  operationId: packages_payments_packages_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/orders\n  method: post\n  operationId: create_order_route_payments_orders_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/orders\n  method: get\n  operationId: list_orders_route_payments_orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/webhooks/{provider}\n  method: post\n  operationId: payment_webhook_payments_webhooks__provider__post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/subscription/cancel\n  method: post\n  operationId: cancel_subscription_route_payments_subscription_cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/subscription/resume\n  method: post\n  operationId: resume_subscription_route_payments_subscription_resume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/orders/{order_id}/resume\n  method: post\n  operationId: resume_order_route_payments_orders__order_id__resume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/orders/{order_id}/cancel\n  method: post\n  operationId: cancel_order_route_payments_orders__order_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/orders/{order_id}/confirm-paid\n  method: post\n  operationId: confirm_paid_route_payments_orders__order_id__confirm_paid_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/orders/{order_id}/confirm-failed\n  method: post\n  operationId: confirm_failed_route_payments_orders__order_id__confirm_failed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/orders/{order_id}\n  method: get\n  operationId: order_status_payments_orders__order_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/orders/{order_id}/events\n  method: get\n  operationId: order_events_stream_payments_orders__order_id__events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: usage_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/logs\n  method: get\n  operationId: usage_logs_usage_logs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/export\n  method: get\n  operationId: usage_export_usage_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback\n  method: post\n  operationId: create_feedback_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feedback\n  method: get\n  operationId: list_my_feedback_feedback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extract\n  method: post\n  operationId: extract_extract_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify\n  method: post\n  operationId: verify_claim_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/batch\n  method: post\n  operationId: verify_batch_verify_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extract\n  method: post\n  operationId: extract_v1_extract_post\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify\n  method: post\n  operationId: verify_claim_v1_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify/batch\n  method: post\n  operationId: verify_batch_v1_verify_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /messages\n  method: get\n  operationId: list_my_messages_messages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/unread-count\n  method: get\n  operationId: unread_count_messages_unread_count_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{message_id}/read\n  method: post\n  operationId: mark_message_read_messages__message_id__read_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/\n  method: get\n  operationId: admin_entry_admin__get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin\n  method: get\n  operationId: admin_entry_admin_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/login\n  method: get\n  operationId: admin_login_page_admin_login_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/login\n  method: post\n  operationId: admin_login_submit_admin_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/logout\n  method: get\n  operationId: admin_logout_admin_logout_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users\n  method: get\n  operationId: list_users_admin_users_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users/{user_id}\n  method: patch\n  operationId: update_user_admin_users__user_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/credits\n  method: get\n  operationId: credits_overview_admin_credits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/credits/grant\n\
  \  method: post\n  operationId: grant_credits_admin_admin_credits_grant_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/orders\n  method: get\n  operationId: list_orders_admin_orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/stats\n  method: get\n  operationId: stats_admin_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/feedback\n  method: get\n  operationId: list_feedback_admin_feedback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /admin/feedback/{ticket_id}/close\n  method: post\n  operationId: close_feedback_admin_feedback__ticket_id__close_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/messages\n  method: get\n  operationId: admin_messages_page_admin_messages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/messages\n  method: post\n  operationId: admin_send_message_admin_messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/monitor\n  method: get\n  operationId: monitor_page_admin_monitor_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/perf\n  method: get\n  operationId: perf_page_admin_perf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/behavior\n  method: get\n  operationId: behavior_page_admin_behavior_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/auth\n  method: get\n  operationId: auth_landing_dashboard_auth_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /dashboard/bonus-flash\n  method: get\n  operationId: bonus_flash_dashboard_bonus_flash_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/login\n  method: get\n  operationId: login_page_dashboard_login_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/login\n  method: post\n  operationId: login_submit_dashboard_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/register\n  method: get\n  operationId: register_page_dashboard_register_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/register\n  method: post\n  operationId: register_submit_dashboard_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/forgot-password\n  method: get\n  operationId: forgot_password_page_dashboard_forgot_password_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/forgot-password\n  method: post\n  operationId: forgot_password_submit_dashboard_forgot_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/reset-password\n  method: get\n  operationId: reset_password_page_dashboard_reset_password_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/reset-password\n  method: post\n  operationId: reset_password_submit_dashboard_reset_password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dashboard/resend-verification\n  method: post\n  operationId: resend_verification_dashboard_resend_verification_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dashboard/logout\n  method: get\n  operationId: logout_dashboard_logout_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/\n  method: get\n  operationId: dashboard_home_dashboard__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard\n  method: get\n  operationId: dashboard_home_dashboard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /dashboard/api-keys\n  method: get\n  operationId: dashboard_api_keys_dashboard_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/usage\n  method: get\n  operationId: dashboard_usage_dashboard_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/billing\n  method: get\n  operationId: dashboard_billing_dashboard_billing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/docs\n  method: get\n  operationId: dashboard_docs_dashboard_docs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/feedback\n  method:\
  \ get\n  operationId: dashboard_feedback_dashboard_feedback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/messages\n  method: get\n  operationId: dashboard_messages_dashboard_messages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: healthz_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-setup/SKILL.md\n  method: get\n  operationId: agent_setup_skill_agent_setup_SKILL_md_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: search_search_post\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: post\n  operationId: search_v1_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/searchpipe-tech/agentic-access/searchpipe-tech-agentic-access.yml
summary_line: 116 operations · 34 acting · 3 human-in-the-loop
tags:
- Web Search
- MCP
- AI Agents
- Search
---
