---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 10
api_specs:
- filename: brainfish-agents-api-openapi.yml
  format: yaml
  label: Brainfish Agents API
  slug: brainfish-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-agents-api-openapi.yml
- filename: brainfish-analytics-api-openapi.yml
  format: yaml
  label: Brainfish Analytics API
  slug: brainfish-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-analytics-api-openapi.yml
- filename: brainfish-authentication-api-openapi.yml
  format: yaml
  label: Brainfish Authentication API
  slug: brainfish-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-authentication-api-openapi.yml
- filename: brainfish-catalogs-api-openapi.yml
  format: yaml
  label: Brainfish Catalogs API
  slug: brainfish-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-catalogs-api-openapi.yml
- filename: brainfish-collections-api-openapi.yml
  format: yaml
  label: Brainfish Collections API
  slug: brainfish-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-collections-api-openapi.yml
- filename: brainfish-conversations-api-openapi.yml
  format: yaml
  label: Brainfish Conversations API
  slug: brainfish-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-conversations-api-openapi.yml
- filename: brainfish-documents-api-openapi.yml
  format: yaml
  label: Brainfish Documents API
  slug: brainfish-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-documents-api-openapi.yml
- filename: brainfish-sessions-api-openapi.yml
  format: yaml
  label: Brainfish Sessions API
  slug: brainfish-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-sessions-api-openapi.yml
- filename: brainfish-users-api-openapi.yml
  format: yaml
  label: Brainfish Users API
  slug: brainfish-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/openapi/brainfish-users-api-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Brainfish Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/revoke
operation_count: 27
overview: 'Brainfish exposes 27 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 16 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Brainfish
provider_slug: brainfish
slug: brainfish-agentic-access
source_filename: brainfish-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/brainfish-agents-api-openapi.yml, openapi/brainfish-analytics-api-openapi.yml,\n  openapi/brainfish-authentication-api-openapi.yml, openapi/brainfish-catalogs-api-openapi.yml,\n  openapi/brainfish-collections-api-openapi.yml, openapi/brainfish-conversations-api-openapi.yml,\n  openapi/brainfish-documents-api-openapi.yml, openapi/brainfish-sessions-api-openapi.yml, openapi/brainfish-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 17\n    connected: 10\n  by_consequence:\n    write: 16\n    read: 10\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/agents/answer\n  method: post\n  operationId: generateAnswer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analytics/threads\n  method: post\n  operationId: listAnalyticsThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/validate\n  method: post\n  operationId: validateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/revoke\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/catalogs\n  method: get\n  operationId: listCatalogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs\n  method: post\n  operationId: createCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalogs/{id}\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/catalogs/{id}/content\n  method: post\n  operationId: syncCatalogContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/collections/{id}\n  method: get\n  operationId:\
  \ getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections/{id}\n  method: put\n  operationId: updateCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/collections/{id}\n  method: delete\n  operationId: deleteCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conversations/{conversationId}/follow-ups\n  method: post\n  operationId: generateFollowUpQuestions\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /v1/documents/{id}\n  method: put\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}/move\n  method: post\n  operationId: moveDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/search\n  method: post\n  operationId: searchDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/suggestion\n  method: post\n  operationId: generateArticleSuggestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/search\n  method: post\n  operationId: searchSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /v1/sessions/{id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{id}/timeline\n  method: get\n  operationId: getSessionTimeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{id}/insights\n  method: post\n  operationId: generateSessionInsights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/answer\n  method: post\n  operationId: generateUserAnswer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainfish/refs/heads/main/agentic-access/brainfish-agentic-access.yml
summary_line: 27 operations · 17 acting · 1 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Customer Support
- Knowledge Base
- Help Desk
- Agents
- Support Automation
- Software-as-a-Service
---
