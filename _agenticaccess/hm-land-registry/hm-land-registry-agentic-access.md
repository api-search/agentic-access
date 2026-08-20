---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 18
api_specs:
- filename: hm-land-registry-land-register-api-openapi.yml
  format: yaml
  label: Land Register API
  slug: land-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-land-register-api-openapi.yml
- filename: hm-land-registry-estimate-completion-date-openapi.yml
  format: yaml
  label: HM Land Registry Estimate Completion Date API
  slug: hm-land-registry-estimate-completion-date-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-estimate-completion-date-openapi.yml
- filename: hm-land-registry-official-copy-document-availability-v1-customer-test-openapi.json
  format: json
  label: HM Land Registry HMLR Business Gateway (Hm Land Registry Official Copy Document Availability V1 Customer Test)
  slug: hm-land-registry-official-copy-document-availability-v1-customer-test-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-official-copy-document-availability-v1-customer-test-openapi.json
- filename: hm-land-registry-official-copy-document-availability-v1-openapi.json
  format: json
  label: HM Land Registry Official Copy Document Availability Service (Hm Land Registry Official Copy Document Availability V1)
  slug: hm-land-registry-official-copy-document-availability-v1-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-official-copy-document-availability-v1-openapi.json
- filename: hm-land-registry-official-copy-document-availability-v2-customer-test-openapi.json
  format: json
  label: HM Land Registry HMLR Business Gateway (Hm Land Registry Official Copy Document Availability V2 Customer Test)
  slug: hm-land-registry-official-copy-document-availability-v2-customer-test-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-official-copy-document-availability-v2-customer-test-openapi.json
- filename: hm-land-registry-official-copy-document-availability-v2-openapi.json
  format: json
  label: HM Land Registry Official Copy Document Availability Service (Hm Land Registry Official Copy Document Availability V2)
  slug: hm-land-registry-official-copy-document-availability-v2-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-official-copy-document-availability-v2-openapi.json
- filename: hm-land-registry-official-search-of-whole-with-data-openapi.yml
  format: yaml
  label: HM Land Registry Official Search of Whole with Data
  slug: hm-land-registry-official-search-of-whole-with-data-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-official-search-of-whole-with-data-openapi.yml
- filename: hm-land-registry-registered-proprietor-names-openapi.json
  format: json
  label: HM Land Registry Registered Proprietor Names Service
  slug: hm-land-registry-registered-proprietor-names-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-registered-proprietor-names-openapi.json
- filename: hm-land-registry-submit-application-to-change-the-register-v0.3-openapi.json
  format: json
  label: HM Land Registry V0.3 'Submit an application to change the Land Register API' Schema
  slug: hm-land-registry-submit-application-to-change-the-register-v0-3-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-submit-application-to-change-the-register-v0.3-openapi.json
- filename: hm-land-registry-submit-application-to-change-the-register-v1.0-openapi.json
  format: json
  label: HM Land Registry V1.0 'Submit an application to change the Land Register API' Schema
  slug: hm-land-registry-submit-application-to-change-the-register-v1-0-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-submit-application-to-change-the-register-v1.0-openapi.json
- filename: hm-land-registry-use-land-property-data-openapi.yml
  format: yaml
  label: HM Land Registry Use Land and Property Data API
  slug: hm-land-registry-use-land-property-data-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-use-land-property-data-openapi.yml
consequence_counts:
  physical: 4
  read: 18
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hm Land Registry Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v0/documents/url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/documents/url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: Upload a document
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: Upload a document
operation_count: 29
overview: 'HM Land Registry exposes 29 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 7 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HM Land Registry
provider_slug: hm-land-registry
slug: hm-land-registry-agentic-access
source_filename: hm-land-registry-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/hm-land-registry-estimate-completion-date-openapi.yml, openapi/hm-land-registry-land-register-api-openapi.yml,\n  openapi/hm-land-registry-official-copy-document-availability-v1-customer-test-openapi.json,\n  openapi/hm-land-registry-official-copy-document-availability-v1-openapi.json, openapi/hm-land-registry-official-copy-document-availability-v2-customer-test-openapi.json,\n  openapi/hm-land-registry-official-copy-document-availability-v2-openapi.json, openapi/hm-land-registry-official-search-of-whole-with-data-openapi.yml,\n  openapi/hm-land-registry-registered-proprietor-names-openapi.json, openapi/hm-land-registry-submit-application-to-change-the-register-v0.3-openapi.json,\n  openapi/hm-land-registry-submit-application-to-change-the-register-v1.0-openapi.json, openapi/hm-land-registry-use-land-property-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n\
  \  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 18\n    acting: 11\n  by_consequence:\n    read: 18\n    write: 7\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/applications/{application_reference}/estimate-completion-date\n  method: get\n  operationId: getEstimateCompletionDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /title/{titleNumber}\n  method: get\n  operationId: getTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /draft-titles/{titleNumber}\n  method: get\n  operationId: getDraftTitle\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles/{title_number}/official-copies/availability\n  method: get\n  operationId: getOfficialCopiesAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles/{title_number}/official-copies/availability\n  method: get\n  operationId: getOfficialCopiesAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles/{title_number}/official-copies/availability\n  method: get\n  operationId: getOfficialCopiesAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /titles/{title_number}/official-copies/availability\n  method: get\n  operationId: getOfficialCopiesAvailability\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/official-searches-of-whole\n  method: post\n  operationId: submitOfficialSearchOfWholeWithPriority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /titles/{title_number}/registered-proprietor-names\n  method: get\n  operationId: getRegisteredProprietorNames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/applications\n  method: post\n  operationId: Submit an application API\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/documents/url\n  method: post\n  operationId: Create an upload URL\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: Upload a document\n  method: put\n  operationId: Upload a document\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/applications/{application_request_id}/information\n\
  \  method: get\n  operationId: Application information API\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/notifications\n  method: get\n  operationId: Receive notifications API\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/notifications/acknowledge\n  method: post\n  operationId: Acknowledge notifications API\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications\n  method: post\n  operationId: submit_an_application_to_change_the_register_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{document_id}\n  method: get\n  operationId: download_a_document_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: Download a document\n  method: get\n  operationId: Download a document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/url\n  method: post\n  operationId: send_a_document_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: Upload a document\n  method: put\n  operationId: Upload a document\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/{application_request_id}/information\n  method: get\n  operationId: get_application_information_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{application_request_id}/attachments\n  method: post\n  operationId: attach_a_document_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/{application_request_id}/messages\n  method: post\n  operationId: attach_a_message_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications\n  method: get\n  operationId: get_notifications_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/acknowledge\n  method: post\n  operationId: acknowledge_notifications_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_name}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{dataset_name}/{file_name}\n  method: get\n  operationId: getDatasetFileDownloadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/history/{dataset_name}\n  method: get\n  operationId: getDatasetHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/agentic-access/hm-land-registry-agentic-access.yml
summary_line: 29 operations · 11 acting
tags:
- Real-Estate
- United Kingdom
- Land Registry
- Open Data
- Title
- Conveyancing
- Property Records
- Price Paid Data
- Linked Data
- Geospatial
- Government
- PropTech
---
