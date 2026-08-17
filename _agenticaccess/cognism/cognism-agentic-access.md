---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 24
api_specs:
- filename: cognism-api-openapi.yml
  format: yaml
  label: Cognism Enrichment API
  slug: enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/openapi/cognism-api-openapi.yml
consequence_counts:
  financial: 1
  read: 24
description: Recommended x-agentic-access execution contracts for the Cognism API. The baseline was generated mechanically from the OpenAPI, then CURATED against what Cognism actually documents. The mechanical pass classified all six POST operations as acting/write; five of them - searchContacts, searchAccounts, enrichContact, enrichAccount and redeemAccounts - are POST-shaped reads that mutate nothing and consume no credits, and have been reclassified. redeemContacts was raised to acting/financial because it is the single operation in this API that spends money, and it has no idempotency key to protect a retry. A governance starting point - bind audience per deployment.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Cognism Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Cognism exposes 25 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cognism
provider_slug: cognism
slug: cognism-agentic-access
source_filename: cognism-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/cognism-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts for the Cognism API. The baseline was generated\n  mechanically from the OpenAPI, then CURATED against what Cognism actually documents. The mechanical\n  pass classified all six POST operations as acting/write; five of them - searchContacts, searchAccounts,\n  enrichContact, enrichAccount and redeemAccounts - are POST-shaped reads that mutate nothing and consume\n  no credits, and have been reclassified. redeemContacts was raised to acting/financial because it is\n  the single operation in this API that spends money, and it has no idempotency key to protect a retry.\n  A governance starting point - bind audience per deployment.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 24\n    acting: 1\n  by_consequence:\n    read: 24\n    financial: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/search/contact/search\n\
  \  method: post\n  operationId: searchContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: recommended\n    x-curation-note: POST but semantically a read - the body is a filter set, not a mutation. Consumes\n      no credits.\n- path: /api/search/account/search\n  method: post\n  operationId: searchAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: recommended\n    x-curation-note: POST but semantically a read. Consumes no credits.\n- path: /api/search/contact/redeem\n  method: post\n  operationId: redeemContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: financial\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - batch-size\n \
  \     - spend-threshold\n      - abnormal\n    audit: required\n    purpose: required\n    x-curation-note: THE metered operation. First redemption of a contact consumes a credit; re-redemption\n      of an already-redeemed contact is free. There is no idempotency key, so a retry of a first redemption\n      can spend twice. Cap the token, require a purpose, audit every call, and escalate on batch size\n      or spend threshold.\n- path: /api/search/account/redeem\n  method: post\n  operationId: redeemAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: recommended\n    x-curation-note: Redeem verb, but account redemptions are explicitly free of credits.\n- path: /api/search/contact/enrich\n  method: post\n  operationId: enrichContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 3600\n    audit: recommended\n    x-curation-note: POST but semantically a read - matches an input record against the database. Consumes\n      no credits.\n- path: /api/search/account/enrich\n  method: post\n  operationId: enrichAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: recommended\n    x-curation-note: POST but semantically a read. Consumes no credits.\n- path: /api/search/entitlement/contactEntitlementSubscription\n  method: get\n  operationId: getContactEntitlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/entitlement/accountEntitlementSubscription\n  method: get\n  operationId: getAccountEntitlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/search/filter/technologiesSearch\n  method: get\n  operationId: listTechnologies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/managementLevels\n  method: get\n  operationId: listManagementLevels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/companySizes\n  method: get\n  operationId: listCompanySizes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/industries\n  method: get\n  operationId: listIndustries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/jobFunctions\n\
  \  method: get\n  operationId: listJobFunctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/regions\n  method: get\n  operationId: listRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/states\n  method: get\n  operationId: listStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/sic\n  method: get\n  operationId: listSicCodes\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/isic\n  method: get\n  operationId: listIsicCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/naics\n  method: get\n  operationId: listNaicsCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/skills\n  method: get\n  operationId: listSkills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/filter/companyTypes\n  method: get\n  operationId: listCompanyTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/search/filter/seniority\n  method: get\n  operationId: listSeniorityLevels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/contact/optOut\n  method: get\n  operationId: listOptOutContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/contact/optOut/email/{email}\n  method: get\n  operationId: getOptOutByEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/contact/optOut/id/{id}\n  method: get\n  operationId: getOptOutById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\ncurated: '2026-08-13'\ncuration_source:\n- https://help.cognism.com/hc/en-gb/articles/37383428888978-API-Authentication-Credits\n\
  - conventions/cognism-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognism/refs/heads/main/agentic-access/cognism-agentic-access.yml
summary_line: 25 operations · 1 acting
tags:
- Sales Intelligence
- B2B
- Enrichment
- Contact Data
- GDPR
- Intent Data
- Lead Generation
- Firmographics
- Technographics
- Company Data
- Prospecting
- Data as a Service
---
