---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 17
api_specs:
- filename: salv-alert-api-openapi.yml
  format: yaml
  label: Salv Alert API
  slug: salv-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-alert-api-openapi.yml
- filename: salv-alerts-api-openapi.yml
  format: yaml
  label: Salv Alerts API
  slug: salv-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-alerts-api-openapi.yml
- filename: salv-aml-api-openapi.yml
  format: yaml
  label: Salv Aml API
  slug: salv-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-aml-api-openapi.yml
- filename: salv-custom-list-record-api-openapi.yml
  format: yaml
  label: Salv Custom List Record API
  slug: salv-custom-list-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-custom-list-record-api-openapi.yml
- filename: salv-custom-list-usable-field-public-api-openapi.yml
  format: yaml
  label: Salv Custom List Usable Field Public API
  slug: salv-custom-list-usable-field-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-custom-list-usable-field-public-api-openapi.yml
- filename: salv-data-upload-api-openapi.yml
  format: yaml
  label: Salv Data Upload API
  slug: salv-data-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-data-upload-api-openapi.yml
- filename: salv-manual-alerts-api-openapi.yml
  format: yaml
  label: Salv Manual Alerts API
  slug: salv-manual-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-manual-alerts-api-openapi.yml
- filename: salv-monitoring-checks-api-openapi.yml
  format: yaml
  label: Salv Monitoring Checks API
  slug: salv-monitoring-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-monitoring-checks-api-openapi.yml
- filename: salv-note-api-openapi.yml
  format: yaml
  label: Salv Note API
  slug: salv-note-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-note-api-openapi.yml
- filename: salv-risk-api-openapi.yml
  format: yaml
  label: Salv Risk API
  slug: salv-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-risk-api-openapi.yml
- filename: salv-screening-alerts-api-openapi.yml
  format: yaml
  label: Salv Screening Alerts API
  slug: salv-screening-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-screening-alerts-api-openapi.yml
- filename: salv-screening-checks-api-openapi.yml
  format: yaml
  label: Salv Screening Checks API
  slug: salv-screening-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-screening-checks-api-openapi.yml
- filename: salv-screening-list-groups-api-openapi.yml
  format: yaml
  label: Salv Screening List Groups API
  slug: salv-screening-list-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-screening-list-groups-api-openapi.yml
- filename: salv-screening-searches-api-openapi.yml
  format: yaml
  label: Salv Screening Searches API
  slug: salv-screening-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-screening-searches-api-openapi.yml
- filename: salv-unresolved-alerts-api-openapi.yml
  format: yaml
  label: Salv Unresolved Alerts API
  slug: salv-unresolved-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-unresolved-alerts-api-openapi.yml
consequence_counts:
  read: 17
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Salv Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'Salv exposes 36 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Salv
provider_slug: salv
slug: salv-agentic-access
source_filename: salv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/salv-alert-api-openapi.yml, openapi/salv-alerts-api-openapi.yml, openapi/salv-aml-api-openapi.yml,\n  openapi/salv-custom-list-record-api-openapi.yml, openapi/salv-custom-list-usable-field-public-api-openapi.yml,\n  openapi/salv-data-upload-api-openapi.yml, openapi/salv-manual-alerts-api-openapi.yml, openapi/salv-monitoring-checks-api-openapi.yml,\n  openapi/salv-note-api-openapi.yml, openapi/salv-risk-api-openapi.yml, openapi/salv-screening-alerts-api-openapi.yml,\n  openapi/salv-screening-checks-api-openapi.yml, openapi/salv-screening-list-groups-api-openapi.yml,\n  openapi/salv-screening-searches-api-openapi.yml, openapi/salv-unresolved-alerts-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 36\n  by_action_class:\n    connected: 17\n    acting: 19\n  by_consequence:\n    read: 17\n    write: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/alerts/{alertId}\n  method: get\n  operationId: getAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/alerts/status\n  method: put\n  operationId: publicUpdateAlertStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v2/persons\n  method: post\n  operationId: addPersonV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v2/persons/search\n  method: post\n  operationId: findAllPersons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v2/persons/{personId}\n  method: patch\n  operationId: patchPersonV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v2/persons/{personId}\n  method: put\n  operationId: updatePersonV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/persons\n  method: get\n  operationId: findAllPersonsDeprecated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/persons\n  method: post\n  operationId: addPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/persons/{personId}\n  method: get\n  operationId: findPersonById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - aml\n- path: /v1/persons/{personId}\n  method: patch\n  operationId: updatePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/persons/{personId}/transactions\n  method: get\n  operationId: findAllPersonTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/persons/{personId}/transactions\n  method: post\n  operationId: addTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - aml\n- path: /v1/persons/{personId}/transactions/{transactionId}\n  method: get\n  operationId: findTransactionByIdAndPersonId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/persons/{personId}/transactions/{transactionId}\n  method: patch\n  operationId: updateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/persons/{personId}/statuses\n  method: get\n  operationId: findStatusesHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - aml\n- path: /v1/custom-lists/{customListId}/records\n  method: get\n  operationId: getRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/custom-lists/{customListId}/records\n  method: post\n  operationId: addRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/custom-lists/{customListId}/records/{id}\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/custom-lists/{customListId}/records/{id}\n  method: put\n  operationId:\
  \ updateRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/custom-lists/{customListId}/records/{id}\n  method: delete\n  operationId: deleteRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/custom-lists/{customListId}/screening-fields\n  method: get\n  operationId: getListScreeningFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n-\
  \ path: /v1/data-upload\n  method: post\n  operationId: uploadData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/data-upload/{uploadId}/status\n  method: get\n  operationId: getDataUploadStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/manual-alerts\n  method: post\n  operationId: createManualAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n  \
  \  - aml\n- path: /v1/manual-alerts/{alertId}\n  method: put\n  operationId: updateManualAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/persons/{personId}/monitoring-checks\n  method: post\n  operationId: runPersonMonitoringChecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/transactions/{transactionId}/monitoring-checks\n  method: post\n  operationId: runTransactionMonitoringChecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/persons/{personId}/notes\n  method: post\n  operationId: addPersonNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/persons/{personId}/risks\n  method: get\n  operationId: getPersonRisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/screening-alerts/{screeningAlertId}/hits\n  method: get\n  operationId: getScreeningAlertHits\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/transactions/{id}/screening-checks\n  method: post\n  operationId: checkTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/persons/{id}/screening-checks\n  method: post\n  operationId: checkPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aml\n- path: /v1/screening-list-groups\n  method: get\n  operationId: findCustomListSelectorGroups\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v2/screening-searches\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/persons/{id}/unresolved-alerts\n  method: get\n  operationId: hasUnresolvedPersonAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n- path: /v1/transactions/{id}/unresolved-alerts\n  method: get\n  operationId: hasUnresolvedTransactionAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/agentic-access/salv-agentic-access.yml
summary_line: 36 operations · 19 acting
tags:
- Company
- AML
- Financial Crime
- Compliance
- RegTech
- Sanctions Screening
- Transaction Monitoring
- Fraud Prevention
---
