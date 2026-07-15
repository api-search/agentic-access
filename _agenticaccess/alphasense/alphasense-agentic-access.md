---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: alphasense-agent-api-openapi.yml
  format: yaml
  label: AlphaSense Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-agent-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Ingestion API
  slug: ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Companies API
  slug: companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Brokers API
  slug: brokers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-utility-api-openapi.yml
  format: yaml
  label: AlphaSense Watchlist API
  slug: watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-utility-api-openapi.yml
- filename: alphasense-agent-api-openapi.yml
  format: yaml
  label: AlphaSense Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/openapi/alphasense-agent-api-openapi.yml
consequence_counts:
  read: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Alphasense Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'AlphaSense exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AlphaSense
provider_slug: alphasense
slug: alphasense-agentic-access
source_filename: alphasense-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/alphasense-agent-api-openapi.yml, openapi/alphasense-utility-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 4\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /auth\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gql\n  method: post\n  operationId: graphqlGateway\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gql\n  method: post\n  operationId: utilityGraphqlGateway\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/i/ingestion-api/v1/documents\n  method: post\n  operationId: ingestDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/i/ingestion-api/v1/jobs/{jobId}\n\
  \  method: get\n  operationId: getIngestionJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphasense/refs/heads/main/agentic-access/alphasense-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- Market Intelligence
- Financial Research
- Search
- Generative AI
- AI Agents
- Expert Calls
- Document Intelligence
- Enterprise Intelligence
- MCP
- GraphQL
---
