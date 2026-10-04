---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: fullenrich-account-api-openapi.yml
  format: yaml
  label: FullEnrich Account API
  slug: fullenrich-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-account-api-openapi.yml
- filename: fullenrich-company-api-openapi.yml
  format: yaml
  label: FullEnrich Company API
  slug: fullenrich-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-company-api-openapi.yml
- filename: fullenrich-contact-api-openapi.yml
  format: yaml
  label: FullEnrich Contact API
  slug: fullenrich-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-contact-api-openapi.yml
- filename: fullenrich-people-api-openapi.yml
  format: yaml
  label: FullEnrich People API
  slug: fullenrich-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-people-api-openapi.yml
consequence_counts:
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fullenrich Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'FullEnrich exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FullEnrich
provider_slug: fullenrich
slug: fullenrich-agentic-access
source_filename: fullenrich-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/fullenrich-account-api-openapi.yml, openapi/fullenrich-company-api-openapi.yml,\n  openapi/fullenrich-contact-api-openapi.yml, openapi/fullenrich-people-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 6\n    acting: 4\n  by_consequence:\n    read: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /account/keys/verify\n  method: get\n  operationId: checkKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/credits\n  method: get\n  operationId: getAccountCredits\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/search\n  method: post\n  operationId: postCompanySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/lookup\n  method: post\n  operationId: postCompanyLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/enrich/bulk\n  method: post\n  operationId: postContactBulkEnrich\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /contact/enrich/bulk/{enrichment_id}\n  method: get\n  operationId: GetContactBulkEnrichByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact/reverse/email/bulk\n  method: post\n  operationId: postContactBulkReverseEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/reverse/email/bulk/{enrichment_id}\n  method: get\n  operationId: GetContactBulkReverseEmailByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/search\n  method: post\n  operationId: postPeopleSearch\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/lookup\n  method: post\n  operationId: postPeopleLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/agentic-access/fullenrich-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- B2B Data
- Contact Enrichment
- Email Finder
- Phone Finder
- Waterfall Enrichment
- Sales Intelligence
- People Search
- Company Search
- Reverse Email Lookup
- Agent Ready
- A2A
---
