---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 52
api_specs:
- filename: twentyci-address-match-api-openapi.yml
  format: yaml
  label: TwentyCi Address Match API
  slug: twentyci-address-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-address-match-api-openapi.yml
- filename: twentyci-agent-performance-api-openapi.yml
  format: yaml
  label: TwentyCi Agent Performance API
  slug: twentyci-agent-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-agent-performance-api-openapi.yml
- filename: twentyci-authorisation-api-openapi.yml
  format: yaml
  label: TwentyCi Authorisation API
  slug: twentyci-authorisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-authorisation-api-openapi.yml
- filename: twentyci-categories-api-openapi.yml
  format: yaml
  label: TwentyCi Categories API
  slug: twentyci-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-categories-api-openapi.yml
- filename: twentyci-properties-api-openapi.yml
  format: yaml
  label: TwentyCi Properties API
  slug: twentyci-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-properties-api-openapi.yml
- filename: twentyci-schools-api-openapi.yml
  format: yaml
  label: TwentyCi Schools API
  slug: twentyci-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-schools-api-openapi.yml
- filename: twentyci-this-is-now-retail-propensity-to-buy-goods-api-openapi.yml
  format: yaml
  label: TwentyCi This is Now | Retail Propensity To Buy Goods API
  slug: twentyci-this-is-now-retail-propensity-to-buy-goods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-this-is-now-retail-propensity-to-buy-goods-api-openapi.yml
- filename: twentyci-trigger-information-api-openapi.yml
  format: yaml
  label: TwentyCi Trigger Information API
  slug: twentyci-trigger-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-trigger-information-api-openapi.yml
- filename: twentyci-uk-housing-market-metrics-api-openapi.yml
  format: yaml
  label: TwentyCi UK Housing Market Metrics API
  slug: twentyci-uk-housing-market-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-uk-housing-market-metrics-api-openapi.yml
consequence_counts:
  read: 52
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Twentyci Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 58
overview: 'TwentyCi exposes 58 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 52 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TwentyCi
provider_slug: twentyci
slug: twentyci-agentic-access
source_filename: twentyci-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/twentyci-twentyapi-oauth-openapi.json, openapi/twentyci-twentyapi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 58\n  by_action_class:\n    acting: 6\n    connected: 52\n  by_consequence:\n    write: 6\n    read: 52\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: issueTwentyApiToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories\n  method: get\n  operationId: obtain_a_list_of_categories_for_a_property\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{category}\n  method: get\n  operationId: obtain_a_specific_category_for_a_property\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{uprn}\n  method: get\n  operationId: property_information_by_uprn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property}/details\n  method: get\n  operationId: property_details_by_uprn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property}/recent-sale-in-the-area\n  method: get\n  operationId: recent_property_sales_in_the_area\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property}/for-sale-in-the-area\n  method: get\n  operationId: similar_properties_for_sale_in_area\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/area-value-price\n  method: post\n  operationId: average_property_values_by_postcode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /propertiesavm2/{property}\n  method: post\n  operationId: valuation_of_property_by_uprn_avm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/area-search\n  method: post\n  operationId: searching_properties_by_postcode_and_radius\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/postcode-search\n  method: post\n  operationId: searching_properties_by_postcode_and_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/{property}/category/_all\n  method: get\n  operationId:\
  \ property_attributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property}/image\n  method: get\n  operationId: obtaining_a_google_maps_url_for_a_property\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property}/transactions\n  method: get\n  operationId: obtain_all_transactions_for_property_via_uprn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property}/transport-links\n  method: get\n  operationId: obtain_transport_links_near_a_property\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{uprn}/plannings\n  method:\
  \ get\n  operationId: obtain_planning_permission_data_near_a_property\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{uprn}/likely-to-sell\n  method: get\n  operationId: likely_to_sell\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price-per-square/comparables\n  method: get\n  operationId: comparables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trigger-type/{typeId}/properties\n  method: get\n  operationId: get_properties_by_trigger_type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trigger-type/{typeId}/no-uprn-properties\n  method: get\n  operationId:\
  \ get_no_uprn_properties_by_trigger_type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{property}/triggers\n  method: get\n  operationId: trigger_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/best\n  method: get\n  operationId: list_of_best_agents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/rankings/sstc\n  method: get\n  operationId: brands_ranked_by_sstc_s\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/rankings/new-instructions\n  method: get\n  operationId: brands_ranked_by_new_instructions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/rankings/percentage-of-initial-price-achieved\n  method: get\n  operationId: brands_ranked_by_pipa\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/rankings/days-to-sstc\n  method: get\n  operationId: brands_ranked_by_days_from_new_instruction_to_sstc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/new-instructions\n  method: get\n  operationId: new_instructions_statistics_for_a_brand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/sstc\n\
  \  method: get\n  operationId: sstc_statistics_for_a_brand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/time-to-sell\n  method: get\n  operationId: days_to_sstc_for_a_specific_brand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/time-to-sell-all-brands\n  method: get\n  operationId: days_to_sstc_for_all_brands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/property-sale-difference\n  method: get\n  operationId: difference_in_sold_price_for_a_property_for_a_specific_brand_and_all_other_brands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/percentage-of-initial-price-achieved\n  method: get\n  operationId: difference_in_pipa_for_a_property_for_a_specific_brand_and_all_other_brands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/property-sale-value\n  method: get\n  operationId: average_listing_price_for_a_brand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/sold-percentage\n  method: get\n  operationId: properties_sales_ratio_for_a_given_brand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/sold-percentage-all-brands\n  method: get\n  operationId: properties_sales_ratio_for_all_brands\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/days-to-sstc\n  method: get\n  operationId: days_to_sstc_for_a_given_brand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentals/agent-performance/rankings/let-agreed\n  method: get\n  operationId: brands_ranked_by_let_agreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentals/agent-performance/rankings/new-instructions\n  method: get\n  operationId: brands_ranked_by_new_instructions_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentals/agent-performance/brand/let-agreed\n  method:\
  \ get\n  operationId: let_agreed_statistics_for_a_brand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentals/agent-performance/brand/new-instructions\n  method: get\n  operationId: new_instructions_statistics_for_a_brand_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentals/agent-performance/brand/let-percentage\n  method: get\n  operationId: properties_let_ratio_for_a_given_brand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /match-address-processes\n  method: post\n  operationId: address_match\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nearby-places/schools\n  method: get\n  operationId: schools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/initial-metrics\n  method: get\n  operationId: uk_housing_market_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /this-is-now/search\n  method: get\n  operationId: local_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties\n  method: get\n  operationId: get_properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /properties/{property}/category/{category}\n  method: get\n  operationId: get_properties_property_category_category\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/{uprn}/floor-plans\n  method: get\n  operationId: get_properties_uprn_floor_plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trigger/{trigger}\n  method: get\n  operationId: get_trigger_trigger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/rankings/exchange\n  method: get\n  operationId: get_agent_performance_rankings_exchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /agent-performance/brand/exchange\n  method: get\n  operationId: get_agent_performance_brand_exchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/property-sale-value-all-brands\n  method: get\n  operationId: get_agent_performance_brand_property_sale_value_all_brands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/initial-price-achieve\n  method: get\n  operationId: get_agent_performance_brand_initial_price_achieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-performance/brand/property-listing-value\n  method: get\n  operationId: get_agent_performance_brand_property_listing_value\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentals/agent-performance/brand/time-to-let\n  method: get\n  operationId: get_rentals_agent_performance_brand_time_to_let\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentals/agent-performance/brand/time-to-let-all-brands\n  method: get\n  operationId: get_rentals_agent_performance_brand_time_to_let_all_brands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rentals/agent-performance/brand/let-percentage-all-brands\n  method: get\n  operationId: get_rentals_agent_performance_brand_let_percentage_all_brands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /this-is-now/search-national\n  method: get\n  operationId: get_this_is_now_search_national\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/agentic-access/twentyci-agentic-access.yml
summary_line: 58 operations · 6 acting
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Valuation
- AVM
- Rentals
- Address Data
- Conveyancing
- Homemover Data
- Agent Performance
- Data as a Service
---
