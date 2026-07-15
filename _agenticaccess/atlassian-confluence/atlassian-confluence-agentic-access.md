---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 7
api_specs:
- filename: swagger.v3.json
  format: json
  label: Confluence Cloud REST API
  slug: confluence-cloud-rest-api
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/confluence/swagger.v3.json
- filename: openapi-v2.v3.json
  format: json
  label: Confluence Cloud REST API V2
  slug: confluence-cloud-rest-api-v2
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/confluence/openapi-v2.v3.json
consequence_counts:
  read: 7
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atlassian Confluence Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Atlassian Confluence exposes 15 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Atlassian Confluence
provider_slug: atlassian-confluence
slug: atlassian-confluence-agentic-access
source_filename: atlassian-confluence-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/atlassian-confluence-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 7\n    acting: 8\n  by_consequence:\n    read: 7\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /rest/api/content/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:confluence-content.summary\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/api/content/archive\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:confluence-content\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/api/content/blueprint/instance/{draftId}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:confluence-content\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/api/content/blueprint/instance/{draftId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:confluence-content\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/pages\n  method: get\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:page:confluence\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/pages\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:page:confluence\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/pages/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:page:confluence\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/pages/{id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:page:confluence\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/pages/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:page:confluence\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/pages/{id}/title\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:page:confluence\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/spaces\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:space:confluence\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/spaces\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:space:confluence\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/spaces/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:space:confluence\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/spaces/{id}/pages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:page:confluence\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/labels/{id}/pages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - read:page:confluence\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-confluence/refs/heads/main/agentic-access/atlassian-confluence-agentic-access.yml
summary_line: 15 operations · 8 acting
tags:
- Atlassian
- Collaboration
- Content Management
- Documentation
- Knowledge Management
- Wiki
---
