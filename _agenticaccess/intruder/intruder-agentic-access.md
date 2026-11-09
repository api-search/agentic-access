---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 15
api_specs:
- filename: intruder-health-api-openapi.yml
  format: yaml
  label: Intruder Health API
  slug: intruder-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-health-api-openapi.yml
- filename: intruder-issues-api-openapi.yml
  format: yaml
  label: Intruder Issues API
  slug: intruder-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-issues-api-openapi.yml
- filename: intruder-licenses-api-openapi.yml
  format: yaml
  label: Intruder Licenses API
  slug: intruder-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-licenses-api-openapi.yml
- filename: intruder-occurrences-api-openapi.yml
  format: yaml
  label: Intruder Occurrences API
  slug: intruder-occurrences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-occurrences-api-openapi.yml
- filename: intruder-scans-api-openapi.yml
  format: yaml
  label: Intruder Scans API
  slug: intruder-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-scans-api-openapi.yml
- filename: intruder-tags-api-openapi.yml
  format: yaml
  label: Intruder Tags API
  slug: intruder-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-tags-api-openapi.yml
- filename: intruder-targets-api-openapi.yml
  format: yaml
  label: Intruder Targets API
  slug: intruder-targets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-targets-api-openapi.yml
consequence_counts:
  read: 15
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Intruder Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'Intruder exposes 33 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Intruder
provider_slug: intruder
slug: intruder-agentic-access
source_filename: intruder-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/intruder-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 15\n    acting: 18\n  by_consequence:\n    read: 15\n    write: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/health/\n  method: get\n  operationId: health_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/issues/\n  method: get\n  operationId: issues_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/issues/{issue_id}/occurrences/\n\
  \  method: get\n  operationId: issues_occurrences_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/issues/{issue_id}/occurrences/{id}/snooze/\n  method: post\n  operationId: issues_occurrences_snooze_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/issues/{issue_id}/occurrences/{occurrence_id}/comments/\n  method: get\n  operationId: issues_occurrences_comments_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/issues/{issue_id}/occurrences/{occurrence_id}/comments/\n  method: post\n  operationId: issues_occurrences_comments_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/issues/{issue_id}/occurrences/{occurrence_id}/scanner_output/\n  method: get\n  operationId: issues_occurrences_scanner_output_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/issues/{issue_id}/targets/\n  method: get\n  operationId: issues_targets_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/licenses/\n  method: get\n  operationId: licenses_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/occurrences/fixed/\n  method: get\n  operationId: occurrences_fixed_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scans/\n  method: get\n  operationId: scans_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scans/\n  method: post\n  operationId: scans_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scans/schedules/\n  method: get\n  operationId: scans_schedules_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/scans/schedules/\n  method: post\n  operationId: scans_schedules_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scans/schedules/{id}/\n  method: patch\n  operationId: scans_schedules_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scans/schedules/{id}/\n  method: delete\n  operationId: scans_schedules_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scans/{id}/\n  method: get\n  operationId: scans_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scans/{id}/cancel/\n  method: post\n  operationId: scans_cancel_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tags/\n  method: get\n  operationId: tags_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/targets/\n  method: get\n  operationId: targets_list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/targets/\n  method: post\n  operationId: targets_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/targets/bulk/\n  method: post\n  operationId: targets_bulk_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/targets/{id}/\n  method: delete\n  operationId: targets_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/targets/{target_id}/api_schemas/\n  method: get\n  operationId: targets_api_schemas_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/targets/{target_id}/api_schemas/\n  method: post\n  operationId: targets_api_schemas_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/targets/{target_id}/api_schemas/{id}/\n  method: patch\n  operationId: targets_api_schemas_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/targets/{target_id}/api_schemas/{id}/\n  method: delete\n  operationId: targets_api_schemas_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/targets/{target_id}/authentications/\n  method: get\n  operationId: targets_authentications_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/targets/{target_id}/authentications/\n  method: post\n  operationId: targets_authentications_create\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/targets/{target_id}/authentications/{id}/\n  method: patch\n  operationId: targets_authentications_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/targets/{target_id}/authentications/{id}/\n  method: delete\n  operationId: targets_authentications_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/targets/{target_id}/tags/\n  method: post\n  operationId: targets_tags_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/targets/{target_id}/tags/{name}/\n  method: delete\n  operationId: targets_tags_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/intruder/agentic-access/intruder-agentic-access.yml
summary_line: 33 operations · 18 acting
tags:
- Company
- Security
- Cloud
- Artificial Intelligence
- Platform
---
