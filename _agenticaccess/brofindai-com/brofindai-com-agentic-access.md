---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: brofindai-com-agents-api-openapi.yml
  format: yaml
  label: Bro Find AI Agents API
  slug: brofindai-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-agents-api-openapi.yml
- filename: brofindai-com-badge-api-openapi.yml
  format: yaml
  label: Bro Find AI Badge API
  slug: brofindai-com-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-badge-api-openapi.yml
- filename: brofindai-com-comments-api-openapi.yml
  format: yaml
  label: Bro Find AI Comments API
  slug: brofindai-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-comments-api-openapi.yml
- filename: brofindai-com-feedback-api-openapi.yml
  format: yaml
  label: Bro Find AI Feedback API
  slug: brofindai-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-feedback-api-openapi.yml
- filename: brofindai-com-mcp-servers-api-openapi.yml
  format: yaml
  label: Bro Find AI MCP Servers API
  slug: brofindai-com-mcp-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-mcp-servers-api-openapi.yml
- filename: brofindai-com-reviews-api-openapi.yml
  format: yaml
  label: Bro Find AI Reviews API
  slug: brofindai-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-reviews-api-openapi.yml
- filename: brofindai-com-search-api-openapi.yml
  format: yaml
  label: Bro Find AI Search API
  slug: brofindai-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-search-api-openapi.yml
- filename: brofindai-com-tools-api-openapi.yml
  format: yaml
  label: Bro Find AI Tools API
  slug: brofindai-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brofindai-com/openapi/brofindai-com-tools-api-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Brofindai Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Bro Find AI exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bro Find AI
provider_slug: brofindai-com
slug: brofindai-com-agentic-access
source_filename: brofindai-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/brofindai-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 6\n    connected: 8\n  by_consequence:\n    write: 6\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/submit\n  method: post\n  operationId: submitTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/submit-agent\n  method: post\n  operationId: submitAgent\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/submit-mcp\n  method: post\n  operationId: submitMcpServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reviews\n  method: get\n  operationId: getReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reviews\n  method: post\n  operationId: createReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/comments\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/comments\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/feedback\n  method: post\n  operationId: submitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/search-tools\n  method: get\n  operationId: searchTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search-agents\n  method: get\n  operationId: searchAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search-mcp\n  method: get\n  operationId: searchMcpServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/badge/{toolId}/votes.json\n  method: get\n  operationId: getBadgeVotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/badge/votes.json\n  method: get\n  operationId: getBadgeVotesByMaker\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/badge/{toolId}.svg\n  method: get\n  operationId: getBadgeSvg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/brofindai-com/agentic-access/brofindai-com-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Artificial Intelligence
- Directory
- Tools
- Marketplace
- Company
---
