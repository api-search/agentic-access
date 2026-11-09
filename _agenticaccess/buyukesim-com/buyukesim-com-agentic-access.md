---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: buyukesim-com-bundle-crypto-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Bundle Crypto Quote.php API
  slug: buyukesim-com-bundle-crypto-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-bundle-crypto-quote-php-api-openapi.yml
- filename: buyukesim-com-crypto-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Crypto Quote.php API
  slug: buyukesim-com-crypto-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-crypto-quote-php-api-openapi.yml
- filename: buyukesim-com-payment-methods-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Payment Methods.php API
  slug: buyukesim-com-payment-methods-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-payment-methods-php-api-openapi.yml
- filename: buyukesim-com-reviews-list-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Reviews List.php API
  slug: buyukesim-com-reviews-list-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-reviews-list-php-api-openapi.yml
- filename: buyukesim-com-topup-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Topup Quote.php API
  slug: buyukesim-com-topup-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-topup-quote-php-api-openapi.yml
- filename: buyukesim-com-travel-crypto-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Travel Crypto Quote.php API
  slug: buyukesim-com-travel-crypto-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-travel-crypto-quote-php-api-openapi.yml
- filename: buyukesim-com-travel-packages-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Travel Packages.php API
  slug: buyukesim-com-travel-packages-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-travel-packages-php-api-openapi.yml
- filename: buyukesim-com-vpn-crypto-quote-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Vpn Crypto Quote.php API
  slug: buyukesim-com-vpn-crypto-quote-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-vpn-crypto-quote-php-api-openapi.yml
- filename: buyukesim-com-vpn-plans-php-api-openapi.yml
  format: yaml
  label: BuyUKeSIM Vpn Plans.php API
  slug: buyukesim-com-vpn-plans-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyukesim-com/openapi/buyukesim-com-vpn-plans-php-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Buyukesim Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'BuyUKeSIM exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BuyUKeSIM
provider_slug: buyukesim-com
slug: buyukesim-com-agentic-access
source_filename: buyukesim-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/buyukesim-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /payment_methods.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crypto_quote.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topup_quote.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travel_packages.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /travel_crypto_quote.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundle_crypto_quote.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews_list.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vpn_plans.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /vpn_crypto_quote.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/buyukesim-com/agentic-access/buyukesim-com-agentic-access.yml
summary_line: 9 operations
tags:
- eSIM
- Cryptocurrency
- Privacy
- Telecommunications
- Travel
---
