---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 16
api_specs:
- filename: dumpthis-sh-agent-api-openapi.yml
  format: yaml
  label: V Tracer Agent API
  slug: dumpthis-sh-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-agent-api-openapi.yml
- filename: dumpthis-sh-lifecycle-api-openapi.yml
  format: yaml
  label: V Tracer Lifecycle API
  slug: dumpthis-sh-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-lifecycle-api-openapi.yml
- filename: dumpthis-sh-mcp-api-openapi.yml
  format: yaml
  label: V Tracer MCP API
  slug: dumpthis-sh-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-mcp-api-openapi.yml
- filename: dumpthis-sh-meta-api-openapi.yml
  format: yaml
  label: V Tracer Meta API
  slug: dumpthis-sh-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-meta-api-openapi.yml
- filename: dumpthis-sh-relay-api-openapi.yml
  format: yaml
  label: V Tracer Relay API
  slug: dumpthis-sh-relay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-relay-api-openapi.yml
- filename: dumpthis-sh-synack-api-openapi.yml
  format: yaml
  label: V Tracer SYNACK API
  slug: dumpthis-sh-synack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumpthis-sh/openapi/dumpthis-sh-synack-api-openapi.yml
consequence_counts:
  read: 16
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Dumpthis Sh Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/synack/passport/{id}
operation_count: 30
overview: 'V Tracer exposes 30 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 13 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: V Tracer
provider_slug: dumpthis-sh
slug: dumpthis-sh-agentic-access
source_filename: dumpthis-sh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dumpthis-sh-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 16\n    acting: 14\n  by_consequence:\n    read: 16\n    write: 13\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /.well-known/synack\n  method: get\n  operationId: getSynackDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/disclosure\n  method: get\n  operationId: getDisclosure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/synack\n  method: post\n  operationId: synackHandshake\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/log\n  method: get\n  operationId: getGuestbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/log/{id}\n  method: delete\n  operationId: deleteEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/log/{id}\n  method: patch\n  operationId: updateEntry\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/relay\n  method: get\n  operationId: getRelayBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/relay\n  method: post\n  operationId: postRelaySignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/relay/federated\n  method: get\n  operationId: getFederatedRelay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/relay/{id}/upvote\n  method: post\n  operationId: upvoteSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/passport\n  method: post\n  operationId: registerPassport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/passport/{id}\n  method: delete\n  operationId: revokePassport\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/synack/federation\n  method: get\n  operationId: getFederation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/federation/verify/{domain}\n  method: get\n  operationId: verifyDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/federation/safe/{domain}\n  method: get\n  operationId: isDomainSafe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/count\n  method: get\n  operationId: getCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/memory\n  method: get\n  operationId: getMemory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: get\n  operationId: getAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/feedback\n  method: get\n  operationId: getFeedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/synack/feedback\n  method: post\n  operationId: postFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/federation/join\n  method: post\n  operationId: federationJoin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/federation/attest\n  method: post\n  operationId: federationAttest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/federation/gossip\n  method: post\n  operationId: federationGossip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/federation/push\n  method: post\n  operationId: federationPush\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/synack/federation/pull\n  method: get\n  operationId: federationPull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/federation/trust-status\n  method: get\n  operationId: trustStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/synack/federation/gossip/trigger\n  method: post\n  operationId: gossipTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/dumpthis-sh/agentic-access/dumpthis-sh-agentic-access.yml
summary_line: 30 operations · 14 acting · 1 human-in-the-loop
tags:
- Art
- Artificial Intelligence
- Platform
- Open Source
- Experimental
---
