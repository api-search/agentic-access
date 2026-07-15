---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 13
api_specs:
- filename: sensible-extractions-api-openapi.yml
  format: yaml
  label: Sensible Extractions API
  slug: sensible-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-extractions-api-openapi.yml
- filename: sensible-classification-api-openapi.yml
  format: yaml
  label: Sensible Classification API
  slug: sensible-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-classification-api-openapi.yml
- filename: sensible-document-types-api-openapi.yml
  format: yaml
  label: Sensible Document Types and Configurations API
  slug: sensible-document-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-document-types-api-openapi.yml
- filename: sensible-reference-documents-api-openapi.yml
  format: yaml
  label: Sensible Reference Documents API
  slug: sensible-reference-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-reference-documents-api-openapi.yml
consequence_counts:
  read: 13
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sensible So Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'sensible-so exposes 32 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: sensible-so
provider_slug: sensible-so
slug: sensible-so-agentic-access
source_filename: sensible-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sensible-classification-api-openapi.yml, openapi/sensible-document-types-api-openapi.yml,\n  openapi/sensible-extractions-api-openapi.yml, openapi/sensible-reference-documents-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 19\n    connected: 13\n  by_consequence:\n    write: 19\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /classify\n  method: post\n  operationId: classify-document-sync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /classify/async\n  method: post\n  operationId: classify-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_types/{type-id}/configurations\n  method: post\n  operationId: create-configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_types/{type-id}/configurations\n  method: get\n  operationId: list-configurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /document_types/{type-id}/configurations/{config-name}\n  method: get\n  operationId: get-configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document_types/{type-id}/configurations/{config-name}\n  method: put\n  operationId: update-configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_types/{type-id}/configurations/{config-name}\n  method: delete\n  operationId: delete-configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_types/{type-id}/configurations/{config-name}/{version}\n  method: delete\n  operationId: delete-configuration-by-version\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_types/{type-id}/configurations/{config-name}/{version}\n  method: get\n  operationId: get-configuration-by-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document_types\n  method: post\n  operationId: create-document-type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_types\n  method: get\n  operationId: list-document-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document_types/{type-id}\n  method: get\n  operationId: get-document-type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document_types/{type-id}\n  method: delete\n  operationId: delete-document-type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_types/{type-id}/configurations/{config-name}/versions\n\
  \  method: get\n  operationId: get-configuration-versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extract/{document_type}/{config_name}\n  method: post\n  operationId: extract-data-from-a-document-with-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generate_csv/{ids}\n  method: get\n  operationId: get-csv-extraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extract/{document_type}\n  method: post\n  operationId: extract-data-from-a-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extract_from_url\n  method: post\n  operationId: provide-a-download-url-for-a-pdf-portfolio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extractions/statistics\n  method: get\n  operationId: statistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generate_upload_url\n  method: post\n  operationId: generate-an-upload-url-for-a-pdf-portfolio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}\n  method: get\n  operationId: retrieving-results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generate_upload_url/{document_type}/{config_name}\n  method: post\n  operationId: generate-an-upload-url-with-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extract_from_url/{document_type}/{config_name}\n  method: post\n  operationId: provide-a-download-url-with-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extractions\n  method: get\n  operationId: list-extractions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generate_excel/{ids}\n  method: get\n  operationId: get-excel-extraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document_types/{type-id}/goldens\n  method: post\n  operationId: create-reference-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /document_types/{type-id}/goldens\n  method: get\n  operationId: list-reference-documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extract_text_from_golden/{type-name}\n  method: post\n  operationId: extract-all-text-from-reference-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_types/{type-id}/goldens/{document-name}\n  method: put\n  operationId: update-reference-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /document_types/{type-id}/goldens/{document-name}\n  method: get\n  operationId: get-reference-document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document_types/{type-id}/goldens/{document-name}\n  method: delete\n  operationId: delete-reference-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_types/{type-id}/goldens/{document-name}/configuration\n  method: delete\n  operationId: delete-reference-document-association\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/agentic-access/sensible-so-agentic-access.yml
summary_line: 32 operations · 19 acting
tags: []
---
