---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 11
api_specs:
- filename: scispot-openapi.yml
  format: yaml
  label: Scispot API
  slug: scispot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/openapi/scispot-openapi.yml
consequence_counts:
  read: 11
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scispot Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Scispot exposes 18 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scispot
provider_slug: scispot
slug: scispot-agentic-access
source_filename: scispot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/scispot-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 11\n    acting: 7\n  by_consequence:\n    read: 11\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /labsheets\n  method: get\n  operationId: listLabsheets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labsheets/{labsheetId}/rows\n  method: get\n  operationId: getLabsheetRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labsheets/{labsheetId}/rows\n\
  \  method: post\n  operationId: addLabsheetRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labsheets/{labsheetId}/rows/{rowId}\n  method: get\n  operationId: getLabsheetRow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labsheets/{labsheetId}/rows/{rowId}\n  method: put\n  operationId: updateLabsheetRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labsheets/{labsheetId}/rows/{rowId}\n  method: delete\n\
  \  operationId: deleteLabsheetRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /results/search/{barcode}\n  method: get\n  operationId: searchResultsByBarcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/search/sample/{sampleId}\n  method: get\n  operationId: searchResultsBySampleId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eln/notebooks\n  method: get\n  operationId: listNotebooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /eln/notebooks/{notebookId}/entries\n  method: get\n  operationId: listNotebookEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eln/notebooks/{notebookId}/entries\n  method: post\n  operationId: createNotebookEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manifests\n  method: get\n  operationId: listManifests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manifests\n  method: post\n  operationId: createManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manifests/{manifestId}\n  method: get\n  operationId: getManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences\n  method: get\n  operationId: listSequences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences\n  method: post\n  operationId: createSequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/{sequenceId}\n  method:\
  \ get\n  operationId: getSequence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/{sequenceId}\n  method: put\n  operationId: updateSequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/agentic-access/scispot-agentic-access.yml
summary_line: 18 operations · 7 acting
tags:
- Laboratory
- Life Science
- LIMS
- ELN
- Biotech
- API First
- Scientific Data
- Healthcare
---
