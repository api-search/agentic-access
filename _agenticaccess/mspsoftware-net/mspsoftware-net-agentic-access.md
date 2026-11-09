---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: mspsoftware-net-categories-api-openapi.yml
  format: yaml
  label: MSP Software Categories API
  slug: mspsoftware-net-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mspsoftware-net/openapi/mspsoftware-net-categories-api-openapi.yml
- filename: mspsoftware-net-compare-api-openapi.yml
  format: yaml
  label: MSP Software Compare API
  slug: mspsoftware-net-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mspsoftware-net/openapi/mspsoftware-net-compare-api-openapi.yml
- filename: mspsoftware-net-msp-software-api-api-openapi.yml
  format: yaml
  label: MSP Software MSP Software API
  slug: mspsoftware-net-msp-software-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mspsoftware-net/openapi/mspsoftware-net-msp-software-api-api-openapi.yml
- filename: mspsoftware-net-posts-api-openapi.yml
  format: yaml
  label: MSP Software Posts API
  slug: mspsoftware-net-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mspsoftware-net/openapi/mspsoftware-net-posts-api-openapi.yml
- filename: mspsoftware-net-recent-api-openapi.yml
  format: yaml
  label: MSP Software Recent API
  slug: mspsoftware-net-recent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mspsoftware-net/openapi/mspsoftware-net-recent-api-openapi.yml
- filename: mspsoftware-net-software-api-openapi.yml
  format: yaml
  label: MSP Software Software API
  slug: mspsoftware-net-software-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mspsoftware-net/openapi/mspsoftware-net-software-api-openapi.yml
- filename: mspsoftware-net-vendors-api-openapi.yml
  format: yaml
  label: MSP Software Vendors API
  slug: mspsoftware-net-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mspsoftware-net/openapi/mspsoftware-net-vendors-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mspsoftware Net Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'MSP Software exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MSP Software
provider_slug: mspsoftware-net
slug: mspsoftware-net-agentic-access
source_filename: mspsoftware-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/mspsoftware-directory-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: apiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{slug}\n  method: get\n  operationId: getCategory\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /software\n  method: get\n  operationId: searchSoftware\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /software/{slug}\n  method: get\n  operationId: getSoftware\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compare/{pair}\n  method: get\n  operationId: getComparison\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recent\n  method: get\n  operationId: getRecent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posts/{slug}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendors/{slug}\n  method: get\n  operationId: getVendor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/mspsoftware-net/agentic-access/mspsoftware-net-agentic-access.yml
summary_line: 10 operations
tags:
- Directory
- MSP
- Software
- Comparison
- Reviews
- OpenAPI
---
