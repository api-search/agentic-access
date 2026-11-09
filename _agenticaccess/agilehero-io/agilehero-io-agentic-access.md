---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 16
api_specs:
- filename: agilehero-io-account-api-openapi.yml
  format: yaml
  label: AgileHero Account API
  slug: agilehero-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-account-api-openapi.yml
- filename: agilehero-io-cards-api-openapi.yml
  format: yaml
  label: AgileHero Cards API
  slug: agilehero-io-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-cards-api-openapi.yml
- filename: agilehero-io-discovery-api-openapi.yml
  format: yaml
  label: AgileHero Discovery API
  slug: agilehero-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-discovery-api-openapi.yml
- filename: agilehero-io-projects-api-openapi.yml
  format: yaml
  label: AgileHero Projects API
  slug: agilehero-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-projects-api-openapi.yml
- filename: agilehero-io-webhooks-api-openapi.yml
  format: yaml
  label: AgileHero Webhooks API
  slug: agilehero-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 16
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agilehero Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/cards/{card_id}/move
operation_count: 40
overview: 'AgileHero exposes 40 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 23 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgileHero
provider_slug: agilehero-io
slug: agilehero-io-agentic-access
source_filename: agilehero-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agilehero-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 16\n    acting: 24\n  by_consequence:\n    read: 16\n    write: 23\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v0/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - api:read\n- path: /v0/workspaces/{workspace_id}/members\n  method: get\n  operationId: listWorkspaceMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/workspaces/{workspace_id}/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/projects/{project_id}/lists\n  method: get\n  operationId: listLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/projects/{project_id}/lists\n  method: post\n  operationId: createList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/lists/{list_id}\n  method: patch\n  operationId: updateList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/lists/{list_id}\n  method: delete\n  operationId: deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v0/projects/{project_id}/labels\n  method: get\n  operationId: listLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/projects/{project_id}/labels\n  method: post\n  operationId: createLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labels/{label_id}\n  method: patch\n  operationId: updateLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v0/labels/{label_id}\n  method: delete\n  operationId: deleteLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/projects/{project_id}/epics\n  method: get\n  operationId: listEpics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/epics/{epic_id}\n  method: get\n  operationId: getEpic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/projects/{project_id}/cards\n \
  \ method: get\n  operationId: listCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/projects/{project_id}/cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/cards/{card_id}\n  method: patch\n  operationId: updateCard\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}\n  method: delete\n  operationId: deleteCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}/move\n  method: post\n  operationId: moveCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}/labels\n  method: post\n  operationId: addCardLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}/labels/{label_id}\n  method: delete\n  operationId: removeCardLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}/assignees\n  method: post\n  operationId:\
  \ addCardAssignee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}/assignees/{user_id}\n  method: delete\n  operationId: removeCardAssignee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}/relations\n  method: get\n  operationId: listCardRelations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - api:read\n- path: /v0/cards/{card_id}/relations\n  method: post\n  operationId: createCardRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}/relations/{relation_id}\n  method: delete\n  operationId: deleteCardRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}/checklists\n  method: get\n  operationId: listCardChecklists\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/cards/{card_id}/checklists\n  method: post\n  operationId: createCardChecklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/checklists/{checklist_id}\n  method: delete\n  operationId: deleteChecklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/checklists/{checklist_id}/items\n  method:\
  \ post\n  operationId: createChecklistItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/checklist_items/{item_id}\n  method: patch\n  operationId: updateChecklistItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/checklist_items/{item_id}\n  method: delete\n  operationId: deleteChecklistItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    -\
  \ api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/cards/{card_id}/comments\n  method: get\n  operationId: listCardComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/cards/{card_id}/comments\n  method: post\n  operationId: createCardComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/webhook_endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/webhook_endpoints\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/webhook_endpoints/sample\n  method: get\n  operationId: sampleWebhookEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n- path: /v0/webhook_endpoints/{webhook_endpoint_id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  scope:\n    - api:read\n    - api:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: getProtectedResourceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api:read\n"
source_yaml_url: https://artifacts.apis.io/agilehero-io/agentic-access/agilehero-io-agentic-access.yml
summary_line: 40 operations · 24 acting
tags:
- Company
- Project Management
- Agile
- AI Integration
- Collaboration
---
