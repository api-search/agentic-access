---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 9
api_specs:
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Document Parse API
  slug: tensorlake-document-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Structured Extraction API
  slug: tensorlake-structured-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Files API
  slug: tensorlake-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Datasets API
  slug: tensorlake-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
- filename: tensorlake-openapi.yml
  format: yaml
  label: Tensorlake Sandboxes API
  slug: tensorlake-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/openapi/tensorlake-openapi.yml
consequence_counts:
  read: 9
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tensorlake Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Tensorlake exposes 27 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tensorlake
provider_slug: tensorlake
slug: tensorlake-agentic-access
source_filename: tensorlake-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tensorlake-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 18\n    connected: 9\n  by_consequence:\n    write: 18\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /documents/v2/parse\n  method: post\n  operationId: post_parse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/parse\n  method: get\n  operationId: list_parse\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/v2/parse/{parse_id}\n  method: get\n  operationId: get_parse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/v2/parse/{parse_id}\n  method: delete\n  operationId: delete_parse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/extract\n  method: post\n  operationId: post_extract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /documents/v2/classify\n  method: post\n  operationId: post_classify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/read\n  method: post\n  operationId: post_read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/edit\n  method: post\n  operationId: post_edit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/files\n  method: put\n  operationId: put_file_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/files\n  method: get\n  operationId: list_files_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/v2/files/{file_id}\n  method: delete\n  operationId: delete_file_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /documents/v2/files/{file_id}/metadata\n  method: get\n  operationId: get_file_metadata_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/v2/datasets\n  method: post\n  operationId: create_dataset_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/datasets\n  method: get\n  operationId: list_datasets_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/v2/datasets/{dataset_id}\n  method: get\n  operationId: get_dataset_v2\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/v2/datasets/{dataset_id}\n  method: put\n  operationId: update_dataset_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/datasets/{dataset_id}\n  method: delete\n  operationId: delete_dataset_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/datasets/{dataset_id}/data\n  method: get\n  operationId: get_dataset_data_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/v2/datasets/{dataset_id}/parse\n  method: post\n  operationId: parse_dataset_file_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandboxes\n  method: post\n  operationId: create_sandbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandboxes\n  method: get\n  operationId: list_sandboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /sandboxes/{sandbox_id}\n  method: get\n  operationId: get_sandbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sandboxes/{sandbox_id}\n  method: patch\n  operationId: update_sandbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandboxes/{sandbox_id}\n  method: delete\n  operationId: delete_sandbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandboxes/{sandbox_id}/snapshot\n  method: post\n\
  \  operationId: snapshot_sandbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandboxes/{sandbox_id}/suspend\n  method: post\n  operationId: suspend_sandbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandboxes/{sandbox_id}/resume\n  method: post\n  operationId: resume_sandbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensorlake/refs/heads/main/agentic-access/tensorlake-agentic-access.yml
summary_line: 27 operations · 18 acting
tags:
- Document Extraction
- Data Extraction
- Document Ingestion
- Document Parsing
- OCR
- Data Ingestion
- AI
- Unstructured Data
- Document AI
- RAG
---
