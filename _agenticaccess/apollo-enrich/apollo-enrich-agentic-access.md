---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 1
api_specs:
- filename: apollo-enrich-openapi.yml
  format: yaml
  label: Apollo People Enrichment API
  slug: apollo-people-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-openapi.yml
- filename: apollo-enrich-openapi.yml
  format: yaml
  label: Apollo People Search API
  slug: apollo-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-openapi.yml
- filename: apollo-enrich-openapi.yml
  format: yaml
  label: Apollo Organization Enrichment API
  slug: apollo-organization-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-openapi.yml
- filename: apollo-enrich-openapi.yml
  format: yaml
  label: Apollo Organization Search API
  slug: apollo-organization-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-openapi.yml
- filename: apollo-enrich-openapi.yml
  format: yaml
  label: Apollo Contacts API
  slug: apollo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-openapi.yml
- filename: apollo-enrich-openapi.yml
  format: yaml
  label: Apollo Accounts API
  slug: apollo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-openapi.yml
- filename: apollo-enrich-openapi.yml
  format: yaml
  label: Apollo Sequences API
  slug: apollo-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/openapi/apollo-enrich-openapi.yml
consequence_counts:
  read: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apollo Enrich Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Apollo.io exposes 14 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apollo.io
provider_slug: apollo-enrich
slug: apollo-enrich-agentic-access
source_filename: apollo-enrich-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/apollo-enrich-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 13\n    connected: 1\n  by_consequence:\n    write: 13\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /people/match\n  method: post\n  operationId: matchPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/bulk_match\n  method: post\n  operationId: bulkMatchPeople\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mixed_people/api_search\n  method: post\n  operationId: searchPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/enrich\n  method: get\n  operationId: enrichOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/bulk_enrich\n  method: post\n  operationId: bulkEnrichOrganizations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mixed_companies/search\n  method: post\n  operationId: searchOrganizations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/search\n  method: post\n  operationId: searchContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/search\n  method: post\n  operationId: searchAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: post\n  operationId: createAccount\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_campaigns/search\n  method: post\n  operationId: searchSequences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_campaigns/{id}/add_contact_ids\n\
  \  method: post\n  operationId: addContactsToSequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-enrich/refs/heads/main/agentic-access/apollo-enrich-agentic-access.yml
summary_line: 14 operations · 13 acting
tags:
- Contact Discovery
- Data Enrichment
- Sales Intelligence
- B2B Data
- Prospecting
- Web Intelligence
- Lead Generation
- People Search
---
