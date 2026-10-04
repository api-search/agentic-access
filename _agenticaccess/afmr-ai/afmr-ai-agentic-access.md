---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 20
api_specs:
- filename: afmr-ai-a2a-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry A2a API
  slug: afmr-ai-a2a-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-a2a-api-openapi.yml
- filename: afmr-ai-agents-json-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Agents.json API
  slug: afmr-ai-agents-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-agents-json-api-openapi.yml
- filename: afmr-ai-changelog-json-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Changelog.json API
  slug: afmr-ai-changelog-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-changelog-json-api-openapi.yml
- filename: afmr-ai-evidence-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Evidence API
  slug: afmr-ai-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-evidence-api-openapi.yml
- filename: afmr-ai-feed-xml-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Feed.xml API
  slug: afmr-ai-feed-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-feed-xml-api-openapi.yml
- filename: afmr-ai-lift-evidence-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Lift Evidence API
  slug: afmr-ai-lift-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-lift-evidence-api-openapi.yml
- filename: afmr-ai-llms-full-txt-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Llms Full.txt API
  slug: afmr-ai-llms-full-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-llms-full-txt-api-openapi.yml
- filename: afmr-ai-llms-txt-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Llms.txt API
  slug: afmr-ai-llms-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-llms-txt-api-openapi.yml
- filename: afmr-ai-registries-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Registries API
  slug: afmr-ai-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-registries-api-openapi.yml
- filename: afmr-ai-resources-json-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Resources.json API
  slug: afmr-ai-resources-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-resources-json-api-openapi.yml
- filename: afmr-ai-rpc-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Rpc API
  slug: afmr-ai-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-rpc-api-openapi.yml
- filename: afmr-ai-server-json-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Server.json API
  slug: afmr-ai-server-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-server-json-api-openapi.yml
- filename: afmr-ai-sitemap-xml-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Sitemap.xml API
  slug: afmr-ai-sitemap-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-sitemap-xml-api-openapi.yml
- filename: afmr-ai-standards-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Standards API
  slug: afmr-ai-standards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-standards-api-openapi.yml
- filename: afmr-ai-status-json-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry Status.json API
  slug: afmr-ai-status-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-status-json-api-openapi.yml
- filename: afmr-ai-well-known-api-openapi.yml
  format: yaml
  label: Agent Failure Mode Registry .well Known API
  slug: afmr-ai-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/openapi/afmr-ai-well-known-api-openapi.yml
consequence_counts:
  physical: 1
  read: 20
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Afmr Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a
operation_count: 22
overview: 'Agent Failure Mode Registry exposes 22 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agent Failure Mode Registry
provider_slug: afmr-ai
slug: afmr-ai-agentic-access
source_filename: afmr-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/afmr-ai-discovery-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 20\n    acting: 2\n  by_consequence:\n    read: 20\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/afmr.json\n  method: get\n  operationId: getAfmrDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: getA2aAgentCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /.well-known/mcp.json\n  method: get\n  operationId: getMcpDiscoveryPointer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources.json\n  method: get\n  operationId: getMachineResourceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /server.json\n  method: get\n  operationId: getMcpRegistryManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents.json\n  method: get\n  operationId: getAgentAndToolIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getCompactAgentOrientation\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getExpandedAgentDocumentation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status.json\n  method: get\n  operationId: getPublicationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog.json\n  method: get\n  operationId: getPublicWorkChangelog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed.xml\n  method: get\n  operationId: getUpdateFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /sitemap.xml\n  method: get\n  operationId: getSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /evidence/index.json\n  method: get\n  operationId: getEvidenceMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lift-evidence/index.json\n  method: get\n  operationId: getLiftEvidenceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /standards/reputation-attestation/0.1/specification\n  method: get\n  operationId: getReputationAttestationSpecification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /standards/governance-voting/1.0/contract.json\n\
  \  method: get\n  operationId: getGovernanceVotingContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /standards/reputation-attestation/0.1/schema.json\n  method: get\n  operationId: getReputationAttestationSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /standards/reputation-attestation/0.1/verifier.json\n  method: get\n  operationId: getVerifierRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registries/endpoints/v0.1/index.json\n  method: get\n  operationId: getEndpointConformanceRegistry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rpc\n\
  \  method: post\n  operationId: mcpJsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rpc\n  method: get\n  operationId: mcpListeningStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a\n  method: post\n  operationId: a2aSendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afmr-ai/refs/heads/main/agentic-access/afmr-ai-agentic-access.yml
summary_line: 22 operations · 2 acting
tags:
- Company
- AI Agents
- Agent Governance
- Standards
- Reputation
- Failure Modes
- Discovery
- MCP
- A2A
- Machine-Readable Standards
---
