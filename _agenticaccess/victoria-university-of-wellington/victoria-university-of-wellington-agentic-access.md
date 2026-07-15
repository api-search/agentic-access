---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: victoria-university-of-wellington-figshare-rest.yaml
  format: yaml
  label: Figshare REST API (Open Access Repository)
  slug: figshare-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-figshare-rest.yaml
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Victoria University Of Wellington Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Victoria University of Wellington exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Victoria University of Wellington
provider_slug: victoria-university-of-wellington
slug: victoria-university-of-wellington-agentic-access
source_filename: victoria-university-of-wellington-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/victoria-university-of-wellington-figshare-rest.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /articles\n  method: get\n  operationId: articles_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/search\n  method: post\n  operationId: articles_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /articles/{article_id}\n  method: get\n  operationId: article_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/versions\n  method: get\n  operationId: article_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/versions/{version_id}\n  method: get\n  operationId: article_version_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/files\n  method: get\n  operationId: article_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article_id}/files/{file_id}\n  method: get\n  operationId: article_file_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/agentic-access/victoria-university-of-wellington-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Library
- New Zealand
---
