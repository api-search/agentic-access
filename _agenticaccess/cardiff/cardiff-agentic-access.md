---
acting_count: 0
action_class_counts:
  connected: 26
api_specs:
- filename: cardiff-courses-api-openapi.yml
  format: yaml
  label: Cardiff University Courses API
  slug: cardiff-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-courses-api-openapi.yml
- filename: cardiff-clearing-adjustments-api-openapi.yml
  format: yaml
  label: Cardiff University Clearing Adjustments API
  slug: cardiff-clearing-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-clearing-adjustments-api-openapi.yml
- filename: cardiff-groups-api-openapi.yml
  format: yaml
  label: Cardiff University Groups API
  slug: cardiff-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-groups-api-openapi.yml
- filename: cardiff-modules-api-openapi.yml
  format: yaml
  label: Cardiff University Modules API
  slug: cardiff-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-modules-api-openapi.yml
- filename: cardiff-assessments-api-openapi.yml
  format: yaml
  label: Cardiff University Assessments API
  slug: cardiff-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-assessments-api-openapi.yml
- filename: cardiff-occurrences-api-openapi.yml
  format: yaml
  label: Cardiff University Occurrences API
  slug: cardiff-occurrences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-occurrences-api-openapi.yml
- filename: cardiff-rollover-api-openapi.yml
  format: yaml
  label: Cardiff University Rollover API
  slug: cardiff-rollover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-rollover-api-openapi.yml
- filename: cardiff-schools-api-openapi.yml
  format: yaml
  label: Cardiff University Schools API
  slug: cardiff-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-schools-api-openapi.yml
- filename: cardiff-subjects-api-openapi.yml
  format: yaml
  label: Cardiff University Subjects API
  slug: cardiff-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-subjects-api-openapi.yml
- filename: cardiff-levels-api-openapi.yml
  format: yaml
  label: Cardiff University Levels API
  slug: cardiff-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-levels-api-openapi.yml
- filename: cardiff-semesters-api-openapi.yml
  format: yaml
  label: Cardiff University Semesters API
  slug: cardiff-semesters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-semesters-api-openapi.yml
- filename: cardiff-qualifications-api-openapi.yml
  format: yaml
  label: Cardiff University Qualifications API
  slug: cardiff-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-qualifications-api-openapi.yml
- filename: cardiff-years-api-openapi.yml
  format: yaml
  label: Cardiff University Years API
  slug: cardiff-years-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-years-api-openapi.yml
- filename: cardiff-publications-api-openapi.yml
  format: yaml
  label: Cardiff University Publications API
  slug: cardiff-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-publications-api-openapi.yml
- filename: cardiff-default-api-openapi.yml
  format: yaml
  label: Cardiff University Echo Default API
  slug: cardiff-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-default-api-openapi.yml
- filename: cardiff-test-api-openapi.yml
  format: yaml
  label: Cardiff University Echo Test API
  slug: cardiff-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-test-api-openapi.yml
consequence_counts:
  read: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cardiff Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Cardiff University exposes 26 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cardiff University
provider_slug: cardiff
slug: cardiff-agentic-access
source_filename: cardiff-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cardiff-courses.yaml, openapi/cardiff-echo.yaml, openapi/cardiff-lookups.yaml,\n  openapi/cardiff-modules.yaml, openapi/cardiff-publications.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 26\n  by_consequence:\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /groups\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{code}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{code}/descriptions\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{code}/structure\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clearing-adjustments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - clearing\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /*\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /test\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schools\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /semesters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subjects\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /levels\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qualifications\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /years\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{code}/occurrences/{occurrence}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{code}/assessments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{code}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{code}/occurrences\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /map\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - lc_rollover\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /occurrences\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn-occurrences\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rollover/{year}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - lc_rollover\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /module-catalogues\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{eprintid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/agentic-access/cardiff-agentic-access.yml
summary_line: 26 operations
tags:
- Education
- Higher Education
- University
- Public Research University
- United Kingdom
- Wales
- Russell Group
- Open Data
- Course Catalog
- Research Repository
- Identity Federation
- Research Computing
- Publications
---
