---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 3
api_specs:
- filename: ocean-io-autocomplete-api-openapi.yml
  format: yaml
  label: Ocean.io Autocomplete API
  slug: ocean-io-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-autocomplete-api-openapi.yml
- filename: ocean-io-enrich-api-openapi.yml
  format: yaml
  label: Ocean.io Enrich API
  slug: ocean-io-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-enrich-api-openapi.yml
- filename: ocean-io-lookup-api-openapi.yml
  format: yaml
  label: Ocean.io Lookup API
  slug: ocean-io-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-lookup-api-openapi.yml
- filename: ocean-io-ocean-io-api-documentation-api-openapi.yml
  format: yaml
  label: Ocean.io Ocean.io API Documentation API
  slug: ocean-io-ocean-io-api-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-ocean-io-api-documentation-api-openapi.yml
- filename: ocean-io-other-api-openapi.yml
  format: yaml
  label: Ocean.io Other API
  slug: ocean-io-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-other-api-openapi.yml
- filename: ocean-io-reveal-api-openapi.yml
  format: yaml
  label: Ocean.io Reveal API
  slug: ocean-io-reveal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-reveal-api-openapi.yml
- filename: ocean-io-search-api-openapi.yml
  format: yaml
  label: Ocean.io Search API
  slug: ocean-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-search-api-openapi.yml
- filename: ocean-io-segmentation-api-openapi.yml
  format: yaml
  label: Ocean.io Segmentation API
  slug: ocean-io-segmentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/openapi/ocean-io-segmentation-api-openapi.yml
consequence_counts:
  read: 3
  safety-critical: 1
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Ocean Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/autocomplete/skills
operation_count: 26
overview: 'Ocean.io exposes 26 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 22 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ocean.io
provider_slug: ocean-io
slug: ocean-io-agentic-access
source_filename: ocean-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/ocean-io-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 23\n    connected: 3\n  by_consequence:\n    write: 22\n    safety-critical: 1\n    read: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /v2/autocomplete/companies\n  method: post\n  operationId: autoCompleteCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/autocomplete/keywords\n  method: post\n  operationId: autoCompleteKeywords\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/autocomplete/job-titles\n  method: post\n  operationId: autoCompleteJobTitles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/autocomplete/locations\n  method: post\n  operationId: autoCompleteLocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v2/autocomplete/skills\n  method: post\n  operationId: autoCompleteSkills\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/search/companies\n  method: post\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/search/companies\n  method: post\n  operationId: searchCompaniesV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrich/company\n  method: post\n  operationId: enrichCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrich/person\n  method: post\n  operationId: enrichPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/data-fields\n  method: get\n  operationId: getDataFieldsPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/search/people\n  method: post\n  operationId: searchPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/search/people\n  method: post\n  operationId: searchPeopleV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/search/people/preview\n  method: post\n  operationId: searchPeopleV3Preview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/credits/balance\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/lookup/companies\n  method: post\n  operationId: lookupCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/lookup/people\n  method: post\n  operationId: lookupPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /v2/reveal/emails\n  method: post\n  operationId: revealEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/reveal/phones\n  method: post\n  operationId: revealPhones\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warmup/companies\n  method: post\n  operationId: warmupCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/search/companies/preview\n  method: post\n  operationId: previewSearchCompaniesV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrich/companies\n  method: post\n  operationId: enrichCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrich/people\n  method: post\n  operationId: enrichPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/segmentation/{segmentation_id}\n  method: get\n  operationId: getSegmentation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/segmentation\n  method: post\n  operationId: createSegmentation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/segmentation/{segmentation_id}/markDomains\n  method: post\n  operationId: addMarkedDomains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/segmentation/{segmentation_id}/attribute-domains\n  method: post\n  operationId: attributeSegmentationDomains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-io/refs/heads/main/agentic-access/ocean-io-agentic-access.yml
summary_line: 26 operations · 23 acting · 1 human-in-the-loop
tags:
- Sales Intelligence
- B2B
- Enrichment
- Lookalike
- Account Based Marketing
- Prospecting
- Company Data
- People Data
- Contact Data
- Segmentation
- Go-To-Market
- MCP
---
