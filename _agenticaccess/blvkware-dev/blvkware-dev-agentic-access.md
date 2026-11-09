---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: blvkware-dev-check-api-openapi.yml
  format: yaml
  label: BlvkWare Check API
  slug: blvkware-dev-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvkware-dev/openapi/blvkware-dev-check-api-openapi.yml
- filename: blvkware-dev-corpus-api-openapi.yml
  format: yaml
  label: BlvkWare Corpus API
  slug: blvkware-dev-corpus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvkware-dev/openapi/blvkware-dev-corpus-api-openapi.yml
- filename: blvkware-dev-meta-api-openapi.yml
  format: yaml
  label: BlvkWare Meta API
  slug: blvkware-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvkware-dev/openapi/blvkware-dev-meta-api-openapi.yml
- filename: blvkware-dev-watch-api-openapi.yml
  format: yaml
  label: BlvkWare Watch API
  slug: blvkware-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvkware-dev/openapi/blvkware-dev-watch-api-openapi.yml
consequence_counts:
  read: 7
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blvkware Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'BlvkWare exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BlvkWare
provider_slug: blvkware-dev
slug: blvkware-dev-agentic-access
source_filename: blvkware-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/blvkware-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 3\n    connected: 7\n  by_consequence:\n    write: 3\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /check\n  method: post\n  operationId: checkBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check/{namespace}/{value}\n  method: get\n  operationId: checkIdentifier\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /corpus\n  method: get\n  operationId: streamCorpus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces\n  method: get\n  operationId: listNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proof\n  method: get\n  operationId: proofSurface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: corpusStats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verdicts\n  method: get\n  operationId: describeVerdicts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /watch\n  method: post\n  operationId: createWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/{watchId}\n  method: delete\n  operationId: deleteWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://artifacts.apis.io/blvkware-dev/agentic-access/blvkware-dev-agentic-access.yml
summary_line: 10 operations · 3 acting
tags:
- Artificial Intelligence
- Agents
- Kit
- Automation
- Marketplace
- Company
---
