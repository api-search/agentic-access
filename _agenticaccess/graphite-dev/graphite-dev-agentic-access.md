---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite GitHub App
  slug: graphite-github-app
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite CLI (gt)
  slug: graphite-cli
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite GT MCP Server
  slug: graphite-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite Agent (Diamond) AI Code Review
  slug: graphite-agent-diamond
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite Merge Queue
  slug: graphite-merge-queue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
- filename: graphite-dev-openapi.yml
  format: yaml
  label: Graphite Insights
  slug: graphite-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/openapi/graphite-dev-openapi.yml
consequence_counts:
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Graphite Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Graphite exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Graphite
provider_slug: graphite-dev
slug: graphite-dev-agentic-access
source_filename: graphite-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/graphite-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 2\n    acting: 5\n  by_consequence:\n    read: 2\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /apps/graphite-app\n  method: get\n  operationId: installGitHubApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketplace/graphite-dev\n  method: get\n  operationId: getMarketplaceListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth\n\
  \  method: post\n  operationId: authenticateCli\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stacks/branches\n  method: post\n  operationId: createBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stacks/submit\n  method: post\n  operationId: submitStack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /stacks/sync\n  method: post\n  operationId: syncStack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stacks/merge\n  method: post\n  operationId: mergeStack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphite-dev/refs/heads/main/agentic-access/graphite-dev-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- Code Review
- Stacked PRs
- Merge Queue
- AI Code Review
- Developer Tools
- GitHub
---
