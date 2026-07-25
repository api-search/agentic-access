---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: orcid-address-api-openapi.yml
  format: yaml
  label: ORCID Address API
  slug: orcid-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-address-api-openapi.yml
- filename: orcid-educations-api-openapi.yml
  format: yaml
  label: ORCID Educations API
  slug: orcid-educations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-educations-api-openapi.yml
- filename: orcid-email-api-openapi.yml
  format: yaml
  label: ORCID Email API
  slug: orcid-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-email-api-openapi.yml
- filename: orcid-employments-api-openapi.yml
  format: yaml
  label: ORCID Employments API
  slug: orcid-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-employments-api-openapi.yml
- filename: orcid-external-identifiers-api-openapi.yml
  format: yaml
  label: ORCID External Identifiers API
  slug: orcid-external-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-external-identifiers-api-openapi.yml
- filename: orcid-fundings-api-openapi.yml
  format: yaml
  label: ORCID Fundings API
  slug: orcid-fundings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-fundings-api-openapi.yml
- filename: orcid-keywords-api-openapi.yml
  format: yaml
  label: ORCID Keywords API
  slug: orcid-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-keywords-api-openapi.yml
- filename: orcid-other-names-api-openapi.yml
  format: yaml
  label: ORCID Other Names API
  slug: orcid-other-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-other-names-api-openapi.yml
- filename: orcid-peer-reviews-api-openapi.yml
  format: yaml
  label: ORCID Peer Reviews API
  slug: orcid-peer-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-peer-reviews-api-openapi.yml
- filename: orcid-person-api-openapi.yml
  format: yaml
  label: ORCID Person API
  slug: orcid-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-person-api-openapi.yml
- filename: orcid-personal-details-api-openapi.yml
  format: yaml
  label: ORCID Personal Details API
  slug: orcid-personal-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-personal-details-api-openapi.yml
- filename: orcid-record-api-openapi.yml
  format: yaml
  label: ORCID Record API
  slug: orcid-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-record-api-openapi.yml
- filename: orcid-researcher-urls-api-openapi.yml
  format: yaml
  label: ORCID Researcher Urls API
  slug: orcid-researcher-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-researcher-urls-api-openapi.yml
- filename: orcid-summary-api-openapi.yml
  format: yaml
  label: ORCID Summary API
  slug: orcid-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-summary-api-openapi.yml
- filename: orcid-works-api-openapi.yml
  format: yaml
  label: ORCID Works API
  slug: orcid-works-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/openapi/orcid-works-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Orcid Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'ORCID exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ORCID
provider_slug: orcid
slug: orcid-agentic-access
source_filename: orcid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/orcid-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /{orcid_id}/record\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/person\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/summary\n  method: get\n  operationId: getSummary\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/address\n  method: get\n  operationId: getAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/email\n  method: get\n  operationId: getEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/external-identifiers\n  method: get\n  operationId: getExternalIdentifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/keywords\n  method: get\n  operationId: getKeywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/other-names\n  method: get\n  operationId: getOtherNames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/personal-details\n  method: get\n  operationId: getPersonalDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/researcher-urls\n  method: get\n  operationId: getResearcherUrls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/educations\n  method: get\n  operationId: getEducations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/employments\n  method: get\n\
  \  operationId: getEmployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/fundings\n  method: get\n  operationId: getFundings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/peer-reviews\n  method: get\n  operationId: getPeerReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/works\n  method: get\n  operationId: getWorks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{orcid_id}/works/{put_codes}\n  method: get\n  operationId: getWorksBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orcid/refs/heads/main/agentic-access/orcid-agentic-access.yml
summary_line: 16 operations
tags:
- Academic
- Identity
- Researchers
---
