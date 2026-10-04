---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 2
api_specs:
- filename: janus-machine-market-repos-api-openapi.yml
  format: yaml
  label: JANUS Machine Market Repos API
  slug: janus-machine-market-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/janus-machine-market/refs/heads/main/openapi/janus-machine-market-repos-api-openapi.yml
consequence_counts:
  physical: 1
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Janus Machine Market Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /repos/Hawkar-usls/JANUS-MACHINE-MARKET/issues
operation_count: 4
overview: 'JANUS Machine Market exposes 4 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: JANUS Machine Market
provider_slug: janus-machine-market
slug: janus-machine-market-agentic-access
source_filename: janus-machine-market-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: generated\nsource: openapi/janus-machine-market-pr-review-github-ingress-openapi.yml, openapi/janus-machine-market-search-github-ingress-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 2\n    connected: 2\n  by_consequence:\n    write: 1\n    read: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /repos/Hawkar-usls/JANUS-MACHINE-MARKET/issues\n  method: post\n  operationId: createJanusFirstFreePRReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /repos/Hawkar-usls/JANUS-MACHINE-MARKET/issues/{issue_number}/comments\n  method: get\n  operationId: getJanusPRReviewResultComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/Hawkar-usls/JANUS-MACHINE-MARKET/issues\n  method: post\n  operationId: createJanusFirstFreeSearchOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/Hawkar-usls/JANUS-MACHINE-MARKET/issues/{issue_number}/comments\n  method: get\n  operationId: getJanusSearchResultComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/janus-machine-market/refs/heads/main/agentic-access/janus-machine-market-agentic-access.yml
summary_line: 4 operations · 2 acting
tags:
- AI Agents
- Research
- Search
- Provenance
- Code Review
- GitHub Issues
- Agent Marketplace
---
