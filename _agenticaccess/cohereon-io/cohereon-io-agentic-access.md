---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 14
api_specs:
- filename: cohereon-io-claim-api-openapi.yml
  format: yaml
  label: Cohereon Claim API
  slug: cohereon-io-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-claim-api-openapi.yml
- filename: cohereon-io-components-api-openapi.yml
  format: yaml
  label: Cohereon Components API
  slug: cohereon-io-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-components-api-openapi.yml
- filename: cohereon-io-declare-api-openapi.yml
  format: yaml
  label: Cohereon Declare API
  slug: cohereon-io-declare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-declare-api-openapi.yml
- filename: cohereon-io-doc-api-openapi.yml
  format: yaml
  label: Cohereon Doc API
  slug: cohereon-io-doc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-doc-api-openapi.yml
- filename: cohereon-io-free-api-openapi.yml
  format: yaml
  label: Cohereon Free API
  slug: cohereon-io-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-free-api-openapi.yml
- filename: cohereon-io-fund-api-openapi.yml
  format: yaml
  label: Cohereon Fund API
  slug: cohereon-io-fund-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-fund-api-openapi.yml
- filename: cohereon-io-health-api-openapi.yml
  format: yaml
  label: Cohereon Health API
  slug: cohereon-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-health-api-openapi.yml
- filename: cohereon-io-identify-api-openapi.yml
  format: yaml
  label: Cohereon Identify API
  slug: cohereon-io-identify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-identify-api-openapi.yml
- filename: cohereon-io-imperium-manifold-api-api-openapi.yml
  format: yaml
  label: Cohereon Imperium Manifold API
  slug: cohereon-io-imperium-manifold-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-imperium-manifold-api-api-openapi.yml
- filename: cohereon-io-invoice-api-openapi.yml
  format: yaml
  label: Cohereon Invoice API
  slug: cohereon-io-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-invoice-api-openapi.yml
- filename: cohereon-io-lnurlp-api-openapi.yml
  format: yaml
  label: Cohereon Lnurlp API
  slug: cohereon-io-lnurlp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-lnurlp-api-openapi.yml
- filename: cohereon-io-mcp-api-openapi.yml
  format: yaml
  label: Cohereon MCP API
  slug: cohereon-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-mcp-api-openapi.yml
- filename: cohereon-io-meta-api-openapi.yml
  format: yaml
  label: Cohereon Meta API
  slug: cohereon-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-meta-api-openapi.yml
- filename: cohereon-io-patronage-api-openapi.yml
  format: yaml
  label: Cohereon Patronage API
  slug: cohereon-io-patronage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-patronage-api-openapi.yml
- filename: cohereon-io-petition-api-openapi.yml
  format: yaml
  label: Cohereon Petition API
  slug: cohereon-io-petition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-petition-api-openapi.yml
- filename: cohereon-io-ride-the-lightning-api-openapi.yml
  format: yaml
  label: Cohereon Ride The Lightning API
  slug: cohereon-io-ride-the-lightning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-ride-the-lightning-api-openapi.yml
- filename: cohereon-io-skill-md-api-openapi.yml
  format: yaml
  label: Cohereon SKILL.md API
  slug: cohereon-io-skill-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-skill-md-api-openapi.yml
- filename: cohereon-io-sponsor-api-openapi.yml
  format: yaml
  label: Cohereon Sponsor API
  slug: cohereon-io-sponsor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-sponsor-api-openapi.yml
- filename: cohereon-io-tier-api-openapi.yml
  format: yaml
  label: Cohereon Tier API
  slug: cohereon-io-tier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-tier-api-openapi.yml
- filename: cohereon-io-well-known-api-openapi.yml
  format: yaml
  label: Cohereon .well Known API
  slug: cohereon-io-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cohereon-io/openapi/cohereon-io-well-known-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Cohereon Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /mcp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice/{component_id}
operation_count: 23
overview: 'Cohereon exposes 23 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 7 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cohereon
provider_slug: cohereon-io
slug: cohereon-io-agentic-access
source_filename: cohereon-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cohereon-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 14\n    acting: 9\n  by_consequence:\n    read: 14\n    physical: 1\n    write: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /components/\n  method:\
  \ get\n  operationId: listGatedComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta/{component_id}\n  method: get\n  operationId: getComponentMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free/\n  method: get\n  operationId: listFreeComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free/{slug}\n  method: get\n  operationId: getFreeComponent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice/{component_id}\n  method: post\n  operationId: requestInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /doc/{component_id}\n  method: get\n  operationId: getComponent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tier/{npub}\n  method: get\n  operationId: getTier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identify\n  method: post\n  operationId: identifyAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /declare\n  method: post\n  operationId: declareAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fund/declare\n  method: post\n  operationId: fundDeclare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patronage/\n  method: get\n  operationId: getPatronageBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /petition/{component_id}\n  method: post\n  operationId: createPetition\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sponsor/{petition_id}\n  method: post\n  operationId: sponsorPetition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{claim_token}\n  method: get\n  operationId: claimSponsored\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lnurlp/manifold\n  method: get\n  operationId: lnurlPay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /ride-the-lightning\n  method: post\n  operationId: rideTheLightning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcpServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcpJsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: delete\n  operationId: mcpSessionTerminate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /.well-known/agent.json\n  method: get\n  operationId: agentDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SKILL.md\n  method: get\n  operationId: skillFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cohereon-io/agentic-access/cohereon-io-agentic-access.yml
summary_line: 23 operations · 9 acting · 1 human-in-the-loop
tags:
- Cohereon
- AI Risk
- Governance
- Nonhuman Intelligence
- Standards
---
