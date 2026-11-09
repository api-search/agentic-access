---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 19
api_specs:
- filename: kokofinance-net-billing-api-openapi.yml
  format: yaml
  label: kokofinance-net Billing API
  slug: kokofinance-net-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-billing-api-openapi.yml
- filename: kokofinance-net-cards-api-openapi.yml
  format: yaml
  label: kokofinance-net Cards API
  slug: kokofinance-net-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-cards-api-openapi.yml
- filename: kokofinance-net-developers-api-openapi.yml
  format: yaml
  label: kokofinance-net Developers API
  slug: kokofinance-net-developers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-developers-api-openapi.yml
- filename: kokofinance-net-intelligence-api-openapi.yml
  format: yaml
  label: kokofinance-net Intelligence API
  slug: kokofinance-net-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-intelligence-api-openapi.yml
- filename: kokofinance-net-international-api-openapi.yml
  format: yaml
  label: kokofinance-net International API
  slug: kokofinance-net-international-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-international-api-openapi.yml
- filename: kokofinance-net-platform-api-openapi.yml
  format: yaml
  label: kokofinance-net Platform API
  slug: kokofinance-net-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-platform-api-openapi.yml
- filename: kokofinance-net-portfolio-api-openapi.yml
  format: yaml
  label: kokofinance-net Portfolio API
  slug: kokofinance-net-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-portfolio-api-openapi.yml
- filename: kokofinance-net-reference-api-openapi.yml
  format: yaml
  label: kokofinance-net Reference API
  slug: kokofinance-net-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kokofinance-net/openapi/kokofinance-net-reference-api-openapi.yml
consequence_counts:
  read: 19
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kokofinance Net Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 39
overview: 'kokofinance-net exposes 39 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: kokofinance-net
provider_slug: kokofinance-net
slug: kokofinance-net-agentic-access
source_filename: kokofinance-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/kokofinance-net-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 19\n    acting: 20\n  by_consequence:\n    read: 19\n    write: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/cards/\n  method: get\n  operationId: list_cards_api_v1_cards__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cards/changes\n  method: get\n  operationId: get_all_changes_api_v1_cards_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/cards/{card_id}\n  method: get\n  operationId: get_card_detail_api_v1_cards__card_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cards/{card_id}/terms\n  method: get\n  operationId: get_card_terms_api_v1_cards__card_id__terms_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cards/{card_id}/history\n  method: get\n  operationId: get_card_history_api_v1_cards__card_id__history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cards/search\n  method: post\n  operationId: search_cards_api_v1_cards_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{country}/cards/\n  method: get\n  operationId: market_list_cards_api_v1__country__cards__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{country}/cards/{card_id}\n  method: get\n  operationId: market_get_card_detail_api_v1__country__cards__card_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{country}/cards/search\n  method: post\n  operationId: market_search_cards_api_v1__country__cards_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/{country}/cards/compare\n  method: post\n  operationId: market_compare_cards_api_v1__country__cards_compare_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/intelligence/compare\n  method: post\n  operationId: compare_cards_api_v1_intelligence_compare_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/intelligence/recommend\n  method: post\n  operationId: recommend_cards_api_v1_intelligence_recommend_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/intelligence/value\n  method: post\n  operationId: calculate_card_value_api_v1_intelligence_value_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/intelligence/renewal\n  method: post\n  operationId: renewal_check_api_v1_intelligence_renewal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/intelligence/merchant/best-card\n\
  \  method: post\n  operationId: merchant_best_card_api_v1_intelligence_merchant_best_card_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/intelligence/merchant/benefits\n  method: post\n  operationId: merchant_benefits_api_v1_intelligence_merchant_benefits_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/portfolio/analyze\n  method: post\n  operationId: v1_analyze_portfolio_api_v1_portfolio_analyze_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/portfolio/points-playbook\n  method: post\n  operationId: v1_points_playbook_api_v1_portfolio_points_playbook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/portfolio/points/balances\n  method: get\n  operationId: get_balances_api_v1_portfolio_points_balances_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/portfolio/points/balances\n  method: post\n  operationId: save_balances_api_v1_portfolio_points_balances_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/portfolio/points/balances/{program_key}\n  method: delete\n  operationId: delete_balance_api_v1_portfolio_points_balances__program_key__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/portfolio/points/summary\n  method: get\n  operationId: get_summary_api_v1_portfolio_points_summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reference/programs\n  method:\
  \ get\n  operationId: list_programs_api_v1_reference_programs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reference/programs/{program_key}\n  method: get\n  operationId: get_program_api_v1_reference_programs__program_key__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reference/programs/{program_key}/history\n  method: get\n  operationId: get_program_history_api_v1_reference_programs__program_key__history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reference/benefit-categories\n  method: get\n  operationId: v1_benefit_categories_api_v1_reference_benefit_categories_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/platform/health\n  method: get\n  operationId: v1_health_api_v1_platform_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/platform/status\n  method: get\n  operationId: v1_status_api_v1_platform_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/platform/usage\n  method: get\n  operationId: get_usage_api_v1_platform_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/platform/billing/portal\n  method: post\n  operationId: create_portal_session_api_v1_platform_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/platform/developers/dashboard\n  method: get\n  operationId: get_dashboard_api_v1_platform_developers_dashboard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/platform/developers/setup\n  method: post\n  operationId: developer_setup_api_v1_platform_developers_setup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/platform/developers/keys\n  method: post\n  operationId: create_key_api_v1_platform_developers_keys_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/platform/developers/keys/{key_prefix}/rotate\n  method: post\n  operationId: rotate_key_api_v1_platform_developers_keys__key_prefix__rotate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/platform/developers/keys/{key_prefix}/deactivate\n  method: post\n  operationId: deactivate_key_api_v1_platform_developers_keys__key_prefix__deactivate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/platform/developers/organization\n  method: put\n  operationId: update_organization_api_v1_platform_developers_organization_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/platform/developers/billing/setup-intent\n  method: post\n  operationId: developer_setup_intent_api_v1_platform_developers_billing_setup_intent_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/platform/developers/billing/portal\n  method: post\n  operationId: developer_portal_api_v1_platform_developers_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/platform/developers/usage-history\n  method: get\n  operationId: get_usage_history_api_v1_platform_developers_usage_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/kokofinance-net/agentic-access/kokofinance-net-agentic-access.yml
summary_line: 39 operations · 20 acting
tags:
- Company
- Fintech
- Credit Cards
- MCP
---
