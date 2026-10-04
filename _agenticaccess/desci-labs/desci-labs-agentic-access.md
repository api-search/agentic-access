---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: desci-labs-data-api-openapi.yml
  format: yaml
  label: DeSci Labs Data API
  slug: desci-labs-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/desci-labs/refs/heads/main/openapi/desci-labs-data-api-openapi.yml
- filename: desci-labs-query-api-openapi.yml
  format: yaml
  label: DeSci Labs Query API
  slug: desci-labs-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/desci-labs/refs/heads/main/openapi/desci-labs-query-api-openapi.yml
- filename: desci-labs-resolve-api-openapi.yml
  format: yaml
  label: DeSci Labs Resolve API
  slug: desci-labs-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/desci-labs/refs/heads/main/openapi/desci-labs-resolve-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Desci Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'DeSci Labs exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DeSci Labs
provider_slug: desci-labs
slug: desci-labs-agentic-access
source_filename: desci-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/desci-labs-data-api-openapi.yml, openapi/desci-labs-query-api-openapi.yml, openapi/desci-labs-resolve-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/data/dpid/{dpid}\n  method: get\n  operationId: getV2DataDpidByDpid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/data/cid/{cid}\n  method: get\n  operationId: getV2DataCidByCid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/data/dpid/{dpid}/*\n  method: get\n  operationId: getV2DataDpidByDpid*\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/query/objects\n  method: get\n  operationId: getV2QueryObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/query/history/{id}\n  method: get\n  operationId: getV2QueryHistoryById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/query/history\n  method: post\n  operationId: postV2QueryHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/query/dpids\n  method: get\n  operationId:\
  \ getV2QueryDpids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/query/owner/{id}\n  method: get\n  operationId: getV2QueryOwnerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/query/reverse/{id}\n  method: get\n  operationId: getV2QueryReverseById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/resolve/dpid/{dpid}/{versionIx}\n  method: get\n  operationId: getV2ResolveDpidByDpidByVersionIx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/resolve/codex/{streamOrCommitId}/{versionIx}\n  method: get\n  operationId: getV2ResolveCodexByStreamOrCommitIdByVersionIx\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/resolve/{path}\n  method: get\n  operationId: getV2ResolveByPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/desci-labs/refs/heads/main/agentic-access/desci-labs-agentic-access.yml
summary_line: 12 operations
tags:
- Company
- Ai Enterprise Software
- Research Infrastructure
- Decentralized Science
- Scholarly Communication
- Persistent Identifiers
- Open Access
- AI Research Tools
- IPFS
- MCP
---
