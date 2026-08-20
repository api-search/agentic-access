---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 8
api_specs:
- filename: agora-data-health-api-openapi.yml
  format: yaml
  label: Agora Data Health API
  slug: agora-data-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-health-api-openapi.yml
- filename: agora-data-hooks-api-openapi.yml
  format: yaml
  label: Agora Data Hooks API
  slug: agora-data-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-hooks-api-openapi.yml
- filename: agora-data-import-api-openapi.yml
  format: yaml
  label: Agora Data Import API
  slug: agora-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-import-api-openapi.yml
- filename: agora-data-inventory-api-openapi.yml
  format: yaml
  label: Agora Data Inventory API
  slug: agora-data-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-inventory-api-openapi.yml
- filename: agora-data-loans-api-openapi.yml
  format: yaml
  label: Agora Data Loans API
  slug: agora-data-loans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-loans-api-openapi.yml
- filename: agora-data-login-api-openapi.yml
  format: yaml
  label: Agora Data Login API
  slug: agora-data-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-login-api-openapi.yml
- filename: agora-data-oauth-api-openapi.yml
  format: yaml
  label: Agora Data OAUTH API
  slug: agora-data-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-oauth-api-openapi.yml
- filename: agora-data-providers-api-openapi.yml
  format: yaml
  label: Agora Data Providers API
  slug: agora-data-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-providers-api-openapi.yml
- filename: agora-data-status-api-openapi.yml
  format: yaml
  label: Agora Data Status API
  slug: agora-data-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-status-api-openapi.yml
- filename: agora-data-uploads-api-openapi.yml
  format: yaml
  label: Agora Data Uploads API
  slug: agora-data-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/openapi/agora-data-uploads-api-openapi.yml
consequence_counts:
  read: 8
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agora Data Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Agora Data exposes 21 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agora Data
provider_slug: agora-data
slug: agora-data-agentic-access
source_filename: agora-data-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/agora-data-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 13\n    connected: 8\n  by_consequence:\n    write: 13\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/import/priority/{dms_vendor}/{upload_subtype}\n  method: post\n  operationId: priority_upload_api_v1_import_priority__dms_vendor___upload_subtype__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/import/{dms_vendor}/{upload_subtype}\n\
  \  method: post\n  operationId: file_import_api_v1_import__dms_vendor___upload_subtype__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/import/{dms_vendor}\n  method: post\n  operationId: performing_file_import_api_v1_import__dms_vendor__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/uploads/{api_activity_uuid}\n  method: get\n  operationId: loan_upload_status_api_v1_uploads__api_activity_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/import\n  method: get\n  operationId: return_import_format_api_v1_import_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/loans\n  method: get\n  operationId: get_loans_by_status_api_v1_loans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/loans/{rest_of_path}\n  method: delete\n  operationId: delete_loans_api_v1_loans__rest_of_path__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /import/{upload_subtype}\n  method: post\n  operationId: file_import_agora_import__upload_subtype__post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /import/priority/{dms_vendor}/{upload_subtype}\n  method: post\n  operationId: priority_file_import_import_priority__dms_vendor___upload_subtype__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /import/{dms_vendor}/{upload_subtype}\n  method: post\n  operationId: file_import_import__dms_vendor___upload_subtype__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status/{api_activity_uuid}\n  method: get\n  operationId: get_import_status_status__api_activity_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loans/{rest_of_path}\n  method: delete\n  operationId: delete_loans_loans__rest_of_path__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers\n  method: get\n  operationId: template_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/{provider_name}/{rest_of_path}\n\
  \  method: get\n  operationId: agora_endpoint_providers__provider_name___rest_of_path__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login/authenticate\n  method: post\n  operationId: login_login_authenticate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/authorize\n  method: post\n  operationId: create_a_code_oauth_authorize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n \
  \ method: post\n  operationId: rotate_tokens_oauth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hooks/files/idms\n  method: post\n  operationId: idms_file_endpoint_hooks_files_idms_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hooks/files/autoMaster\n  method: post\n  operationId: auto_master_file_endpoint_hooks_files_autoMaster_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory/homenet/aggregation\n  method: get\n  operationId: run_inventory_aggregator_inventory_homenet_aggregation_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: status_endpoint_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora-data/refs/heads/main/agentic-access/agora-data-agentic-access.yml
summary_line: 21 operations · 13 acting
tags:
- Company
- Auto Finance
- Automotive
- Lending
- Financial-Services
- Fintech
- Loan Origination
- Data Analytics
- Artificial Intelligence
- Capital Markets
---
