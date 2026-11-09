---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 14
api_specs:
- filename: acuris-geo-com-account-api-openapi.yml
  format: yaml
  label: acuris-geo-com Account API
  slug: acuris-geo-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuris-geo-com/openapi/acuris-geo-com-account-api-openapi.yml
- filename: acuris-geo-com-billing-api-openapi.yml
  format: yaml
  label: acuris-geo-com Billing API
  slug: acuris-geo-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuris-geo-com/openapi/acuris-geo-com-billing-api-openapi.yml
- filename: acuris-geo-com-config-api-openapi.yml
  format: yaml
  label: acuris-geo-com Config API
  slug: acuris-geo-com-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuris-geo-com/openapi/acuris-geo-com-config-api-openapi.yml
- filename: acuris-geo-com-geocoding-api-openapi.yml
  format: yaml
  label: acuris-geo-com Geocoding API
  slug: acuris-geo-com-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuris-geo-com/openapi/acuris-geo-com-geocoding-api-openapi.yml
- filename: acuris-geo-com-postcode-lookup-api-openapi.yml
  format: yaml
  label: acuris-geo-com Postcode lookup API
  slug: acuris-geo-com-postcode-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuris-geo-com/openapi/acuris-geo-com-postcode-lookup-api-openapi.yml
- filename: acuris-geo-com-suggest-api-openapi.yml
  format: yaml
  label: acuris-geo-com Suggest API
  slug: acuris-geo-com-suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuris-geo-com/openapi/acuris-geo-com-suggest-api-openapi.yml
- filename: acuris-geo-com-validation-api-openapi.yml
  format: yaml
  label: acuris-geo-com Validation API
  slug: acuris-geo-com-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuris-geo-com/openapi/acuris-geo-com-validation-api-openapi.yml
- filename: acuris-geo-com-versioned-aliases-v1-api-openapi.yml
  format: yaml
  label: acuris-geo-com Versioned aliases (v1) API
  slug: acuris-geo-com-versioned-aliases-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acuris-geo-com/openapi/acuris-geo-com-versioned-aliases-v1-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Acuris Geo Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stripe/create-checkout-session
operation_count: 23
overview: 'acuris-geo-com exposes 23 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: acuris-geo-com
provider_slug: acuris-geo-com
slug: acuris-geo-com-agentic-access
source_filename: acuris-geo-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/acuris-geo-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 9\n    connected: 14\n  by_consequence:\n    write: 8\n    read: 14\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /validate\n  method: post\n  operationId: validateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate-credits\n  method: get\n  operationId: validateCredits\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocode\n  method: get\n  operationId: geocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocode-usa\n  method: get\n  operationId: geocodeUsa\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse\n  method: get\n  operationId: reverseGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocode-credits\n  method: get\n  operationId: geocodeCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check-key\n  method: get\n  operationId:\
  \ checkKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suggest\n  method: get\n  operationId: suggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /widget/token\n  method: get\n  operationId: widgetToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/country-config\n  method: get\n  operationId: countryConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stripe/create-checkout-session\n  method: post\n  operationId: stripeCreateCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postcode-lookup\n  method: post\n  operationId: postcodeLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validate\n  method: post\n  operationId: validateAddressV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/validate/batch\n  method: post\n  operationId: validateAddressBatchV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/geocode\n  method: post\n  operationId: geocodeV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reverse\n  method: post\n  operationId: reverseGeocodeV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geocode-uk\n  method: get\n  operationId: geocodeUk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /validate/batch\n  method: post\n  operationId: validateAddressBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate/jobs\n  method: post\n  operationId: validateAddressCreateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate/jobs/{job_id}\n  method: get\n  operationId: validateAddressGetJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /account/balances\n  method: get\n  operationId: accountBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/usage\n  method: get\n  operationId: meUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dev-key\n  method: post\n  operationId: devKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/acuris-geo-com/agentic-access/acuris-geo-com-agentic-access.yml
summary_line: 23 operations · 9 acting
tags:
- Company
- Geocoding
- Address Validation
- Location Data
---
