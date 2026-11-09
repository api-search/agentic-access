---
acting_count: 11
action_class_counts:
  acting: 11
api_specs:
- filename: crosswalk-to-account-api-openapi.yml
  format: yaml
  label: crosswalk Account API
  slug: crosswalk-to-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-account-api-openapi.yml
- filename: crosswalk-to-crosswalks-api-openapi.yml
  format: yaml
  label: crosswalk Crosswalks API
  slug: crosswalk-to-crosswalks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-crosswalks-api-openapi.yml
- filename: crosswalk-to-files-api-openapi.yml
  format: yaml
  label: crosswalk Files API
  slug: crosswalk-to-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-files-api-openapi.yml
- filename: crosswalk-to-help-api-openapi.yml
  format: yaml
  label: crosswalk Help API
  slug: crosswalk-to-help-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-help-api-openapi.yml
- filename: crosswalk-to-mail-api-openapi.yml
  format: yaml
  label: crosswalk Mail API
  slug: crosswalk-to-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-mail-api-openapi.yml
- filename: crosswalk-to-open-api-openapi.yml
  format: yaml
  label: crosswalk Open API
  slug: crosswalk-to-open-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-open-api-openapi.yml
- filename: crosswalk-to-post-api-openapi.yml
  format: yaml
  label: crosswalk Post API
  slug: crosswalk-to-post-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-post-api-openapi.yml
- filename: crosswalk-to-read-api-openapi.yml
  format: yaml
  label: crosswalk Read API
  slug: crosswalk-to-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-read-api-openapi.yml
- filename: crosswalk-to-remove-api-openapi.yml
  format: yaml
  label: crosswalk Remove API
  slug: crosswalk-to-remove-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-remove-api-openapi.yml
- filename: crosswalk-to-tasks-api-openapi.yml
  format: yaml
  label: crosswalk Tasks API
  slug: crosswalk-to-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-tasks-api-openapi.yml
- filename: crosswalk-to-tune-api-openapi.yml
  format: yaml
  label: crosswalk Tune API
  slug: crosswalk-to-tune-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-tune-api-openapi.yml
consequence_counts:
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crosswalk To Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'crosswalk exposes 11 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: crosswalk
provider_slug: crosswalk-to
slug: crosswalk-to-agentic-access
source_filename: crosswalk-to-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/crosswalk-to-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 11\n  by_consequence:\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/read\n  method: post\n  operationId: read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/open\n  method: post\n  operationId: open\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/post\n  method: post\n  operationId: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tune\n  method: post\n  operationId: tune\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crosswalks\n  method: post\n  operationId: crosswalks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mail\n  method: post\n  operationId: mail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account\n  method: post\n  operationId: account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/help\n  method: post\n  operationId: help\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remove\n  method: post\n  operationId: remove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tasks\n  method: post\n  operationId: tasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files\n  method: post\n  operationId: files\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/crosswalk-to/agentic-access/crosswalk-to-agentic-access.yml
summary_line: 11 operations · 11 acting
tags:
- AI Agents
- Message boards
- Email
- Calendar
- File Sharing
---
