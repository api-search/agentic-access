---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 23
api_specs:
- filename: getapi-nl-bag-addresses-and-buildings-register-api-openapi.yml
  format: yaml
  label: getapi-nl BAG – Addresses and Buildings Register API
  slug: getapi-nl-bag-addresses-and-buildings-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-bag-addresses-and-buildings-register-api-openapi.yml
- filename: getapi-nl-cbs-sbi-codes-api-openapi.yml
  format: yaml
  label: getapi-nl CBS - SBI Codes API
  slug: getapi-nl-cbs-sbi-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-cbs-sbi-codes-api-openapi.yml
- filename: getapi-nl-dns-lookup-api-openapi.yml
  format: yaml
  label: getapi-nl DNS Lookup API
  slug: getapi-nl-dns-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-dns-lookup-api-openapi.yml
- filename: getapi-nl-dnsbl-spam-blacklist-api-openapi.yml
  format: yaml
  label: getapi-nl DNSBL / Spam Blacklist API
  slug: getapi-nl-dnsbl-spam-blacklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-dnsbl-spam-blacklist-api-openapi.yml
- filename: getapi-nl-dso-environmental-information-api-openapi.yml
  format: yaml
  label: getapi-nl DSO - Environmental information API
  slug: getapi-nl-dso-environmental-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-dso-environmental-information-api-openapi.yml
- filename: getapi-nl-email-validation-api-openapi.yml
  format: yaml
  label: getapi-nl Email Validation API
  slug: getapi-nl-email-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-email-validation-api-openapi.yml
- filename: getapi-nl-geolocation-services-api-openapi.yml
  format: yaml
  label: getapi-nl Geolocation services API
  slug: getapi-nl-geolocation-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-geolocation-services-api-openapi.yml
- filename: getapi-nl-iban-bic-validation-api-openapi.yml
  format: yaml
  label: getapi-nl IBAN / BIC Validation API
  slug: getapi-nl-iban-bic-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-iban-bic-validation-api-openapi.yml
- filename: getapi-nl-ip-location-lookup-api-openapi.yml
  format: yaml
  label: getapi-nl IP Location Lookup API
  slug: getapi-nl-ip-location-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-ip-location-lookup-api-openapi.yml
- filename: getapi-nl-ndw-charging-points-api-openapi.yml
  format: yaml
  label: getapi-nl NDW - Charging points API
  slug: getapi-nl-ndw-charging-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-ndw-charging-points-api-openapi.yml
- filename: getapi-nl-ndw-emission-zones-api-openapi.yml
  format: yaml
  label: getapi-nl NDW - Emission zones API
  slug: getapi-nl-ndw-emission-zones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-ndw-emission-zones-api-openapi.yml
- filename: getapi-nl-ndw-truckparking-api-openapi.yml
  format: yaml
  label: getapi-nl NDW - Truckparking API
  slug: getapi-nl-ndw-truckparking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-ndw-truckparking-api-openapi.yml
- filename: getapi-nl-property-data-api-openapi.yml
  format: yaml
  label: getapi-nl Property data API
  slug: getapi-nl-property-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-property-data-api-openapi.yml
- filename: getapi-nl-rdw-api-openapi.yml
  format: yaml
  label: getapi-nl RDW API
  slug: getapi-nl-rdw-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-rdw-api-openapi.yml
- filename: getapi-nl-rvo-api-openapi.yml
  format: yaml
  label: getapi-nl RVO API
  slug: getapi-nl-rvo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-rvo-api-openapi.yml
- filename: getapi-nl-site-scraping-api-openapi.yml
  format: yaml
  label: getapi-nl Site Scraping API
  slug: getapi-nl-site-scraping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-site-scraping-api-openapi.yml
- filename: getapi-nl-vat-validation-api-openapi.yml
  format: yaml
  label: getapi-nl VAT Validation API
  slug: getapi-nl-vat-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-vat-validation-api-openapi.yml
consequence_counts:
  read: 23
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Getapi Nl Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'getapi-nl exposes 30 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: getapi-nl
provider_slug: getapi-nl
slug: getapi-nl-agentic-access
source_filename: getapi-nl-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/getapi-nl-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 23\n    acting: 7\n  by_consequence:\n    read: 23\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/kadaster/bag/address\n  method: get\n  operationId: kadaster.bag.address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kadaster/bag/address-suggest\n  method: get\n  operationId: kadaster.bag.address-suggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/kadaster/bag/id\n  method: get\n  operationId: kadaster.bag.id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cbs/sbi\n  method: get\n  operationId: cbs.sbi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cbs/sbi/search\n  method: get\n  operationId: cbs.sbi.search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cbs/sbi/{code}\n  method: get\n  operationId: cbs.sbi.detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookup/dns/nameservers\n  method: get\n  operationId: lookup.dns.nameservers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookup/dns/records\n  method: get\n  operationId: lookup.dns.records\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validate/dnsbl\n  method: post\n  operationId: validation.dnsbl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dso/documents\n  method: get\n  operationId: dso.documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dso/plans\n  method: get\n  operationId: dso.plans\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validate/email\n  method: post\n  operationId: validation.email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/validate/email/batch\n  method: post\n  operationId: validation.email.batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/validate/email/disposable\n  method: post\n  operationId: validation.email.disposable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lookup/postcode\n  method: get\n  operationId: lookup.postcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validate/iban\n  method: post\n  operationId: validation.iban\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lookup/ip\n  method: get\n  operationId: lookup.ip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ndw/laadpunten\n\
  \  method: get\n  operationId: ndw.laadpunten\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ndw/laadpunten/{id}\n  method: get\n  operationId: ndw.laadpunten.detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ndw/emissiezones\n  method: get\n  operationId: ndw.emissiezones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ndw/emissiezones/{id}\n  method: get\n  operationId: ndw.emissiezones.detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ndw/truckparking\n  method: get\n  operationId: ndw.truckparking\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ndw/truckparking/{id}\n  method: get\n  operationId: ndw.truckparking.detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/property/pandgegevens\n  method: get\n  operationId: property.pandgegevens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/property/pandgegevens-lite\n  method: get\n  operationId: property.pandgegevens-lite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/property/woz-waarde\n  method: get\n  operationId: property.woz-waarde\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rdw/vehicle\n  method: get\n  operationId: rdw.vehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/property/energy-label\n  method: get\n  operationId: property.energy-label\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scraping/email\n  method: post\n  operationId: scraping.email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/validate/vat\n  method: post\n  operationId: validation.vat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/getapi-nl/agentic-access/getapi-nl-agentic-access.yml
summary_line: 30 operations · 7 acting
tags:
- Company
- Dutch
- Web Scraping
- Data Validation
---
