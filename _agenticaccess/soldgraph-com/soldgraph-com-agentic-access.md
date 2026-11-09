---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 21
api_specs:
- filename: soldgraph-com-account-api-openapi.yml
  format: yaml
  label: soldgraph-com Account API
  slug: soldgraph-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-account-api-openapi.yml
- filename: soldgraph-com-batches-api-openapi.yml
  format: yaml
  label: soldgraph-com Batches API
  slug: soldgraph-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-batches-api-openapi.yml
- filename: soldgraph-com-depop-api-openapi.yml
  format: yaml
  label: soldgraph-com Depop API
  slug: soldgraph-com-depop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-depop-api-openapi.yml
- filename: soldgraph-com-ebay-api-openapi.yml
  format: yaml
  label: soldgraph-com eBay API
  slug: soldgraph-com-ebay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-ebay-api-openapi.yml
- filename: soldgraph-com-facebook-marketplace-api-openapi.yml
  format: yaml
  label: soldgraph-com Facebook Marketplace API
  slug: soldgraph-com-facebook-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-facebook-marketplace-api-openapi.yml
- filename: soldgraph-com-jobs-api-openapi.yml
  format: yaml
  label: soldgraph-com Jobs API
  slug: soldgraph-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-jobs-api-openapi.yml
- filename: soldgraph-com-mercari-api-openapi.yml
  format: yaml
  label: soldgraph-com Mercari API
  slug: soldgraph-com-mercari-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-mercari-api-openapi.yml
- filename: soldgraph-com-offerup-api-openapi.yml
  format: yaml
  label: soldgraph-com Offer Up API
  slug: soldgraph-com-offerup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-offerup-api-openapi.yml
- filename: soldgraph-com-poshmark-api-openapi.yml
  format: yaml
  label: soldgraph-com Poshmark API
  slug: soldgraph-com-poshmark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-poshmark-api-openapi.yml
- filename: soldgraph-com-tcgplayer-api-openapi.yml
  format: yaml
  label: soldgraph-com TC Gplayer API
  slug: soldgraph-com-tcgplayer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-tcgplayer-api-openapi.yml
- filename: soldgraph-com-vinted-api-openapi.yml
  format: yaml
  label: soldgraph-com Vinted API
  slug: soldgraph-com-vinted-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-vinted-api-openapi.yml
- filename: soldgraph-com-whatnot-api-openapi.yml
  format: yaml
  label: soldgraph-com Whatnot API
  slug: soldgraph-com-whatnot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soldgraph-com/openapi/soldgraph-com-whatnot-api-openapi.yml
consequence_counts:
  read: 21
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Soldgraph Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'soldgraph-com exposes 22 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: soldgraph-com
provider_slug: soldgraph-com
slug: soldgraph-com-agentic-access
source_filename: soldgraph-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/soldgraph-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 21\n    acting: 1\n  by_consequence:\n    read: 21\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /ebay/sold\n  method: get\n  operationId: ebay_sold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ebay/listings\n  method: get\n  operationId: ebay_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /poshmark/sold\n  method: get\n  operationId:\
  \ poshmark_sold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /poshmark/listings\n  method: get\n  operationId: poshmark_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mercari/sold\n  method: get\n  operationId: mercari_sold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mercari/listings\n  method: get\n  operationId: mercari_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /depop/listings\n  method: get\n  operationId: depop_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /whatnot/listings\n  method: get\n  operationId: whatnot_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcgplayer/search\n  method: get\n  operationId: tcgplayer_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcgplayer/sales\n  method: get\n  operationId: tcgplayer_sales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offerup/listings\n  method: get\n  operationId: offerup_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offerup/item\n  method: get\n  operationId: offerup_item\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/listings\n  method: get\n  operationId: facebook_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /facebook/item\n  method: get\n  operationId: facebook_item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vinted/listings\n  method: get\n  operationId: vinted_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vinted/item\n  method: get\n  operationId: vinted_item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /sold\n  method: get\n  operationId: legacy_sold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings\n  method: get\n  operationId: legacy_listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}\n  method: get\n  operationId: get_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: get_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches\n  method: post\n  operationId: create_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batches/{id}\n  method: get\n  operationId: get_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/soldgraph-com/agentic-access/soldgraph-com-agentic-access.yml
summary_line: 22 operations · 1 acting
tags:
- Company
- Resale
- Marketplace
- Pricing
- Data
---
