---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: gleif-corporate-relationships-api-openapi.yml
  format: yaml
  label: GLEIF Corporate Relationships API
  slug: gleif-corporate-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-corporate-relationships-api-openapi.yml
- filename: gleif-lei-issuers-api-openapi.yml
  format: yaml
  label: GLEIF LEI Issuers API
  slug: gleif-lei-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-lei-issuers-api-openapi.yml
- filename: gleif-lei-records-api-openapi.yml
  format: yaml
  label: GLEIF LEI Records API
  slug: gleif-lei-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-lei-records-api-openapi.yml
- filename: gleif-reference-data-api-openapi.yml
  format: yaml
  label: GLEIF Reference Data API
  slug: gleif-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-reference-data-api-openapi.yml
- filename: gleif-search-api-openapi.yml
  format: yaml
  label: GLEIF Search API
  slug: gleif-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/openapi/gleif-search-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gleif Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'GLEIF exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GLEIF
provider_slug: gleif
slug: gleif-agentic-access
source_filename: gleif-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gleif-lei-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /lei-records\n  method: get\n  operationId: listLeiRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-records/{lei}\n  method: get\n  operationId: getLeiRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-records/{lei}/direct-children\n  method: get\n  operationId:\
  \ getLeiRecordDirectChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-records/{lei}/ultimate-children\n  method: get\n  operationId: getLeiRecordUltimateChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-records/{lei}/managing-lou\n  method: get\n  operationId: getLeiRecordManagingLou\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-records/{lei}/lei-issuer\n  method: get\n  operationId: getLeiRecordLeiIssuer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-records/{lei}/field-modifications\n  method: get\n  operationId: getLeiRecordFieldModifications\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-issuers\n  method: get\n  operationId: listLeiIssuers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-issuers/{id}\n  method: get\n  operationId: getLeiIssuer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-issuers/{id}/jurisdictions\n  method: get\n  operationId: getLeiIssuerJurisdictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lei-issuers/{id}/fundJurisdictions\n  method: get\n  operationId: getLeiIssuerFundJurisdictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fuzzycompletions\n  method: get\n  operationId: getFuzzyCompletions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entity-legal-forms\n  method: get\n  operationId: listEntityLegalForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entity-legal-forms/{id}\n  method: get\n  operationId: getEntityLegalForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registration-authorities\n  method: get\n  operationId: listRegistrationAuthorities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /registration-authorities/{id}\n  method: get\n  operationId: getRegistrationAuthority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gleif/refs/heads/main/agentic-access/gleif-agentic-access.yml
summary_line: 16 operations
tags:
- Legal Entity Identifier
- LEI
- vLEI
- Financial Data
- Corporate Identity
- Entity Verification
- Reference Data
- Open Data
---
