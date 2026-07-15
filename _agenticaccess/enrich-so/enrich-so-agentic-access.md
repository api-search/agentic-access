---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 5
api_specs:
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Person Enrichment API
  slug: enrich-so-person-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Email Finder API
  slug: enrich-so-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Email Verification API
  slug: enrich-so-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Phone Finder API
  slug: enrich-so-phone-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Company Intelligence API
  slug: enrich-so-company-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
- filename: enrich-so-openapi.yml
  format: yaml
  label: Enrich Lead Finder API
  slug: enrich-so-lead-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-openapi.yml
consequence_counts:
  read: 5
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Enrich So Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Enrich exposes 17 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Enrich
provider_slug: enrich-so
slug: enrich-so-agentic-access
source_filename: enrich-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/enrich-so-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 12\n    connected: 5\n  by_consequence:\n    write: 12\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /reverse-lookup/lookup\n  method: post\n  operationId: lookupProfileByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reverse-lookup/batch\n  method: post\n  operationId: lookupProfilesBatch\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reverse-lookup/batch/{batchId}\n  method: get\n  operationId: getBulkLookupResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-finder\n  method: post\n  operationId: findProfessionalEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-finder/batch\n  method: post\n  operationId: findEmailsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-validation\n  method: post\n  operationId: validateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-validation/batch\n  method: post\n  operationId: validateEmailsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reverse-lookup/phones\n  method: get\n  operationId: findPhoneNumbers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse-lookup/phones/batch\n  method: post\n  operationId: findPhoneNumbersBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ip-to-company\n  method: post\n  operationId: resolveCompanyFromIp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company-follower\n  method: post\n  operationId: startCompanyFollowerScrape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company-follower/{batchId}\n  method: get\n  operationId: getCompanyFollowerResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lead-finder/search\n  method: post\n  operationId: searchLeads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lead-finder/count\n  method: post\n  operationId: countMatchingLeads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lead-finder/reveal\n  method: post\n  operationId: revealContactInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/balance\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallet/transactions\n  method: get\n  operationId: getTransactionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/agentic-access/enrich-so-agentic-access.yml
summary_line: 17 operations · 12 acting
tags:
- Data Enrichment
- Contact Discovery
- Web Intelligence
- B2B Data
- Lead Enrichment
- Email Finder
- Email Verification
- Phone Numbers
- LinkedIn
- Reference Data
---
