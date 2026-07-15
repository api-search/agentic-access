---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 11
api_specs:
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Datasets API
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Items & Upload API
  slug: items-upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Annotations API
  slug: annotations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Workflows & Stages API
  slug: workflows-stages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Annotation Classes API
  slug: classes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
- filename: v7-labs-openapi.yml
  format: yaml
  label: V7 Darwin Exports API
  slug: exports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/openapi/v7-labs-openapi.yml
consequence_counts:
  read: 11
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: V7 Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'V7 exposes 25 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: V7
provider_slug: v7-labs
slug: v7-labs-agentic-access
source_filename: v7-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/v7-labs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 11\n    acting: 14\n  by_consequence:\n    read: 11\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{id}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/items\n  method: get\n  operationId: listItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/items\n  method: delete\n  operationId: deleteItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/items/{item_id}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/items/register_upload\n  method: post\n  operationId: registerUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/items/uploads/{upload_id}/sign\n  method: get\n  operationId: signUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/items/uploads/{upload_id}/confirm\n  method: post\n  operationId: confirmUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/items/register_existing\n  method: post\n  operationId: registerExisting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/items/register_existing_readonly\n  method: post\n  operationId: registerExistingReadonly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/items/archive\n  method: post\n  operationId: archiveItems\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/items/restore\n  method: post\n  operationId: restoreItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/items/{item_id}/annotations\n  method: get\n  operationId: listItemAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/items/{item_id}/import\n  method: post\n  operationId: importAnnotations\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/annotation_classes\n  method: get\n  operationId: listAnnotationClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/annotation_classes/{class_id}\n  method: put\n  operationId: updateAnnotationClass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/workflows\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/workflows\n  method: post\n  operationId: createWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/workflows/{id}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/items/stage\n  method: post\n  operationId: setStage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/datasets/{dataset_slug}/exports\n  method: get\n  operationId: listExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/datasets/{dataset_slug}/exports\n  method: post\n  operationId: createExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/teams/{team_slug}/datasets/{dataset_slug}/exports/{name}\n  method: get\n  operationId: showExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams/{team_slug}/datasets/{dataset_slug}/exports/{name}\n\
  \  method: delete\n  operationId: deleteExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/v7-labs/refs/heads/main/agentic-access/v7-labs-agentic-access.yml
summary_line: 25 operations · 14 acting
tags:
- AI
- Training Data
- Data Labeling
- Annotation
- Document AI
- Computer Vision
---
