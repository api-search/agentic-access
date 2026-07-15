---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 16
api_specs:
- filename: smarty-us-street-address-api-openapi.yml
  format: yaml
  label: US Street Address API
  slug: us-street-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-street-address-api-openapi.yml
- filename: smarty-us-autocomplete-pro-api-openapi.yml
  format: yaml
  label: US Autocomplete Pro API
  slug: us-autocomplete-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-autocomplete-pro-api-openapi.yml
- filename: smarty-us-zipcode-api-openapi.yml
  format: yaml
  label: US ZIP Code API
  slug: us-zipcode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-zipcode-api-openapi.yml
- filename: smarty-us-reverse-geocode-api-openapi.yml
  format: yaml
  label: US Reverse Geocode API
  slug: us-reverse-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-reverse-geocode-api-openapi.yml
- filename: smarty-us-address-enrichment-api-openapi.yml
  format: yaml
  label: US Address Enrichment API
  slug: us-address-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-address-enrichment-api-openapi.yml
- filename: smarty-us-extract-api-openapi.yml
  format: yaml
  label: US Extract API
  slug: us-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-extract-api-openapi.yml
- filename: smarty-international-street-address-api-openapi.yml
  format: yaml
  label: International Street Address API
  slug: international-street-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-international-street-address-api-openapi.yml
- filename: smarty-international-address-autocomplete-api-openapi.yml
  format: yaml
  label: International Address Autocomplete API
  slug: international-address-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-international-address-autocomplete-api-openapi.yml
- filename: smarty-international-postal-code-api-openapi.yml
  format: yaml
  label: International Postal Code API
  slug: international-postal-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-international-postal-code-api-openapi.yml
consequence_counts:
  read: 16
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smarty Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Smarty exposes 19 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Smarty
provider_slug: smarty
slug: smarty-agentic-access
source_filename: smarty-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smarty-international-address-autocomplete-api-openapi.yml, openapi/smarty-international-postal-code-api-openapi.yml,\n  openapi/smarty-international-street-address-api-openapi.yml, openapi/smarty-us-address-enrichment-api-openapi.yml,\n  openapi/smarty-us-autocomplete-pro-api-openapi.yml, openapi/smarty-us-extract-api-openapi.yml,\n  openapi/smarty-us-reverse-geocode-api-openapi.yml, openapi/smarty-us-street-address-api-openapi.yml,\n  openapi/smarty-us-zipcode-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 16\n    acting: 3\n  by_consequence:\n    read: 16\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/lookup\n\
  \  method: get\n  operationId: get-lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/lookup/{addressId}\n  method: get\n  operationId: get-lookup-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup\n  method: get\n  operationId: lookup-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify\n  method: get\n  operationId: get-verify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/{smartykey}/property\n  method: get\n  operationId: get-lookup-smartykey-property\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/search/property\n  method: get\n  operationId: get-lookup-property\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/{smarykey}/geo-reference/{dataset?}\n  method: get\n  operationId: get-lookup-smartykey-geo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/search/geo-reference/{dataset?}\n  method: get\n  operationId: get-lookup-geo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/{smartykey}/secondary\n  method: get\n  operationId: get-lookup-smartykey-secondary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /lookup/search/secondary\n  method: get\n  operationId: get-lookup-secondary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/{smartykey}/secondary/count\n  method: get\n  operationId: get-lookup-smartykey-secondary-count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/search/secondary/count\n  method: get\n  operationId: get-lookup-secondary-count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup\n  method: get\n  operationId: get-lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n\
  \  operationId: post-extract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lookup\n  method: get\n  operationId: get-street-address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /street-address\n  method: get\n  operationId: get-street-address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /street-address\n  method: post\n  operationId: post-street-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lookup\n  method: get\n  operationId: lookup-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup\n  method: post\n  operationId: lookup-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/agentic-access/smarty-agentic-access.yml
summary_line: 19 operations · 3 acting
tags:
- Address Verification
- Geocoding
- Address Autocomplete
- ZIP Code
- Address Intelligence
- Location Data
- International Address
- US Address
---
