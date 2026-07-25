---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 6
api_specs:
- filename: octoparse-action-api-openapi.yml
  format: yaml
  label: Octoparse Action API
  slug: octoparse-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-action-api-openapi.yml
- filename: octoparse-actions-api-openapi.yml
  format: yaml
  label: Octoparse Actions API
  slug: octoparse-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-actions-api-openapi.yml
- filename: octoparse-cloud-extraction-api-openapi.yml
  format: yaml
  label: Octoparse Cloud_ Extraction API
  slug: octoparse-cloud-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-cloud-extraction-api-openapi.yml
- filename: octoparse-copy-api-openapi.yml
  format: yaml
  label: Octoparse Copy API
  slug: octoparse-copy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-copy-api-openapi.yml
- filename: octoparse-data-api-openapi.yml
  format: yaml
  label: Octoparse Data API
  slug: octoparse-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-data-api-openapi.yml
- filename: octoparse-files-api-openapi.yml
  format: yaml
  label: Octoparse Files API
  slug: octoparse-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-files-api-openapi.yml
- filename: octoparse-group-api-openapi.yml
  format: yaml
  label: Octoparse Group API
  slug: octoparse-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-group-api-openapi.yml
- filename: octoparse-groups-api-openapi.yml
  format: yaml
  label: Octoparse Groups API
  slug: octoparse-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-groups-api-openapi.yml
- filename: octoparse-items-api-openapi.yml
  format: yaml
  label: Octoparse Items API
  slug: octoparse-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-items-api-openapi.yml
- filename: octoparse-loop-api-openapi.yml
  format: yaml
  label: Octoparse Loop API
  slug: octoparse-loop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-loop-api-openapi.yml
- filename: octoparse-move-api-openapi.yml
  format: yaml
  label: Octoparse Move API
  slug: octoparse-move-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-move-api-openapi.yml
- filename: octoparse-properties-api-openapi.yml
  format: yaml
  label: Octoparse Properties API
  slug: octoparse-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-properties-api-openapi.yml
- filename: octoparse-remove-api-openapi.yml
  format: yaml
  label: Octoparse Remove API
  slug: octoparse-remove-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-remove-api-openapi.yml
- filename: octoparse-search-api-openapi.yml
  format: yaml
  label: Octoparse Search API
  slug: octoparse-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-search-api-openapi.yml
- filename: octoparse-statuses-api-openapi.yml
  format: yaml
  label: Octoparse Statuses API
  slug: octoparse-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-statuses-api-openapi.yml
- filename: octoparse-stop-api-openapi.yml
  format: yaml
  label: Octoparse Stop API
  slug: octoparse-stop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-stop-api-openapi.yml
- filename: octoparse-subtasks-api-openapi.yml
  format: yaml
  label: Octoparse Subtasks API
  slug: octoparse-subtasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-subtasks-api-openapi.yml
- filename: octoparse-task-api-openapi.yml
  format: yaml
  label: Octoparse Task API
  slug: octoparse-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-task-api-openapi.yml
- filename: octoparse-token-api-openapi.yml
  format: yaml
  label: Octoparse Token API
  slug: octoparse-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-token-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 2
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Octoparse Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: cloudextraction/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: cloudextraction/subtasks{stop}
operation_count: 21
overview: 'Octoparse exposes 21 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 13 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Octoparse
provider_slug: octoparse
slug: octoparse-agentic-access
source_filename: octoparse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/octoparse-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 15\n    connected: 6\n  by_consequence:\n    write: 13\n    read: 6\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: cloudextraction/task/subtasks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: cloudextraction/statuses\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: cloudextraction/statuses/v2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: cloudextraction/start\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: cloudextraction/stop\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: cloudextraction/subtasks{start}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: cloudextraction/subtasks{stop}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: data/all\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: data/lotno/all\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: data/markexported\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: data/notexported\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: data/remove\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: task/copy\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: task/moveToGroup\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: task/search\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: task/urls{file}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: taskGroup\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: task/getActions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: task/updateActionProperties\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: task/updateLoopItems\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/agentic-access/octoparse-agentic-access.yml
summary_line: 21 operations · 15 acting · 2 human-in-the-loop
tags:
- Harvesting
- Scraping
---
