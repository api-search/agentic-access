---
acting_count: 0
action_class_counts:
  connected: 19
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
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Abstract Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Abstract API exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Abstract API
provider_slug: abstract-api
slug: abstract-api-agentic-access
source_filename: abstract-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/abstract-api-avatars.yaml, openapi/abstract-api-company-enrichment.yaml, openapi/abstract-api-email-reputation.yaml,\n  openapi/abstract-api-exchange-rates.yaml, openapi/abstract-api-iban-validation.yaml, openapi/abstract-api-image-processing.yaml,\n  openapi/abstract-api-ip-geolocation.yaml, openapi/abstract-api-ip-intelligence.yaml, openapi/abstract-api-phone-intelligence.yaml,\n  openapi/abstract-api-public-holidays.yaml, openapi/abstract-api-timezones.yaml, openapi/abstract-api-vat-validation.yaml,\n  openapi/abstract-api-web-scraping.yaml, openapi/abstract-api-website-screenshot.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n\
  \    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: generateAvatar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getCompanyEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getEmailReputation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live\n  method: get\n  operationId: getLiveExchangeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert\n  method: get\n  operationId: convertCurrency\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical\n  method: get\n  operationId: getHistoricalExchangeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: validateIBAN\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /url\n  method: get\n  operationId: processImageByURL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getIPGeolocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getIPIntelligence\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getPhoneIntelligence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getPublicHolidays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current_time\n  method: get\n  operationId: getCurrentTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert_time\n  method: get\n  operationId: convertTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validate\n  method: get\n\
  \  operationId: validateVATNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rates\n  method: get\n  operationId: getVATRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calculate\n  method: get\n  operationId: calculateVAT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: scrapeWebPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: captureWebsiteScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/agentic-access/abstract-api-agentic-access.yml
summary_line: 19 operations
tags:
- Avatars
- Company Enrichment
- Contacts
- Currency
- Email Validation
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
---
