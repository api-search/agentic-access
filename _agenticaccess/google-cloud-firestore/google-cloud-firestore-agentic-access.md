---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: cloud-firestore-openapi.yml
  format: yaml
  label: Cloud Firestore API
  slug: cloud-firestore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-firestore/refs/heads/main/openapi/cloud-firestore-openapi.yml
consequence_counts:
  read: 4
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Firestore Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Google Cloud Firestore exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Firestore
provider_slug: google-cloud-firestore
slug: google-cloud-firestore-agentic-access
source_filename: google-cloud-firestore-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloud-firestore-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 4\n    acting: 6\n  by_consequence:\n    read: 4\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{project}/databases\n  method: get\n  operationId: listDatabases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/databases\n  method: post\n  operationId: createDatabase\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/databases/{database}\n  method: get\n  operationId: getDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/databases/{database}\n  method: delete\n  operationId: deleteDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/databases/{database}/documents/{collectionId}\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/databases/{database}/documents/{collectionId}\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/databases/{database}/documents/{collectionId}/{documentId}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project}/databases/{database}/documents/{collectionId}/{documentId}\n  method: patch\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /projects/{project}/databases/{database}/documents/{collectionId}/{documentId}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project}/databases/{database}/documents:runQuery\n  method: post\n  operationId: runQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/datastore\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-firestore/refs/heads/main/agentic-access/google-cloud-firestore-agentic-access.yml
summary_line: 10 operations · 6 acting
tags:
- Database
- Documents
- Google Cloud
- NoSQL
- Real-Time
---
