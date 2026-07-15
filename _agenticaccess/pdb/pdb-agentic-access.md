---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 18
api_specs:
- filename: rcsb-pdb-search-api.json
  format: json
  label: RCSB PDB Search API
  slug: rcsb-pdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/rcsb-pdb-search-api.json
- filename: rcsb-pdb-model-server-api.json
  format: json
  label: RCSB PDB ModelServer API
  slug: rcsb-pdb-model-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/rcsb-pdb-model-server-api.json
- filename: rcsb-pdb-volume-server-api.json
  format: json
  label: RCSB PDB VolumeServer API
  slug: rcsb-pdb-volume-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/openapi/rcsb-pdb-volume-server-api.json
consequence_counts:
  read: 18
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pdb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'RCSB PDB exposes 28 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RCSB PDB
provider_slug: pdb
slug: pdb-agentic-access
source_filename: pdb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/rcsb-pdb-model-server-api.json, openapi/rcsb-pdb-search-api.json, openapi/rcsb-pdb-volume-server-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 18\n    acting: 10\n  by_consequence:\n    read: 18\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/{id}/assembly\n  method: get\n  operationId: assembly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{id}/assembly\n  method: post\n  operationId: assembly-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{id}/atoms\n  method: get\n  operationId: atoms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{id}/atoms\n  method: post\n  operationId: atoms-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{id}/full\n  method: get\n  operationId: full\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{id}/full\n  method: post\n  operationId: full-post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{id}/ligand\n  method: get\n  operationId: ligand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{id}/ligand\n  method: post\n  operationId: ligand-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{id}/residueInteraction\n  method: get\n  operationId: residueInteraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{id}/residueInteraction\n  method: post\n  operationId: residueInteraction-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{id}/residueSurroundings\n  method: get\n  operationId: residueSurroundings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{id}/residueSurroundings\n  method: post\n  operationId: residueSurroundings-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /v1/{id}/surroundingLigands\n  method: get\n  operationId: surroundingLigands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{id}/surroundingLigands\n  method: post\n  operationId: surroundingLigands-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{id}/symmetryMates\n  method: get\n  operationId: symmetryMates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{id}/symmetryMates\n  method: post\n  operationId: symmetryMates-post\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/query-many\n  method: get\n  operationId: query-many\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/query-many\n  method: post\n  operationId: query-many-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcsbsearch/v2/query\n  method: get\n  operationId: runJsonQueriesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /rcsbsearch/v2/query\n  method: post\n  operationId: runJsonQueriesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcsbsearch/v2/suggest\n  method: get\n  operationId: getSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcsbsearch/v2/query/unreleased\n  method: get\n  operationId: runUnreleasedEntryJsonQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcsbsearch/v2/metadata/unreleased/schema\n  method: get\n  operationId: getUnreleasedEntryMetadata\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcsbsearch/v2/metadata/schema\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcsbsearch/v2/metadata/chemical/schema\n  method: get\n  operationId: getChemicalMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{source}/{id}/\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{source}/{id}/box/{a1,a2,a3}/{b1,b2,b3}/\n  method: get\n  operationId: getBox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /{source}/{id}/cell/\n  method: get\n  operationId: getCell\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdb/refs/heads/main/agentic-access/pdb-agentic-access.yml
summary_line: 28 operations · 10 acting
tags:
- Structural Biology
- Proteomics
- Bioinformatics
- Genomics
- Life Sciences
- Open Data
- Research
- Macromolecules
- Crystallography
- NMR
---
