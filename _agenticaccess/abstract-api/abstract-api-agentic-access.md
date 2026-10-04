---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 16
api_specs:
- filename: abstract-api-vat-validation-api-openapi.yml
  format: yaml
  label: Abstract API VAT Validation API
  slug: abstract-api-vat-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-vat-validation-api-openapi.yml
- filename: abstract-api-abstract-avatars-api-api-openapi.yml
  format: yaml
  label: Abstract API Abstract Avatars API
  slug: abstract-api-abstract-avatars-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-abstract-avatars-api-api-openapi.yml
- filename: abstract-api-calculate-api-openapi.yml
  format: yaml
  label: Abstract API Calculate API
  slug: abstract-api-calculate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-calculate-api-openapi.yml
- filename: abstract-api-categories-api-openapi.yml
  format: yaml
  label: Abstract API Categories API
  slug: abstract-api-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-categories-api-openapi.yml
- filename: abstract-api-convert-api-openapi.yml
  format: yaml
  label: Abstract API Convert API
  slug: abstract-api-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-convert-api-openapi.yml
- filename: abstract-api-convert-time-api-openapi.yml
  format: yaml
  label: Abstract API Convert Time API
  slug: abstract-api-convert-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-convert-time-api-openapi.yml
- filename: abstract-api-current-time-api-openapi.yml
  format: yaml
  label: Abstract API Current Time API
  slug: abstract-api-current-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-current-time-api-openapi.yml
- filename: abstract-api-historical-api-openapi.yml
  format: yaml
  label: Abstract API Historical API
  slug: abstract-api-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-historical-api-openapi.yml
- filename: abstract-api-live-api-openapi.yml
  format: yaml
  label: Abstract API Live API
  slug: abstract-api-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-live-api-openapi.yml
- filename: abstract-api-upload-api-openapi.yml
  format: yaml
  label: Abstract API Upload API
  slug: abstract-api-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-upload-api-openapi.yml
- filename: abstract-api-url-api-openapi.yml
  format: yaml
  label: Abstract API URL API
  slug: abstract-api-url-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-url-api-openapi.yml
- filename: abstract-api-validate-api-openapi.yml
  format: yaml
  label: Abstract API Validate API
  slug: abstract-api-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-validate-api-openapi.yml
consequence_counts:
  read: 16
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Abstract Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Abstract API exposes 25 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Abstract API
provider_slug: abstract-api
slug: abstract-api-agentic-access
source_filename: abstract-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/abstract-api-abstract-avatars-api-api-openapi.yml, openapi/abstract-api-calculate-api-openapi.yml,\n  openapi/abstract-api-categories-api-openapi.yml, openapi/abstract-api-convert-api-openapi.yml,\n  openapi/abstract-api-convert-time-api-openapi.yml, openapi/abstract-api-current-time-api-openapi.yml,\n  openapi/abstract-api-historical-api-openapi.yml, openapi/abstract-api-live-api-openapi.yml,\n  openapi/abstract-api-upload-api-openapi.yml, openapi/abstract-api-url-api-openapi.yml, openapi/abstract-api-validate-api-openapi.yml,\n  openapi/abstract-api-vat-validation-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 16\n    acting:\
  \ 9\n  by_consequence:\n    read: 16\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getAvatar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: postAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calculate\n  method: get\n  operationId: getCalculateVat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calculate\n  method: post\n  operationId: postCalculateVat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories\n  method: get\n  operationId: getVatCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: post\n  operationId: postVatCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /convert\n  method: get\n  operationId: getConvertExchangeRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert\n  method: post\n\
  \  operationId: postConvertExchangeRate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /convert_time\n  method: get\n  operationId: getConvertTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert_time\n  method: post\n  operationId: postConvertTime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /current_time\n  method: get\n  operationId: getCurrentTime\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current_time\n  method: post\n  operationId: postCurrentTime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /historical\n  method: get\n  operationId: getHistoricalExchangeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical\n  method: post\n  operationId: postHistoricalExchangeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live\n  method: get\n  operationId: getLiveExchangeRates\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live\n  method: post\n  operationId: postLiveExchangeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upload\n  method: get\n  operationId: getImageUploadOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /upload\n  method: post\n  operationId: postImageUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /url\n  method: get\n  operationId: getImageFromUrl\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /url\n  method: post\n  operationId: postImageFromUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate\n  method: get\n  operationId: getValidateVat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validate\n  method: post\n  operationId: postValidateVat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate\n  method:\
  \ get\n  operationId: validateVATNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rates\n  method: get\n  operationId: getVATRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calculate\n  method: get\n  operationId: calculateVAT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/agentic-access/abstract-api-agentic-access.yml
summary_line: 25 operations · 9 acting
tags:
- Avatars
- Company Enrichment
- Contacts
- Currency
- Email Verification
- Exchange Rates
- IBAN Validation
- Image Processing
- IP Geolocation
- IP Intelligence
- Phone Validation
- Public Holidays
- Screenshots
- Timezone
- VAT Validation
- Web Scraping
- A2A
---
