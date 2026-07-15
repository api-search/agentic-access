---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 11
api_specs:
- filename: filevine-identity-api-openapi.yml
  format: yaml
  label: Filevine Identity API
  slug: filevine-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-identity-api-openapi.yml
- filename: filevine-projects-api-openapi.yml
  format: yaml
  label: Filevine Projects API
  slug: filevine-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-projects-api-openapi.yml
- filename: filevine-contacts-api-openapi.yml
  format: yaml
  label: Filevine Contacts API
  slug: filevine-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-contacts-api-openapi.yml
- filename: filevine-documents-api-openapi.yml
  format: yaml
  label: Filevine Documents API
  slug: filevine-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-documents-api-openapi.yml
- filename: filevine-notes-api-openapi.yml
  format: yaml
  label: Filevine Notes API
  slug: filevine-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-notes-api-openapi.yml
- filename: filevine-deadlines-api-openapi.yml
  format: yaml
  label: Filevine Deadlines API
  slug: filevine-deadlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-deadlines-api-openapi.yml
- filename: filevine-tasks-api-openapi.yml
  format: yaml
  label: Filevine Tasks API
  slug: filevine-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-tasks-api-openapi.yml
- filename: filevine-time-entries-api-openapi.yml
  format: yaml
  label: Filevine Time Entries API
  slug: filevine-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-time-entries-api-openapi.yml
- filename: filevine-webhooks-api-openapi.yml
  format: yaml
  label: Filevine Webhooks API
  slug: filevine-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/openapi/filevine-webhooks-api-openapi.yml
consequence_counts:
  read: 11
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Filevine Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Filevine exposes 25 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Filevine
provider_slug: filevine
slug: filevine-agentic-access
source_filename: filevine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/filevine-contacts-api-openapi.yml, openapi/filevine-deadlines-api-openapi.yml,\n  openapi/filevine-documents-api-openapi.yml, openapi/filevine-identity-api-openapi.yml, openapi/filevine-notes-api-openapi.yml,\n  openapi/filevine-projects-api-openapi.yml, openapi/filevine-tasks-api-openapi.yml, openapi/filevine-time-entries-api-openapi.yml,\n  openapi/filevine-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 11\n    acting: 14\n  by_consequence:\n    read: 11\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /core/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/contacts/{contactId}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/projects/{projectId}/contacts\n  method: post\n  operationId: attachProjectContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /core/projects/{projectId}/deadlines\n  method: get\n  operationId: listProjectDeadlines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/projects/{projectId}/deadlines\n  method: post\n  operationId: createDeadline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/projects/{projectId}/documents\n  method: get\n  operationId: listProjectDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/projects/{projectId}/documents\n  method: post\n  operationId: uploadProjectDocument\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/documents/{documentId}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/projects/{projectId}/notes\n  method: get\n  operationId: listProjectNotes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/projects/{projectId}/notes\n  method: post\n  operationId: createNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/notes/{noteId}\n  method: patch\n  operationId: updateNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /core/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/projects/{projectId}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/projects/{projectId}\n  method: patch\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/projects/{projectId}/tasks\n  method: get\n  operationId:\
  \ listProjectTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/projects/{projectId}/tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/tasks/{taskId}\n  method: patch\n  operationId: updateTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/time-entries\n  method: get\n  operationId: listTimeEntries\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/time-entries\n  method: post\n  operationId: createTimeEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/webhooks/subscriptions\n  method: get\n  operationId: listWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/webhooks/subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /core/webhooks/subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filevine/refs/heads/main/agentic-access/filevine-agentic-access.yml
summary_line: 25 operations · 14 acting
tags:
- Legal
- Case Management
- Matters
- Intake
- Documents
- LOIS
- Webhooks
- Legal AI
- Personal Injury
- Mass Torts
---
