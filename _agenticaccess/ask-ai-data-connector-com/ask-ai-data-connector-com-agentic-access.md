---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 29
api_specs:
- filename: ask-ai-data-connector-com-gpt-api-openapi.yml
  format: yaml
  label: Ask AI Gpt API
  slug: ask-ai-data-connector-com-gpt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ask-ai-data-connector-com/openapi/ask-ai-data-connector-com-gpt-api-openapi.yml
consequence_counts:
  read: 29
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ask Ai Data Connector Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Ask AI exposes 30 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ask AI
provider_slug: ask-ai-data-connector-com
slug: ask-ai-data-connector-com-agentic-access
source_filename: ask-ai-data-connector-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/ask-ai-data-connector-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 1\n    connected: 29\n  by_consequence:\n    write: 1\n    read: 29\n  human_in_the_loop_required: 0\noperations:\n- path: /api/gpt/ask_question\n  method: post\n  operationId: askQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/gpt/get_data_sources\n  method: post\n  operationId: getDataSources\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_complete_dashboard\n  method: post\n  operationId: getCompleteDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_metrics_comparison\n  method: post\n  operationId: getMetricsComparison\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_customer_insights\n  method: post\n  operationId: getCustomerInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_refunds\n  method: post\n  operationId: getRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_discounts\n  method: post\n  operationId: getDiscounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_inventory_velocity\n  method: post\n  operationId: getInventoryVelocity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_marketing_performance\n  method: post\n  operationId: getMarketingPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_store_summary\n  method: post\n  operationId: getStoreSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/gpt/query_orders\n  method: post\n  operationId: queryOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_orders\n  method: post\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_top_products\n  method: post\n  operationId: getTopProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_customers\n  method: post\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_inventory\n  method: post\n  operationId: getInventory\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_daily_revenue\n  method: post\n  operationId: getDailyRevenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_weekly_trends\n  method: post\n  operationId: getWeeklyTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_triple_whale\n  method: post\n  operationId: getTripleWhale\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_klaviyo\n  method: post\n  operationId: getKlaviyo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/gpt/get_gorgias\n  method: post\n  operationId: getGorgias\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_recharge\n  method: post\n  operationId: getRecharge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_search_console\n  method: post\n  operationId: getSearchConsole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_clarity\n  method: post\n  operationId: getClarity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_youtube\n  method: post\n  operationId: getYoutube\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_reviews\n  method: post\n  operationId: getReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_loyalty\n  method: post\n  operationId: getLoyalty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_wishlist\n  method: post\n  operationId: getWishlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_daily_stats\n  method: post\n  operationId: getDailyStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/gpt/get_abandoned_checkouts\n  method: post\n  operationId: getAbandonedCheckouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpt/get_analytics\n  method: post\n  operationId: getAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ask-ai-data-connector-com/agentic-access/ask-ai-data-connector-com-agentic-access.yml
summary_line: 30 operations · 1 acting
tags:
- Artificial Intelligence
- Analytics
- E-Commerce
- Shopify
- No-Code
---
