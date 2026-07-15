---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 16
api_specs:
- filename: ncbi-e-utilities-openapi.yml
  format: yaml
  label: NCBI E-Utilities API
  slug: ncbi-e-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/ncbi-e-utilities-openapi.yml
- filename: openapi3.docs.yaml
  format: yaml
  label: NCBI Datasets REST API
  slug: ncbi-datasets-api
  spec_type: OpenAPI
  url: https://www.ncbi.nlm.nih.gov/datasets/docs/v2/openapi3/openapi3.docs.yaml
- filename: ncbi-blast-openapi.yml
  format: yaml
  label: NCBI BLAST URL API
  slug: ncbi-blast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/ncbi-blast-openapi.yml
- filename: nlm-clinicaltrials-openapi.yml
  format: yaml
  label: ClinicalTrials.gov API
  slug: nlm-clinical-trials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/nlm-clinicaltrials-openapi.yml
consequence_counts:
  read: 16
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: United States National Library Of Medicine Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'United States National Library of Medicine exposes 17 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: United States National Library of Medicine
provider_slug: united-states-national-library-of-medicine
slug: united-states-national-library-of-medicine-agentic-access
source_filename: united-states-national-library-of-medicine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ncbi-blast-openapi.yml, openapi/ncbi-datasets-openapi.yml, openapi/ncbi-e-utilities-openapi.yml,\n  openapi/nlm-clinicaltrials-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 1\n    connected: 16\n  by_consequence:\n    write: 1\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /Blast.cgi\n  method: put\n  operationId: submitBlastSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /Blast.cgi\n  method: get\n  operationId: getBlastResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /genome/taxon/{taxons}/dataset_report\n  method: get\n  operationId: getGenomeDatasetReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /genome/accession/{accessions}/dataset_report\n  method: get\n  operationId: getGenomeByAccession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gene/id/{gene_ids}\n  method: get\n  operationId: getGeneByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gene/symbol/{symbols}/taxon/{taxon}\n  method: get\n  operationId:\
  \ getGeneBySymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /taxonomy/taxon/{taxons}\n  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esearch.fcgi\n  method: get\n  operationId: searchDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /efetch.fcgi\n  method: get\n  operationId: fetchRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /esummary.fcgi\n  method: get\n  operationId: getSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /elink.fcgi\n  method: get\n  operationId: getLinkages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einfo.fcgi\n  method: get\n  operationId: getDatabaseInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espell.fcgi\n  method: get\n  operationId: checkSpelling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies\n  method: get\n  operationId: searchStudies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{nctId}\n  method: get\n  operationId: getStudy\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/size\n  method: get\n  operationId: getDatasetSize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/metadata\n  method: get\n  operationId: getStudyFieldsMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/agentic-access/united-states-national-library-of-medicine-agentic-access.yml
summary_line: 17 operations · 1 acting
tags:
- Federal Government
- Biomedical Research
- Healthcare
- Genomics
- Literature
---
