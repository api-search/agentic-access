---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: remote-cache-spec
  format: yaml
  label: Turborepo Remote Cache API
  slug: turborepo-remote-cache-api
  spec_type: OpenAPI
  url: https://turborepo.dev/api/remote-cache-spec
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Turborepo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Turborepo exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Turborepo
provider_slug: turborepo
slug: turborepo-agentic-access
source_filename: turborepo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/turborepo-remote-cache-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 3\n    acting: 3\n  by_consequence:\n    read: 3\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /artifacts/status\n  method: get\n  operationId: getArtifactStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artifacts/{hash}\n  method: head\n  operationId: artifactExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artifacts/{hash}\n\
  \  method: get\n  operationId: downloadArtifact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artifacts/{hash}\n  method: put\n  operationId: uploadArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artifacts\n  method: post\n  operationId: queryArtifacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /artifacts/events\n  method: post\n  operationId: recordCacheEvents\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turborepo/refs/heads/main/agentic-access/turborepo-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Build System
- Monorepo
- JavaScript
- TypeScript
- Caching
- Open Source
- Rust
- Vercel
- Developer Tools
- CI/CD
---
