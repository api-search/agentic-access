---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 10
api_specs:
- filename: hunter-domain-search-api-openapi.yml
  format: yaml
  label: Hunter Domain Search API
  slug: hunter-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-domain-search-api-openapi.yml
- filename: hunter-email-finder-api-openapi.yml
  format: yaml
  label: Hunter Email Finder API
  slug: hunter-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-email-finder-api-openapi.yml
- filename: hunter-email-verifier-api-openapi.yml
  format: yaml
  label: Hunter Email Verifier API
  slug: hunter-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-email-verifier-api-openapi.yml
- filename: hunter-email-count-api-openapi.yml
  format: yaml
  label: Hunter Email Count API
  slug: hunter-email-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-email-count-api-openapi.yml
- filename: hunter-discover-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: hunter-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-discover-api-openapi.yml
- filename: hunter-enrichment-api-openapi.yml
  format: yaml
  label: Hunter Enrichment API
  slug: hunter-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-enrichment-api-openapi.yml
- filename: hunter-account-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: hunter-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-account-api-openapi.yml
- filename: hunter-leads-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: hunter-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/openapi/hunter-leads-api-openapi.yml
consequence_counts:
  read: 10
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hunter Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Hunter exposes 15 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hunter
provider_slug: hunter-io
slug: hunter-io-agentic-access
source_filename: hunter-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hunter-account-api-openapi.yml, openapi/hunter-discover-api-openapi.yml, openapi/hunter-domain-search-api-openapi.yml,\n  openapi/hunter-email-count-api-openapi.yml, openapi/hunter-email-finder-api-openapi.yml, openapi/hunter-email-verifier-api-openapi.yml,\n  openapi/hunter-enrichment-api-openapi.yml, openapi/hunter-leads-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 10\n    acting: 5\n  by_consequence:\n    read: 10\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /discover\n  method: post\n  operationId: discoverCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domain-search\n  method: get\n  operationId: domainSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-count\n  method: get\n  operationId: emailCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-finder\n  method: get\n  operationId: emailFinder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /email-verifier\n  method: get\n  operationId: emailVerifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/find\n  method: get\n  operationId: enrichPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/find\n  method: get\n  operationId: enrichCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /combined/find\n  method: get\n  operationId: enrichCombined\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: get\n  operationId: listLeads\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: post\n  operationId: createLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads\n  method: put\n  operationId: upsertLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads/{id}\n  method: get\n  operationId: getLead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/{id}\n  method:\
  \ patch\n  operationId: updateLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads/{id}\n  method: delete\n  operationId: deleteLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hunter-io/refs/heads/main/agentic-access/hunter-io-agentic-access.yml
summary_line: 15 operations · 5 acting
tags:
- Email Finder
- Email Verifier
- Lead Generation
- Outreach
- Prospecting
- Enrichment
- Sales
- Marketing
---
