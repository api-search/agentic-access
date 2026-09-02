---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: pubmed-history-api-openapi.yml
  format: yaml
  label: PubMed History API
  slug: pubmed-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-history-api-openapi.yml
- filename: pubmed-info-api-openapi.yml
  format: yaml
  label: PubMed Info API
  slug: pubmed-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-info-api-openapi.yml
- filename: pubmed-links-api-openapi.yml
  format: yaml
  label: PubMed Links API
  slug: pubmed-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-links-api-openapi.yml
- filename: pubmed-retrieval-api-openapi.yml
  format: yaml
  label: PubMed Retrieval API
  slug: pubmed-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-retrieval-api-openapi.yml
- filename: pubmed-search-api-openapi.yml
  format: yaml
  label: PubMed Search API
  slug: pubmed-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-search-api-openapi.yml
- filename: pubmed-summary-api-openapi.yml
  format: yaml
  label: PubMed Summary API
  slug: pubmed-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-summary-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pubmed Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'PubMed exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PubMed
provider_slug: pubmed
slug: pubmed-agentic-access
source_filename: pubmed-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/entrez-eutils.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /esearch.fcgi\n  method: get\n  operationId: ESearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /efetch.fcgi\n  method: get\n  operationId: EFetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esummary.fcgi\n  method: get\n  operationId: ESummary\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elink.fcgi\n  method: get\n  operationId: ELink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /epost.fcgi\n  method: post\n  operationId: EPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einfo.fcgi\n  method: get\n  operationId: EInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espell.fcgi\n  method: get\n  operationId: ESpell\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /egquery.fcgi\n  method: get\n  operationId: EGQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ecitmatch.cgi\n  method: get\n  operationId: ECitMatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/agentic-access/pubmed-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Biomedical
- Life Science
- Research
- Literature
- Citations
- Abstracts
- Mesh
- Genomics
- PubMed
- NCBI
---
