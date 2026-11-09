---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: agent-module-dev-checkout-api-openapi.yml
  format: yaml
  label: Agent Module Checkout API
  slug: agent-module-dev-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-checkout-api-openapi.yml
- filename: agent-module-dev-delta-api-openapi.yml
  format: yaml
  label: Agent Module Delta API
  slug: agent-module-dev-delta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-delta-api-openapi.yml
- filename: agent-module-dev-demo-api-openapi.yml
  format: yaml
  label: Agent Module Demo API
  slug: agent-module-dev-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-demo-api-openapi.yml
- filename: agent-module-dev-interest-api-openapi.yml
  format: yaml
  label: Agent Module Interest API
  slug: agent-module-dev-interest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-interest-api-openapi.yml
- filename: agent-module-dev-keys-api-openapi.yml
  format: yaml
  label: Agent Module Keys API
  slug: agent-module-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-keys-api-openapi.yml
- filename: agent-module-dev-mcp-api-openapi.yml
  format: yaml
  label: Agent Module MCP API
  slug: agent-module-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-mcp-api-openapi.yml
- filename: agent-module-dev-referral-api-openapi.yml
  format: yaml
  label: Agent Module Referral API
  slug: agent-module-dev-referral-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-referral-api-openapi.yml
- filename: agent-module-dev-status-api-openapi.yml
  format: yaml
  label: Agent Module Status API
  slug: agent-module-dev-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-status-api-openapi.yml
- filename: agent-module-dev-telemetry-api-openapi.yml
  format: yaml
  label: Agent Module Telemetry API
  slug: agent-module-dev-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-telemetry-api-openapi.yml
- filename: agent-module-dev-trial-api-openapi.yml
  format: yaml
  label: Agent Module Trial API
  slug: agent-module-dev-trial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-trial-api-openapi.yml
- filename: agent-module-dev-verify-api-openapi.yml
  format: yaml
  label: Agent Module Verify API
  slug: agent-module-dev-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-verify-api-openapi.yml
- filename: agent-module-dev-waitlist-api-openapi.yml
  format: yaml
  label: Agent Module Waitlist API
  slug: agent-module-dev-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-module-dev/openapi/agent-module-dev-waitlist-api-openapi.yml
consequence_counts:
  physical: 2
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agent Module Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/keys
operation_count: 16
overview: 'Agent Module exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agent Module
provider_slug: agent-module-dev
slug: agent-module-dev-agentic-access
source_filename: agent-module-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agent-module-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 8\n    acting: 8\n  by_consequence:\n    read: 8\n    write: 6\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/demo\n  method: get\n  operationId: getDemoVertical\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trial\n  method:\
  \ post\n  operationId: requestTrialKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/waitlist\n  method: get\n  operationId: getWaitlistOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/waitlist\n  method: post\n  operationId: joinWaitlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/interest\n  method: post\n  operationId: registerInterest\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/interest\n  method: get\n  operationId: getInterestSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/telemetry/pov\n  method: post\n  operationId: submitPoV\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/referral\n  method: post\n  operationId: submitReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkout\n  method: get\n  operationId: getCheckoutInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys\n  method: get\n  operationId: getKeyDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: post\n\
  \  operationId: issueKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/verify\n  method: get\n  operationId: verifyKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/delta\n  method: get\n  operationId: getDeltaSync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcpEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agent-module-dev/agentic-access/agent-module-dev-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Artificial Intelligence
- Automation
- Knowledge Base
- Agents
- Platform
---
