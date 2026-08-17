---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: trustradius-product-data-api-openapi.yml
  format: yaml
  label: TrustRadius Product Data API
  slug: trustradius-product-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-product-data-api-openapi.yml
- filename: trustradius-intent-data-api-openapi.yml
  format: yaml
  label: TrustRadius Downstream Intent Data API
  slug: trustradius-intent-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-intent-data-api-openapi.yml
- filename: trustradius-trustquotes-api-openapi.yml
  format: yaml
  label: TrustRadius TrustQuotes Content Syndication API
  slug: trustradius-trustquotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-trustquotes-api-openapi.yml
- filename: trustradius-traffic-data-api-openapi.yml
  format: yaml
  label: TrustRadius Traffic Data API
  slug: trustradius-traffic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-traffic-data-api-openapi.yml
- filename: trustradius-legacy-api-openapi.yml
  format: yaml
  label: TrustRadius Legacy Visitor Insights API
  slug: trustradius-legacy-visitor-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-legacy-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trustradius Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'TrustRadius exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TrustRadius
provider_slug: trustradius
slug: trustradius-agentic-access
source_filename: trustradius-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/trustradius-intent-data-api-openapi.yml, openapi/trustradius-legacy-api-openapi.yml,\n  openapi/trustradius-product-data-api-openapi.yml, openapi/trustradius-traffic-data-api-openapi.yml,\n  openapi/trustradius-trustquotes-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /intent\n  method: get\n  operationId: intent_data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/visitor-insights/companies\n  method: get\n  operationId: visitor_insights_report\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/visitor-insights/pages\n  method: get\n  operationId: visitor_insights_report_pages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}\n  method: get\n  operationId: account_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product-ids\n  method: get\n  operationId: product_ids_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product-scores\n  method: get\n  operationId: product_scores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/traffic/pages\n  method: get\n  operationId: get_traffic_page_types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/traffic/products\n  method: get\n  operationId: get_traffic_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/syndication/tqw/pages\n  method: get\n  operationId: tqw_pages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trustquotes\n  method: get\n  operationId: trustquotes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags\n  method: get\n  operationId:\
  \ tags_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/agentic-access/trustradius-agentic-access.yml
summary_line: 11 operations
tags:
- B2B Software Reviews
- Buyer Intelligence
- Intent Data
- Software Reviews
- Reviews
- Product Reviews
- Content Syndication
- Account Based Marketing
- Marketing
- Analytics
---
