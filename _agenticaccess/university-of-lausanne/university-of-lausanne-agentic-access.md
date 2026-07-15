---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: university-of-lausanne-spica.yaml
  format: yaml
  label: SPICA Atlas API
  slug: spica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-spica.yaml
- filename: university-of-lausanne-iris.yaml
  format: yaml
  label: IRIS Repository (DSpace REST API)
  slug: iris
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-iris.yaml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: University Of Lausanne Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'University of Lausanne exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: University of Lausanne
provider_slug: university-of-lausanne
slug: university-of-lausanne-agentic-access
source_filename: university-of-lausanne-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/university-of-lausanne-iris.yaml, openapi/university-of-lausanne-spica.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getApiRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities\n  method: get\n  operationId: listCommunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities/{uuid}\n\
  \  method: get\n  operationId: getCommunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects.json\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/query.json\n  method: get\n  operationId: queryProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/get_file\n  method: get\n  operationId: downloadProjectFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/agentic-access/university-of-lausanne-agentic-access.yml
summary_line: 6 operations
tags:
- Education
- Higher Education
- University
- Switzerland
- Open Science
- Research Data
- Institutional Repository
---
