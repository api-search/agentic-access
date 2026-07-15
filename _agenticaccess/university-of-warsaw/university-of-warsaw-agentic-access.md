---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: university-of-warsaw-usos-api.yaml
  format: yaml
  label: USOS API (University of Warsaw)
  slug: usos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-usos-api.yaml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: University Of Warsaw Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'University of Warsaw exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: University of Warsaw
provider_slug: university-of-warsaw
slug: university-of-warsaw-agentic-access
source_filename: university-of-warsaw-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/university-of-warsaw-usos-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /apisrv/now\n  method: get\n  operationId: getNow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apisrv/installation\n  method: get\n  operationId: getInstallation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apiref/method_index\n  method: get\n  operationId: getMethodIndex\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apiref/method\n  method: get\n  operationId: getMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/course\n  method: get\n  operationId: getCourse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/course_edition\n  method: get\n  operationId: getCourseEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fac/faculty\n  method: get\n  operationId: getFaculty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /calendar/search\n  method: get\n  operationId: searchCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/agentic-access/university-of-warsaw-agentic-access.yml
summary_line: 8 operations
tags:
- Education
- Higher Education
- University
- Poland
- Academic Data
- Research Data
- Open Data
---
