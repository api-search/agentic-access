---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 13
api_specs:
- filename: cryptodecentral-co-za-content-api-openapi.yml
  format: yaml
  label: CryptoDecentral Content API
  slug: cryptodecentral-co-za-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptodecentral-co-za/openapi/cryptodecentral-co-za-content-api-openapi.yml
- filename: cryptodecentral-co-za-directory-api-openapi.yml
  format: yaml
  label: CryptoDecentral Directory API
  slug: cryptodecentral-co-za-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptodecentral-co-za/openapi/cryptodecentral-co-za-directory-api-openapi.yml
- filename: cryptodecentral-co-za-discovery-api-openapi.yml
  format: yaml
  label: CryptoDecentral Discovery API
  slug: cryptodecentral-co-za-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptodecentral-co-za/openapi/cryptodecentral-co-za-discovery-api-openapi.yml
- filename: cryptodecentral-co-za-meta-api-openapi.yml
  format: yaml
  label: CryptoDecentral Meta API
  slug: cryptodecentral-co-za-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptodecentral-co-za/openapi/cryptodecentral-co-za-meta-api-openapi.yml
consequence_counts:
  read: 13
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cryptodecentral Co Za Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'CryptoDecentral exposes 14 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CryptoDecentral
provider_slug: cryptodecentral-co-za
slug: cryptodecentral-co-za-agentic-access
source_filename: cryptodecentral-co-za-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cryptodecentral-co-za-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 13\n    acting: 1\n  by_consequence:\n    read: 13\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/directory.json\n  method: get\n  operationId: getDirectoryFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/directory/{id}\n  method: get\n  operationId: getDirectoryListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/directory/changelog.json\n  method: get\n  operationId: getDirectoryChangelog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory/changelog.xml\n  method: get\n  operationId: getDirectoryChangelogRss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search.json\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/guides.json\n  method: get\n  operationId: listGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notes.json\n  method: get\n  operationId: listNotes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pillars.json\n  method: get\n  operationId: listPillars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dex-pulse.json\n  method: get\n  operationId: getDexPulse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/disclaimer.json\n  method: get\n  operationId: getDisclaimer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n\
  \  operationId: mcpPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/mcp.json\n  method: get\n  operationId: getMcpDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent.json\n  method: get\n  operationId: getAgentDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cryptodecentral-co-za/agentic-access/cryptodecentral-co-za-agentic-access.yml
summary_line: 14 operations · 1 acting
tags:
- Cryptocurrency
- Decentralization
- Privacy
- Education
- Sovereign Internet
---
