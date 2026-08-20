---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: cj-affiliate.postman_collection.json
  format: json
  label: CJ Commission Detail API
  slug: cj-affiliate-commission-detail-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/collections/cj-affiliate.postman_collection.json
- filename: cj-affiliate-ads-asyncapi.yml
  format: yaml
  label: CJ Product Search API
  slug: cj-affiliate-product-search-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/asyncapi/cj-affiliate-ads-asyncapi.yml
- filename: cj-affiliate-advertiser-lookup-api-openapi.yml
  format: yaml
  label: CJ Affiliate Advertiser Lookup API
  slug: cj-affiliate-advertiser-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-advertiser-lookup-api-openapi.yml
- filename: cj-affiliate-link-search-api-openapi.yml
  format: yaml
  label: CJ Affiliate Link Search API
  slug: cj-affiliate-link-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-link-search-api-openapi.yml
- filename: cj-affiliate-publisher-lookup-api-openapi.yml
  format: yaml
  label: CJ Affiliate Publisher Lookup API
  slug: cj-affiliate-publisher-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-publisher-lookup-api-openapi.yml
- filename: cj-affiliate-click-events-api-openapi.yml
  format: yaml
  label: CJ Affiliate Click Events API
  slug: cj-affiliate-click-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-click-events-api-openapi.yml
- filename: cj-affiliate-publisher-tracking-api-openapi.yml
  format: yaml
  label: CJ Affiliate Publisher Tracking API
  slug: cj-affiliate-publisher-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-publisher-tracking-api-openapi.yml
- filename: cj-affiliate-commission-detail-legacy-api-openapi.yml
  format: yaml
  label: CJ Affiliate Commission Detail API (Legacy)
  slug: cj-affiliate-commission-detail-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/openapi/cj-affiliate-commission-detail-legacy-api-openapi.yml
consequence_counts:
  destructive: 1
  financial-write: 3
  read: 14
  write: 6
description: 'Recommended x-agentic-access execution contracts for CJ Affiliate, classified from the real operation set. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Note the shape of the risk here: every write on this platform moves money or changes attribution. The Tracking API mutations create and correct commissionable transactions, restateOrders is full-state replacement that DROPS anything omitted, and both click APIs register real consumer clicks that affect attribution and reporting. None of them is safe to call speculatively.'
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: derived
name: Cj Affiliate Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'CJ Affiliate exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 6 write.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CJ Affiliate
provider_slug: cj-affiliate
slug: cj-affiliate-agentic-access
source_filename: cj-affiliate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/_original/cj-affiliate-openapi.yml + graphql/cj-affiliate-*.graphql (live introspection\n  2026-08-13)\ndescription: 'Recommended x-agentic-access execution contracts for CJ Affiliate, classified from the real\n  operation set. A governance starting point for exposing this API to AI agents - review and bind audience\n  per deployment. Note the shape of the risk here: every write on this platform moves money or changes\n  attribution. The Tracking API mutations create and correct commissionable transactions, restateOrders\n  is full-state replacement that DROPS anything omitted, and both click APIs register real consumer clicks\n  that affect attribution and reporting. None of them is safe to call speculatively.'\nsummary:\n  operations: 24\n  rest_operations: 7\n  graphql_fields: 17\n  by_consequence:\n    read: 14\n    write: 6\n    destructive: 1\n    financial-write: 3\n  human_in_the_loop_required: 10\ntoken_note:\
  \ CJ issues one long-lived personal access token with no scopes and no programmatic issuance,\n  so least-privilege must be enforced by the agent gateway rather than by the credential.\nrest_operations:\n- path: /v2/link-search\n  method: get\n  operationId: linkSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/advertiser-lookup\n  method: get\n  operationId: advertiserLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/joined-publisher-lookup\n  method: get\n  operationId: publisherLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/commissions\n  method: get\n\
  \  operationId: commissionDetailLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/item-detail/{original-action-id}\n  method: get\n  operationId: commissionItemDetailLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/event\n  method: post\n  operationId: createClickEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /clickdestination\n  method: post\n  operationId: resolveClickDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: optional\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit:\
  \ required\ngraphql_fields:\n- endpoint: commissions.api.cj.com/query\n  field: publisherCommissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- endpoint: commissions.api.cj.com/query\n  field: advertiserCommissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- endpoint: ads.api.cj.com/query\n  field: products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- endpoint: ads.api.cj.com/query\n  field: shoppingProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- endpoint:\
  \ ads.api.cj.com/query\n  field: travelExperienceProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- endpoint: ads.api.cj.com/query\n  field: financeProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- endpoint: ads.api.cj.com/query\n  field: financeCreditCardProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- endpoint: ads.api.cj.com/query\n  field: shoppingProductFeeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- endpoint: ads.api.cj.com/query\n  field:\
  \ productFeeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    human-in-the-loop: false\n    token:\n      max-ttl: 3600\n    audit: none\n- endpoint: ads.api.cj.com/query\n  field: createShoppingProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit: required\n- endpoint: ads.api.cj.com/query\n  field: updateShoppingProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit: required\n- endpoint: ads.api.cj.com/query\n  field: deleteProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: destructive\n    subject: required\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit: required\n- endpoint: ads.api.cj.com/query\n  field: createCreditCardProducts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit: required\n- endpoint: ads.api.cj.com/query\n  field: updateCreditCardProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: write\n    subject: required\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit: required\n- endpoint: tracking.api.cj.com/graphql\n  field: createOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: financial-write\n    subject: required\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit: required\n- endpoint: tracking.api.cj.com/graphql\n  field: restateOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: financial-write\n    subject: required\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit: required\n- endpoint: tracking.api.cj.com/graphql\n  field: cancelOrders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: financial-write\n    subject: required\n    human-in-the-loop: true\n    token:\n      max-ttl: 3600\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cj-affiliate/refs/heads/main/agentic-access/cj-affiliate-agentic-access.yml
summary_line: 24 operations · 10 human-in-the-loop
tags:
- Affiliate Marketing
- Affiliate Network
- Commission
- Product Search
- Publishers
- Advertiser
- GraphQL
- E-Commerce
- Product Feeds
- Conversion Tracking
- Attribution
- Performance Marketing
- Retail
- Coupons
---
