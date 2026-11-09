---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: caption-sh-antigravity-md-api-openapi.yml
  format: yaml
  label: caption-sh Antigravity.md API
  slug: caption-sh-antigravity-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-antigravity-md-api-openapi.yml
- filename: caption-sh-chatgpt-md-api-openapi.yml
  format: yaml
  label: caption-sh Chatgpt.md API
  slug: caption-sh-chatgpt-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-chatgpt-md-api-openapi.yml
- filename: caption-sh-claude-md-api-openapi.yml
  format: yaml
  label: caption-sh Claude.md API
  slug: caption-sh-claude-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-claude-md-api-openapi.yml
- filename: caption-sh-codex-md-api-openapi.yml
  format: yaml
  label: caption-sh Codex.md API
  slug: caption-sh-codex-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-codex-md-api-openapi.yml
- filename: caption-sh-cursor-md-api-openapi.yml
  format: yaml
  label: caption-sh Cursor.md API
  slug: caption-sh-cursor-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-cursor-md-api-openapi.yml
- filename: caption-sh-index-md-api-openapi.yml
  format: yaml
  label: caption-sh Index.md API
  slug: caption-sh-index-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-index-md-api-openapi.yml
- filename: caption-sh-install-sh-api-openapi.yml
  format: yaml
  label: caption-sh Install.sh API
  slug: caption-sh-install-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-install-sh-api-openapi.yml
- filename: caption-sh-mcp-api-openapi.yml
  format: yaml
  label: caption-sh MCP API
  slug: caption-sh-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-mcp-api-openapi.yml
- filename: caption-sh-pricing-md-api-openapi.yml
  format: yaml
  label: caption-sh Pricing.md API
  slug: caption-sh-pricing-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-pricing-md-api-openapi.yml
- filename: caption-sh-use-lazyweb-md-api-openapi.yml
  format: yaml
  label: caption-sh Use Lazyweb.md API
  slug: caption-sh-use-lazyweb-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-use-lazyweb-md-api-openapi.yml
- filename: caption-sh-well-known-api-openapi.yml
  format: yaml
  label: caption-sh .well Known API
  slug: caption-sh-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caption-sh/openapi/caption-sh-well-known-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Caption Sh Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/install-token
operation_count: 13
overview: 'caption-sh exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: caption-sh
provider_slug: caption-sh
slug: caption-sh-agentic-access
source_filename: caption-sh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/caption-sh-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 2\n    connected: 11\n  by_consequence:\n    physical: 1\n    write: 1\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /api/mcp/install-token\n  method: post\n  operationId: createLazywebMcpInstallToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n\
  \  operationId: callLazywebMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/mcp/server-card.json\n  method: get\n  operationId: getLazywebMcpServerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-skills/index.json\n  method: get\n  operationId: getLazywebAgentSkillsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /install.sh\n  method: get\n  operationId: getLazywebShellInstaller\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /index.md\n  method: get\n  operationId: getLazywebMarkdownLandingPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cursor.md\n  method: get\n  operationId: getLazywebCursorSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codex.md\n  method: get\n  operationId: getLazywebCodexSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claude.md\n  method: get\n  operationId: getLazywebClaudeSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /antigravity.md\n  method: get\n  operationId: getLazywebAntigravitySetup\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chatgpt.md\n  method: get\n  operationId: getLazywebChatGptSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /use-lazyweb.md\n  method: get\n  operationId: getLazywebUsageGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing.md\n  method: get\n  operationId: getLazywebPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/caption-sh/agentic-access/caption-sh-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Company
- Artificial Intelligence
- Video
- Captions
- Automation
---
