---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 9
api_specs:
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Agents API
  slug: contextual-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Agent Query API
  slug: contextual-ai-agent-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Datastores & Documents API
  slug: contextual-ai-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Generate API
  slug: contextual-ai-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Rerank API
  slug: contextual-ai-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Parse API
  slug: contextual-ai-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI LMUnit Evaluation API
  slug: contextual-ai-lmunit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
consequence_counts:
  read: 9
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Contextual Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Contextual AI exposes 25 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Contextual AI
provider_slug: contextual-ai
slug: contextual-ai-agentic-access
source_filename: contextual-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/contextual-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 16\n    connected: 9\n  by_consequence:\n    write: 16\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /agents\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}\n  method: get\n  operationId: getAgentMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}\n  method: patch\n  operationId: editAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agent_id}\n  method: delete\n  operationId: deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /agents/{agent_id}/query\n  method: post\n  operationId: queryAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agent_id}/feedback\n  method: post\n  operationId: provideFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datastores\n  method: post\n  operationId: createDatastore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /datastores\n  method: get\n  operationId: listDatastores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datastores/{datastore_id}\n  method: get\n  operationId: getDatastoreMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datastores/{datastore_id}\n  method: delete\n  operationId: deleteDatastore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datastores/{datastore_id}/documents\n  method: post\n  operationId: ingestDocument\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datastores/{datastore_id}/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datastores/{datastore_id}/documents/{document_id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generate\n  method: post\n  operationId: generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rerank\n  method: post\n  operationId: rerank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parse\n  method: post\n  operationId: parseFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parse/jobs/{job_id}/status\n  method: get\n  operationId: parseStatus\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parse/jobs/{job_id}/results\n  method: get\n  operationId: parseResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parse/jobs\n  method: get\n  operationId: parseListJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lmunit\n  method: post\n  operationId: lmunit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: delete\n  operationId: removeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/invite\n  method: post\n  operationId: inviteUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/agentic-access/contextual-ai-agentic-access.yml
summary_line: 25 operations · 16 acting
tags:
- AI
- RAG
- LLM
- Grounded Language Model
- Enterprise
---
