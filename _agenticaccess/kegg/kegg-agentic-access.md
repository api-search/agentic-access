---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: kegg-rest-api.yml
  format: yaml
  label: KEGG REST API
  slug: kegg-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/openapi/kegg-rest-api.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kegg Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Kyoto Encyclopedia of Genes and Genomes (KEGG) exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kyoto Encyclopedia of Genes and Genomes (KEGG)
provider_slug: kegg
slug: kegg-agentic-access
source_filename: kegg-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kegg-rest-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /info/{database}\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list/{database}\n  method: get\n  operationId: listDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list/pathway/{org}\n  method: get\n  operationId: listPathwaysByOrganism\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /find/{database}/{query}\n  method: get\n  operationId: findEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /find/{database}/{query}/{option}\n  method: get\n  operationId: findEntriesWithOption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get/{dbentries}\n  method: get\n  operationId: getEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get/{dbentries}/{option}\n  method: get\n  operationId: getEntriesWithOption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /conv/{target_db}/{source_db}\n  method: get\n  operationId: convertIdentifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conv/{target_db}/{dbentries}\n  method: get\n  operationId: convertEntryIdentifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/{target_db}/{source_db}\n  method: get\n  operationId: linkDatabases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/{target_db}/{dbentries}\n  method: get\n  operationId: linkEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ddi/{dbentry}\n\
  \  method: get\n  operationId: getDrugInteraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ddi/{dbentries}\n  method: get\n  operationId: getDrugInteractions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/agentic-access/kegg-agentic-access.yml
summary_line: 13 operations
tags:
- Bioinformatics
- Genomics
- Life Sciences
- Pathways
- Metabolomics
- Drug Targets
- Disease
- Chemical Compounds
- Enzymes
- Orthology
---
