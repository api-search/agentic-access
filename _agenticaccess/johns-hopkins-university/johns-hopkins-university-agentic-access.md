---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: johns-hopkins-university-sis-course-search.yaml
  format: yaml
  label: Self-Service Public Course Search API (SIS)
  slug: sis-course-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/openapi/johns-hopkins-university-sis-course-search.yaml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Johns Hopkins University Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Johns Hopkins University exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Johns Hopkins University
provider_slug: johns-hopkins-university
slug: johns-hopkins-university-agentic-access
source_filename: johns-hopkins-university-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/johns-hopkins-university-sis-course-search.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /classes/codes/schools\n  method: get\n  operationId: listSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/codes/terms\n  method: get\n  operationId: listTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/codes/departments/{school}\n\
  \  method: get\n  operationId: listDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/{courseNumber}\n  method: get\n  operationId: getCoursesByNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/{courseNumber}/{term}\n  method: get\n  operationId: getCoursesByNumberAndTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/{school}/{department}/{term}\n  method: get\n  operationId: getCoursesBySchoolDepartmentTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes\n  method: get\n  operationId: advancedSearch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/agentic-access/johns-hopkins-university-agentic-access.yml
summary_line: 7 operations
tags:
- Education
- Higher Education
- University
- Research
- Course Catalog
- News
- United States
---
