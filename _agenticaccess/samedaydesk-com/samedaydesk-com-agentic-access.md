---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 13
api_specs:
- filename: samedaydesk-com-agent-readiness-api-openapi.yml
  format: yaml
  label: samedaydesk-com Agent Readiness API
  slug: samedaydesk-com-agent-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-agent-readiness-api-openapi.yml
- filename: samedaydesk-com-correspondence-api-openapi.yml
  format: yaml
  label: samedaydesk-com Correspondence API
  slug: samedaydesk-com-correspondence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-correspondence-api-openapi.yml
- filename: samedaydesk-com-funnel-evidence-api-openapi.yml
  format: yaml
  label: samedaydesk-com Funnel Evidence API
  slug: samedaydesk-com-funnel-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-funnel-evidence-api-openapi.yml
- filename: samedaydesk-com-health-api-openapi.yml
  format: yaml
  label: samedaydesk-com Health API
  slug: samedaydesk-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-health-api-openapi.yml
- filename: samedaydesk-com-hosted-useful-api-openapi.yml
  format: yaml
  label: samedaydesk-com Hosted Useful API
  slug: samedaydesk-com-hosted-useful-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-hosted-useful-api-openapi.yml
- filename: samedaydesk-com-mcp-api-openapi.yml
  format: yaml
  label: samedaydesk-com MCP API
  slug: samedaydesk-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-mcp-api-openapi.yml
- filename: samedaydesk-com-openapi-json-api-openapi.yml
  format: yaml
  label: samedaydesk-com Openapi.json API
  slug: samedaydesk-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-openapi-json-api-openapi.yml
- filename: samedaydesk-com-public-readiness-api-openapi.yml
  format: yaml
  label: samedaydesk-com Public Readiness API
  slug: samedaydesk-com-public-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-public-readiness-api-openapi.yml
- filename: samedaydesk-com-skill-md-api-openapi.yml
  format: yaml
  label: samedaydesk-com Skill.md API
  slug: samedaydesk-com-skill-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-skill-md-api-openapi.yml
- filename: samedaydesk-com-tools-api-openapi.yml
  format: yaml
  label: samedaydesk-com Tools API
  slug: samedaydesk-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-tools-api-openapi.yml
- filename: samedaydesk-com-well-known-api-openapi.yml
  format: yaml
  label: samedaydesk-com .well Known API
  slug: samedaydesk-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/samedaydesk-com/openapi/samedaydesk-com-well-known-api-openapi.yml
consequence_counts:
  read: 13
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Samedaydesk Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'samedaydesk-com exposes 15 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: samedaydesk-com
provider_slug: samedaydesk-com
slug: samedaydesk-com-agentic-access
source_filename: samedaydesk-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/samedaydesk-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 13\n    acting: 2\n  by_consequence:\n    read: 13\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/funnel-evidence\n  method: post\n  operationId: project_funnel_evidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/ai-readiness\n  method: get\n  operationId: check_ai_readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tools/llms-txt\n  method: get\n  operationId: generate_llms_txt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-readiness\n  method: get\n  operationId: check_agent_readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: get\n  operationId: describeMcpEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /mcp\n  method: post\n  operationId: mcpJsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: getAgentCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp-registry-auth\n  method: get\n  operationId: getMcpRegistryAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /skill.md\n  method: get\n  operationId: getSkillMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/api-catalog\n  method: get\n  operationId: getApiCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/correspondence/healthz\n  method: get\n  operationId: getCorrespondenceHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hosted-useful/healthz\n  method: get\n  operationId: getHostedUsefulHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public-readiness/healthz\n  method: get\n  operationId: getPublicReadinessHealth\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/samedaydesk-com/agentic-access/samedaydesk-com-agentic-access.yml
summary_line: 15 operations · 2 acting
tags:
- Company
---
