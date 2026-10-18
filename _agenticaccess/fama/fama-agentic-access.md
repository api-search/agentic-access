---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 24
api_specs:
- filename: fama-public-endpoints-api-openapi.yml
  format: yaml
  label: Fama Public Endpoints API
  slug: fama-public-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fama/refs/heads/main/openapi/fama-public-endpoints-api-openapi.yml
- filename: fama-publicapi-api-openapi.yml
  format: yaml
  label: Fama Public API
  slug: fama-publicapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fama/refs/heads/main/openapi/fama-publicapi-api-openapi.yml
- filename: fama-report-api-openapi.yml
  format: yaml
  label: Fama Report API
  slug: fama-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fama/refs/heads/main/openapi/fama-report-api-openapi.yml
consequence_counts:
  read: 24
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fama Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Fama exposes 26 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fama
provider_slug: fama
slug: fama-agentic-access
source_filename: fama-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/fama-external-interface-openapi.yml, openapi/fama-public-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 24\n    acting: 2\n  by_consequence:\n    read: 24\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /behavior_kit/{behavior_kit_uuid}\n  method: get\n  operationId: _get_behavior_kit_behavior_kit__behavior_kit_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_type/{check_type_uuid}\n  method: get\n  operationId: _get_check_type_check_type__check_type_uuid__get\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_uuid}\n  method: get\n  operationId: _get_company_company__company_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{company_uuid}/check\n  method: post\n  operationId: _request_check_company__company_uuid__check_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/{company_uuid}/check\n  method: get\n  operationId: _check_status_company__company_uuid__check_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: _get_me_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /my_behavior_kits\n  method: get\n  operationId: _get_my_behavior_kits_my_behavior_kits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /my_check_types\n  method: get\n  operationId: _get_my_check_types_my_check_types_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /my_companies\n  method: get\n  operationId: get_my_companies_my_companies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{report_uuid}/pdf\n  method:\
  \ get\n  operationId: _download_report_pdf_report__report_uuid__pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{report_uuid}/person\n  method: get\n  operationId: _get_person_report__report_uuid__person_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{report_uuid}/posts\n  method: get\n  operationId: _get_posts_report__report_uuid__posts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{report_uuid}/profiles\n  method: get\n  operationId: _get_profiles_report__report_uuid__profiles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /report/{report_uuid}/summary\n  method: get\n  operationId: _get_summary_report__report_uuid__summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{report_uuid}/web_content\n  method: get\n  operationId: _get_web_content_report__report_uuid__web_content_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/checkTypes\n  method: get\n  operationId: get_check_types_api_checkTypes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/company\n  method: get\n  operationId: get_company_api_company_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/flagKits/all\n  method: get\n  operationId: get_flag_kit_all_api_flagKits_all_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/person\n  method: post\n  operationId: create_person_api_person_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/person/{report_id}\n  method: get\n  operationId: get_person_api_person__report_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/person/{report_id}/all\n  method: get\n  operationId: get_person_all_api_person__report_id__all_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/person/{report_id}/post\n  method: get\n  operationId: get_person_posts_api_person__report_id__post_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/person/{report_id}/profile\n  method: get\n  operationId: get_person_profiles_api_person__report_id__profile_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/person/{report_id}/report\n  method: get\n  operationId: get_report_pdf_api_person__report_id__report_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/person/{report_id}/searchContent\n  method: get\n  operationId: get_person_articles_api_person__report_id__searchContent_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user\n  method: get\n  operationId: get_user_api_user_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fama/refs/heads/main/agentic-access/fama-agentic-access.yml
summary_line: 26 operations · 2 acting
tags:
- Company
- Employment Screening
- Background Checks
- Human Resources
- Social Media
- Risk Management
- Compliance
- Artificial Intelligence
---
