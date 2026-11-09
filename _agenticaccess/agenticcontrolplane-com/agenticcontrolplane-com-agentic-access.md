---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 14
api_specs:
- filename: agenticcontrolplane-com-agents-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Agents API
  slug: agenticcontrolplane-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-agents-api-openapi.yml
- filename: agenticcontrolplane-com-credentials-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Credentials API
  slug: agenticcontrolplane-com-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-credentials-api-openapi.yml
- filename: agenticcontrolplane-com-delegation-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Delegation API
  slug: agenticcontrolplane-com-delegation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-delegation-api-openapi.yml
- filename: agenticcontrolplane-com-introspect-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Introspect API
  slug: agenticcontrolplane-com-introspect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-introspect-api-openapi.yml
- filename: agenticcontrolplane-com-mcp-api-openapi.yml
  format: yaml
  label: Agentic Control Plane MCP API
  slug: agenticcontrolplane-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-mcp-api-openapi.yml
- filename: agenticcontrolplane-com-meta-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Meta API
  slug: agenticcontrolplane-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-meta-api-openapi.yml
- filename: agenticcontrolplane-com-proxy-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Proxy API
  slug: agenticcontrolplane-com-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-proxy-api-openapi.yml
- filename: agenticcontrolplane-com-runs-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Runs API
  slug: agenticcontrolplane-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-runs-api-openapi.yml
- filename: agenticcontrolplane-com-sandbox-api-openapi.yml
  format: yaml
  label: Agentic Control Plane Sandbox API
  slug: agenticcontrolplane-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticcontrolplane-com/openapi/agenticcontrolplane-com-sandbox-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Agenticcontrolplane Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/scoped-tokens/{tokenId}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/sandbox-tenants
operation_count: 27
overview: 'Agentic Control Plane exposes 27 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 11 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentic Control Plane
provider_slug: agenticcontrolplane-com
slug: agenticcontrolplane-com-agentic-access
source_filename: agenticcontrolplane-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agenticcontrolplane-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 13\n    connected: 14\n  by_consequence:\n    write: 11\n    read: 14\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/agents\n  method: post\n  operationId: createAgentProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents\n  method: get\n  operationId: listAgentProfiles\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{id}\n  method: get\n  operationId: getAgentProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{id}\n  method: put\n  operationId: replaceAgentProfileFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{id}\n  method: patch\n  operationId: patchAgentProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{id}\n  method: delete\n  operationId: deleteAgentProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{id}/run\n  method: post\n  operationId: runAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/runs\n  method: get\n  operationId: listRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/runs/{runKey}\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/introspect/usage\n  method: get\n  operationId: introspectUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/introspect/cost\n  method: get\n  operationId: introspectCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/introspect/decisions\n  method: get\n  operationId: introspectDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/introspect/trace/{sessionId}\n  method: get\n  operationId: introspectTrace\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/introspect/agents\n  method: get\n  operationId: introspectAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/introspect/recommendations\n  method: get\n  operationId: introspectRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/introspect/cost-insights\n  method: get\n  operationId: introspectCostInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys/child\n  method: post\n  operationId: mintChildKey\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scoped-tokens\n  method: post\n  operationId: issueScopedToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scoped-tokens/{tokenId}/revoke\n  method: post\n  operationId: revokeScopedToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sandbox-tenants\n\
  \  method: post\n  operationId: createSandboxTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: proxyChatCompletions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: proxyListModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /anthropic/v1/messages\n  method:\
  \ post\n  operationId: proxyAnthropicMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/responses\n  method: post\n  operationId: proxyOpenAiResponses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /status.json\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agenticcontrolplane-com/agentic-access/agenticcontrolplane-com-agentic-access.yml
summary_line: 27 operations · 13 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Agents
- Control Plane
- Tool Management
- Monitoring
---
