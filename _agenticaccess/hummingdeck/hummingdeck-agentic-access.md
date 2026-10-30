---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 16
api_specs:
- filename: hummingdeck-companies-api-openapi.yml
  format: yaml
  label: HummingDeck Companies API
  slug: hummingdeck-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-companies-api-openapi.yml
- filename: hummingdeck-contacts-api-openapi.yml
  format: yaml
  label: HummingDeck Contacts API
  slug: hummingdeck-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-contacts-api-openapi.yml
- filename: hummingdeck-decisions-api-openapi.yml
  format: yaml
  label: HummingDeck Decisions API
  slug: hummingdeck-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-decisions-api-openapi.yml
- filename: hummingdeck-decks-api-openapi.yml
  format: yaml
  label: HummingDeck Decks API
  slug: hummingdeck-decks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-decks-api-openapi.yml
- filename: hummingdeck-emails-api-openapi.yml
  format: yaml
  label: HummingDeck Emails API
  slug: hummingdeck-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-emails-api-openapi.yml
- filename: hummingdeck-hooks-api-openapi.yml
  format: yaml
  label: HummingDeck Hooks API
  slug: hummingdeck-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-hooks-api-openapi.yml
- filename: hummingdeck-me-api-openapi.yml
  format: yaml
  label: HummingDeck Me API
  slug: hummingdeck-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-me-api-openapi.yml
- filename: hummingdeck-room-labels-api-openapi.yml
  format: yaml
  label: HummingDeck Room Labels API
  slug: hummingdeck-room-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-room-labels-api-openapi.yml
- filename: hummingdeck-room-views-api-openapi.yml
  format: yaml
  label: HummingDeck Room Views API
  slug: hummingdeck-room-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-room-views-api-openapi.yml
- filename: hummingdeck-rooms-api-openapi.yml
  format: yaml
  label: HummingDeck Rooms API
  slug: hummingdeck-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-rooms-api-openapi.yml
- filename: hummingdeck-shares-api-openapi.yml
  format: yaml
  label: HummingDeck Shares API
  slug: hummingdeck-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-shares-api-openapi.yml
- filename: hummingdeck-views-api-openapi.yml
  format: yaml
  label: HummingDeck Views API
  slug: hummingdeck-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-views-api-openapi.yml
consequence_counts:
  physical: 2
  read: 16
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hummingdeck Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /rooms/{roomId}/items/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /rooms/{roomId}/tabs/order
operation_count: 48
overview: 'HummingDeck exposes 48 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 30 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HummingDeck
provider_slug: hummingdeck
slug: hummingdeck-agentic-access
source_filename: hummingdeck-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: generated\nsource: openapi/hummingdeck-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 16\n    acting: 32\n  by_consequence:\n    read: 16\n    write: 30\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hooks\n  method: post\n  operationId: subscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hooks/{id}\n  method: delete\n  operationId: unsubscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /views\n  method: get\n  operationId: listViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shares\n  method: post\n  operationId: createShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms\n\
  \  method: get\n  operationId: listRooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms\n  method: post\n  operationId: createRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}\n  method: get\n  operationId: getRoom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/{roomId}\n  method: patch\n  operationId: updateRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/links\n  method: get\n  operationId: listRoomLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/{roomId}/links\n  method: post\n  operationId: createRoomLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/links/{linkId}\n  method: patch\n  operationId: updateRoomLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /rooms/{roomId}/archive\n  method: post\n  operationId: archiveRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/restore\n  method: post\n  operationId: restoreRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/tabs\n  method: post\n  operationId: createRoomTab\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/tabs/order\n  method: put\n  operationId: reorderRoomTabs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/tabs/{tabId}\n  method: patch\n  operationId: renameRoomTab\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/tabs/{tabId}\n  method: delete\n  operationId: deleteRoomTab\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/items\n  method: post\n  operationId: addRoomItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/items/order\n  method: put\n  operationId: reorderRoomItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/items/{itemId}\n\
  \  method: delete\n  operationId: removeRoomItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/items/{itemId}/move\n  method: post\n  operationId: moveRoomItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/action-plan\n  method: get\n  operationId: getRoomActionPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/{roomId}/action-plan\n  method: patch\n  operationId: updateRoomActionPlan\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/action-plan/phases\n  method: post\n  operationId: createRoomActionPlanPhase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/action-plan/phases/{phaseId}\n  method: patch\n  operationId: updateRoomActionPlanPhase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /rooms/{roomId}/action-plan/phases/{phaseId}\n  method: delete\n  operationId: deleteRoomActionPlanPhase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/action-plan/tasks\n  method: post\n  operationId: createRoomActionPlanTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/action-plan/tasks/{taskId}\n  method: patch\n  operationId: updateRoomActionPlanTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/action-plan/tasks/{taskId}\n  method: delete\n  operationId: deleteRoomActionPlanTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/action-plan/tasks/{taskId}/status\n  method: post\n  operationId: setRoomActionPlanTaskStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rooms/{roomId}/analytics\n\
  \  method: get\n  operationId: getRoomAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/{roomId}/activity\n  method: get\n  operationId: listRoomActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rooms/{roomId}/captured-emails\n  method: get\n  operationId: listRoomCapturedEmails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /room-views\n  method: get\n  operationId: listRoomViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /room-labels\n  method: get\n  operationId: listRoomLabels\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /room-labels\n  method: post\n  operationId: createRoomLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /room-labels/{labelId}\n  method: patch\n  operationId: updateRoomLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /room-labels/{labelId}\n  method: delete\n  operationId: deleteRoomLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decks\n  method: get\n  operationId: searchDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /decks\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decks/{deckId}/replace\n  method: post\n  operationId: replaceDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /decisions\n  method: get\n  operationId: listDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails\n  method: get\n  operationId: listEmailCaptures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies\n  method: get\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies\n  method: post\n  operationId: findOrCreateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /contacts\n  method: get\n  operationId: searchContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: findOrCreateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/agentic-access/hummingdeck-agentic-access.yml
summary_line: 48 operations · 32 acting
tags:
- Document Sharing
- Engagement Analytics
- Digital Sales Rooms
- Data Rooms
- Client Portals
- Integrations
- Secure Sharing
---
