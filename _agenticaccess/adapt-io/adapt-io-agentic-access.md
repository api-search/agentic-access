---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 2
api_specs:
- filename: adapt-io-account-api-openapi.yml
  format: yaml
  label: Adapt Account API
  slug: adapt-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-account-api-openapi.yml
- filename: adapt-io-company-api-openapi.yml
  format: yaml
  label: Adapt Company API
  slug: adapt-io-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-company-api-openapi.yml
- filename: adapt-io-contact-api-openapi.yml
  format: yaml
  label: Adapt Contact API
  slug: adapt-io-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-contact-api-openapi.yml
- filename: adapt-io-contribution-api-openapi.yml
  format: yaml
  label: Adapt Contribution API
  slug: adapt-io-contribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-contribution-api-openapi.yml
- filename: adapt-io-email-api-openapi.yml
  format: yaml
  label: Adapt Email API
  slug: adapt-io-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-email-api-openapi.yml
- filename: adapt-io-emailid-api-openapi.yml
  format: yaml
  label: Adapt Emailid API
  slug: adapt-io-emailid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-emailid-api-openapi.yml
- filename: adapt-io-filter-api-openapi.yml
  format: yaml
  label: Adapt Filter API
  slug: adapt-io-filter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-filter-api-openapi.yml
- filename: adapt-io-health-api-openapi.yml
  format: yaml
  label: Adapt Health API
  slug: adapt-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-health-api-openapi.yml
- filename: adapt-io-webhooks-api-openapi.yml
  format: yaml
  label: Adapt Webhooks API
  slug: adapt-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adapt-io/openapi/adapt-io-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adapt Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contact/fetch
operation_count: 4
overview: 'Adapt exposes 4 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Adapt
provider_slug: adapt-io
slug: adapt-io-agentic-access
source_filename: adapt-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/adapt-io-company-search-api-openapi.yml, openapi/adapt-io-contact-enrichment-api-openapi.yml,\n  openapi/adapt-io-contact-purchase-api-openapi.yml, openapi/adapt-io-contact-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 2\n    acting: 2\n  by_consequence:\n    read: 2\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /company/search\n  method: post\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact/enrich\n  method: post\n  operationId: enrichContact\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/fetch\n  method: post\n  operationId: purchaseContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/search\n  method: post\n  operationId: searchContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/adapt-io/agentic-access/adapt-io-agentic-access.yml
summary_line: 4 operations · 2 acting
tags:
- B2B Data
- Contact Data
- Company Data
- Lead Intelligence
- Sales Intelligence
- Sales Acceleration
- Data Enrichment
- Prospecting
- Lead Generation
- Email Finder
- Account Based Marketing
- CRM Enrichment
- Marketing
- Sales
---
