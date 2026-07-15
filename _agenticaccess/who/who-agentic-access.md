---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 21
api_specs:
- filename: $metadata
  format: yaml
  label: WHO GHO OData API
  slug: who-gho-odata-api
  spec_type: OpenAPI
  url: https://ghoapi.azureedge.net/api/$metadata
- filename: index.html
  format: yaml
  label: WHO ICD API
  slug: who-icd-api
  spec_type: OpenAPI
  url: https://id.who.int/swagger/index.html
consequence_counts:
  read: 21
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Who Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'World Health Organization (WHO) exposes 25 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: World Health Organization (WHO)
provider_slug: who
slug: who-agentic-access
source_filename: who-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/who-icd-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 21\n    acting: 4\n  by_consequence:\n    read: 21\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /icd/entity\n  method: get\n  operationId: GetFoundation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/entity/{id}\n  method: get\n  operationId: GetFoundationEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - icdapi_access\n- path: /icd/entity/autocode\n  method: get\n  operationId: AutoCodeFoundation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/entity/search\n  method: get\n  operationId: SearchFoundation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/entity/search\n  method: post\n  operationId: SearchFoundation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{linearizationname}\n  method: get\n  operationId:\
  \ GetReleasesForLinerization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{linearizationname}/{id}\n  method: get\n  operationId: GetAvailableReleasesForLinearizationEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{linearizationname}/{id}/{residual}\n  method: get\n  operationId: GetAvailableReleasesForLinearizationResidualEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/{linearizationname}\n  method: get\n  operationId: GetLinearization\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/{linearizationname}/{id}\n  method: get\n  operationId: GetLinearizationEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/{linearizationname}/{id}/{residual}\n  method: get\n  operationId: GetLinearizationResidualEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/{linearizationname}/autocode\n  method: get\n  operationId: AutoCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n\
  - path: /icd/release/11/{releaseId}/{linearizationname}/codeinfo/{code}\n  method: get\n  operationId: GetCodeInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/{linearizationname}/describe\n  method: get\n  operationId: Describe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/{linearizationname}/lookup\n  method: get\n  operationId: Lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/{linearizationname}/search\n  method: get\n  operationId: SearchLinearization\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/{linearizationname}/search\n  method: post\n  operationId: SearchLinearization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/codedit\n  method: get\n  operationId: CertificateCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/codedit\n  method: post\n  operationId: CertificateCheck\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/doris\n  method: get\n  operationId: UnderlyingCauseOfDeathDetection1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/11/{releaseId}/doris\n  method: post\n  operationId: UnderlyingCauseOfDeathDetection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - icdapi_access\n- path: /icd/release/10\n  method: get\n\
  \  operationId: GetICD10Releases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/10/{code}\n  method: get\n  operationId: GetAvailableReleasesForICD10Entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/10/{releaseId}\n  method: get\n  operationId: GetICD10Release\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - icdapi_access\n- path: /icd/release/10/{releaseId}/{code}\n  method: get\n  operationId: GetICD10Entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - icdapi_access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/who/refs/heads/main/agentic-access/who-agentic-access.yml
summary_line: 25 operations · 4 acting
tags:
- Health
- Global Health
- Disease Surveillance
- Immunization
- Health Statistics
- ICD
- WHO
- United Nations
- Open Data
---
