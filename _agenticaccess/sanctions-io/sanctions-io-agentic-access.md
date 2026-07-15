---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 17
api_specs:
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Screening API
  slug: sanctions-io-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Batch Screening API
  slug: sanctions-io-batch-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Adverse Media API
  slug: sanctions-io-adverse-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Data Sources API
  slug: sanctions-io-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Monitoring API
  slug: sanctions-io-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Account Management API
  slug: sanctions-io-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
consequence_counts:
  read: 17
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sanctions Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'sanctions.io exposes 29 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: sanctions.io
provider_slug: sanctions-io
slug: sanctions-io-agentic-access
source_filename: sanctions-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sanctions-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 17\n    acting: 12\n  by_consequence:\n    read: 17\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /search/\n  method: get\n  operationId: createScreeningRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/batch/\n  method: get\n  operationId: listBatchScreenings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/batch/\n \
  \ method: post\n  operationId: createBatchScreening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/batch/{batch_query_id}/\n  method: get\n  operationId: retrieveBatchScreening\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/batch/{batch_query_id}/\n  method: delete\n  operationId: deleteBatchScreening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/batch-result/{batch_result_id}/\n  method:\
  \ get\n  operationId: getBatchScreeningResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/media/\n  method: get\n  operationId: searchAdverseMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources/\n  method: get\n  operationId: listDataSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exporter/\n  method: get\n  operationId: exportSanctionsDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitoring/\n  method: get\n  operationId: getMonitoringList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitoring/\n  method: post\n  operationId: createMonitoringEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitoring/{monitoring_entry_id}/\n  method: get\n  operationId: getMonitoringEntryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitoring/{monitoring_entry_id}/\n  method: delete\n  operationId: deleteMonitoringEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /monitoring/result/{monitoring_result_id}/\n  method: get\n  operationId: getMonitoringResultDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitoring/result/{monitoring_result_id}/\n  method: put\n  operationId: updateMonitoringResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/\n  method: get\n  operationId: listApiTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokens/\n  method: post\n  operationId: createApiToken\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/{token_key}\n  method: delete\n  operationId: deleteApiToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/\n  method: put\n  operationId: editCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/config/\n  method: get\n  operationId: getCompanyConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/config/\n  method: put\n  operationId: editCompanyConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/\n  method: get\n  operationId: listCompanyUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/\n  method: post\n  operationId: inviteUser\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{user_uuid}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{user_uuid}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{user_uuid}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/\n  method: get\n  operationId: manageSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/count\n  method: get\n  operationId: listScreeningsCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/agentic-access/sanctions-io-agentic-access.yml
summary_line: 29 operations · 12 acting
tags:
- Anti-Money Laundering
- AML
- Sanctions Screening
- Compliance
- PEP Screening
- Watchlists
- KYC
- RegTech
---
