---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 16
api_specs:
- filename: ferc-data-api-openapi.json
  format: json
  label: FERC Open Data API
  slug: ferc-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-data-api-openapi.json
- filename: ferc-eforms-api-openapi-derived.yml
  format: yaml
  label: FERC eForms XBRL Submission API
  slug: ferc-eforms-xbrl-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-eforms-api-openapi-derived.yml
consequence_counts:
  read: 16
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Ferc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /SubmissionHistory/ExternalFiling
operation_count: 18
overview: 'FERC exposes 18 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 1 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FERC
provider_slug: ferc
slug: ferc-agentic-access
source_filename: ferc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/ferc-data-api-openapi.json, openapi/ferc-eforms-api-openapi-derived.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\ncurated: partial\ncuration_note: >-\n  Two operations were raised by hand above the heuristic default and are marked `curated: true` —\n  postExternalFiling (mandated, irreversible regulatory filing → safety-critical, human-in-the-loop\n  required) and listPublicSubmissionHistory (anonymous but returns personal data → subject and audit\n  required). The summary counts below reflect those corrections.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 16\n    acting: 2\n  by_consequence:\n    read: 16\n    write: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\n  personal_data_operations:\
  \ 1\noperations:\n- path: /data-assets/\n  method: get\n  operationId: data-asset-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataset/{id}/details/\n  method: get\n  operationId: detail-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataset/{id}/data/\n  method: get\n  operationId: data-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataset/{id}/dictionary/\n  method: get\n  operationId: dictionary-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token\n  method: post\n  operationId: getFilerToken\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SubmissionHistory/ExternalFiling\n  method: post\n  operationId: postExternalFiling\n  curated: true\n  curation_note: >-\n    Raised by hand from the heuristic default (write / conditional). This operation submits a\n    MANDATED regulatory filing to FERC production on behalf of a named credentialed filer. It is\n    irreversible, legally consequential, carries no idempotency key, and a repeat call creates a\n    second filing. Human-in-the-loop is required, not conditional.\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: required\n      proof-of-possession: required\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ required\n      triggers:\n      - always\n    audit: required\n- path: /PublicSubmissionHistory\n  method: get\n  operationId: listPublicSubmissionHistory\n  curated: true\n  curation_note: >-\n    Read-only and anonymous, but the response carries filerEmail — a named individual's work email\n    address — for ~37,600 filings. Treated as personal data: subject required, audit required, and\n    excluded from the agent skills and the candidate MCP tool set. See\n    security/ferc-vulnerability-disclosure.yml.\n  personal_data: true\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - bulk-export\n      - personal-data\n    audit: required\n- path: /SubmissionDetail/{filingID}\n  method: get\n  operationId: getSubmissionDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /SubmissionHistory/forms\n  method: get\n  operationId: listForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getTestStatus\n  method: get\n  operationId: getTestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TaxonomyHistory\n  method: get\n  operationId: listTaxonomyHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TaxonomyHistory/TaxonomyFile/{versionID}\n  method: get\n  operationId: getTaxonomyFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TaxonomyHistory/SampleForm/{versionID}\n  method:\
  \ get\n  operationId: getTaxonomySampleForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TaxonomyHistory/getReleaseFiles\n  method: get\n  operationId: getTaxonomyReleaseFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faq\n  method: get\n  operationId: listFaq\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims\n  method: get\n  operationId: getFilerClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SubmissionHistory\n  method: get\n  operationId: listFilerSubmissionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TaxonomyRevision\n  method: get\n  operationId: listTaxonomyRevisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/agentic-access/ferc-agentic-access.yml
summary_line: 18 operations · 2 acting · 1 human-in-the-loop
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Natural Gas
- Grid
- Regulator
- Government
- Open Data
- Wholesale Power Markets
- Hydropower
- Oil Pipelines
---
