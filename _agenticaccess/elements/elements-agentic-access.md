---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: elements-elements-openapi.yml
  format: yaml
  label: Stoplight Elements
  slug: elements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elements/refs/heads/main/openapi/elements-elements-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Elements Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Stoplight Elements exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Stoplight Elements
provider_slug: elements
slug: elements-agentic-access
source_filename: elements-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/elements-elements-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /open-source/elements\n  method: get\n  operationId: getElementsOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/elements\n  method: get\n  operationId: getElementsDocumentation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/elements/b074dc07b3bae-getting-started-with-elements-in-react\n\
  \  method: get\n  operationId: getReactGettingStarted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/elements/19a7f9f0cbf23-getting-started-with-web-component\n  method: get\n  operationId: getWebComponentGettingStarted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/elements/507fb7fab9b7d-getting-started-with-elements-in-angular\n  method: get\n  operationId: getAngularGettingStarted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/elements/ZG9jOjMyNjU5MTM-elements-configuration-options\n  method: get\n  operationId: getConfigurationOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elements/refs/heads/main/agentic-access/elements-agentic-access.yml
summary_line: 6 operations
tags:
- API Documentation
- Developer Tools
- Documentation
- Interactive Docs
- OpenAPI
- React
- Web Components
---
