---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Authentication API
  slug: openclinica-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Participants API
  slug: openclinica-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Study Events API
  slug: openclinica-study-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Clinical Data API
  slug: openclinica-clinical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica ODM Metadata API
  slug: openclinica-odm-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Bulk Operations API
  slug: openclinica-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
consequence_counts:
  read: 5
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openclinica Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'OpenClinica exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenClinica
provider_slug: openclinica
slug: openclinica-agentic-access
source_filename: openclinica-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openclinica-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 9\n    connected: 5\n  by_consequence:\n    write: 9\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /user-service/api/oauth/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/auth/api/clinicaldata/studies/{studyOID}/participants\n  method: get\n  operationId: listStudyParticipants\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pages/auth/api/clinicaldata/studies/{studyOID}/participants\n  method: post\n  operationId: addStudyParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/auth/api/clinicaldata/studies/{studyOID}/sites/{siteOID}/participants\n  method: get\n  operationId: listSiteParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pages/auth/api/clinicaldata/studies/{studyOID}/sites/{siteOID}/participants\n  method: post\n  operationId: addSiteParticipant\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/auth/api/clinicaldata/studies/{studyOID}/sites/{siteOID}/participants/extractParticipantsInfo\n  method: post\n  operationId: extractParticipantsInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/auth/api/clinicaldata/studies/{studyOID}/participants/bulk\n  method: post\n  operationId: addBulkParticipants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/auth/api/clinicaldata/studies/{studyOID}/events\n  method: post\n  operationId: createBulkStudyEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/auth/api/clinicaldata/studies/{studyOID}/sites/{siteOID}/events\n  method: post\n  operationId: createStudyEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/auth/api/clinicaldata/studies/{studyOID}/sites/{siteOID}/events\n  method: put\n  operationId: updateStudyEvent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/auth/api/clinicaldata/{studyOID}/{participantOID}/{studyEventOID}/{formOID}\n  method: get\n  operationId: getClinicalData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pages/auth/api/clinicaldata\n  method: post\n  operationId: importClinicalData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/auth/api/clinicaldata/metadata/{studyOID}\n  method: get\n\
  \  operationId: getStudyMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pages/auth/api/bulkActionsLog\n  method: get\n  operationId: getBulkActionsLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/agentic-access/openclinica-agentic-access.yml
summary_line: 14 operations · 9 acting
tags:
- Clinical Trials
- Electronic Data Capture
- EDC
- Clinical Data Management
- CDISC ODM
- Healthcare
- Open Source
---
