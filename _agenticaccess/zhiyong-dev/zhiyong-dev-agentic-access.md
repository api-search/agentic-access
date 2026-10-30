---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: zhiyong-dev-agent-api-openapi.yml
  format: yaml
  label: zhiyong-dev Agent API
  slug: zhiyong-dev-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-agent-api-openapi.yml
- filename: zhiyong-dev-agent-discovery-json-api-openapi.yml
  format: yaml
  label: zhiyong-dev Agent Discovery.json API
  slug: zhiyong-dev-agent-discovery-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-agent-discovery-json-api-openapi.yml
- filename: zhiyong-dev-agent-feedback-api-openapi.yml
  format: yaml
  label: zhiyong-dev Agent Feedback API
  slug: zhiyong-dev-agent-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-agent-feedback-api-openapi.yml
- filename: zhiyong-dev-agent-observation-api-openapi.yml
  format: yaml
  label: zhiyong-dev Agent Observation API
  slug: zhiyong-dev-agent-observation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-agent-observation-api-openapi.yml
- filename: zhiyong-dev-agent-task-api-openapi.yml
  format: yaml
  label: zhiyong-dev Agent Task API
  slug: zhiyong-dev-agent-task-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-agent-task-api-openapi.yml
- filename: zhiyong-dev-agent-topic-api-openapi.yml
  format: yaml
  label: zhiyong-dev Agent Topic API
  slug: zhiyong-dev-agent-topic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-agent-topic-api-openapi.yml
- filename: zhiyong-dev-community-api-openapi.yml
  format: yaml
  label: zhiyong-dev Community API
  slug: zhiyong-dev-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-community-api-openapi.yml
- filename: zhiyong-dev-entity-feedback-api-openapi.yml
  format: yaml
  label: zhiyong-dev Entity Feedback API
  slug: zhiyong-dev-entity-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-entity-feedback-api-openapi.yml
- filename: zhiyong-dev-health-api-openapi.yml
  format: yaml
  label: zhiyong-dev Health API
  slug: zhiyong-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-health-api-openapi.yml
- filename: zhiyong-dev-search-api-openapi.yml
  format: yaml
  label: zhiyong-dev Search API
  slug: zhiyong-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zhiyong-dev/openapi/zhiyong-dev-search-api-openapi.yml
consequence_counts:
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zhiyong Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'zhiyong-dev exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: zhiyong-dev
provider_slug: zhiyong-dev
slug: zhiyong-dev-agentic-access
source_filename: zhiyong-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/zhiyong-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 10\n    acting: 4\n  by_consequence:\n    read: 10\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /agent-discovery.json\n  method: get\n  operationId: getAgentDiscoveryPacket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method:\
  \ get\n  operationId: semanticSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent\n  method: get\n  operationId: agentDiscoveryOrSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent\n  method: post\n  operationId: agentSemanticSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-task\n  method: get\n  operationId: getAgentVerificationTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-observation\n  method: post\n  operationId: submitAgentObservation\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent-feedback\n  method: get\n  operationId: discoverOrCompatibilitySubmitAgentFeedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-feedback\n  method: post\n  operationId: submitAgentFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent-topic\n  method: post\n  operationId: createAgentTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/community/feed\n  method: get\n  operationId: listCommunityFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/entity-feedback\n  method: get\n  operationId: readCommunityThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/community/topics\n  method: get\n  operationId: listCommunityTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/community/topics\n  method: post\n  operationId: createHumanCommunityTopic\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/zhiyong-dev/agentic-access/zhiyong-dev-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Company
- Software
- DeveloperTools
- APIs
- Integration
---
