---
acting_count: 45
action_class_counts:
  acting: 45
  connected: 152
api_specs:
- filename: vital-io-aggregate-api-openapi.yml
  format: yaml
  label: Vital Aggregate API
  slug: vital-io-aggregate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-aggregate-api-openapi.yml
- filename: vital-io-compendium-api-openapi.yml
  format: yaml
  label: Vital Compendium API
  slug: vital-io-compendium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-compendium-api-openapi.yml
- filename: vital-io-insurance-api-openapi.yml
  format: yaml
  label: Vital Insurance API
  slug: vital-io-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-insurance-api-openapi.yml
- filename: vital-io-introspect-api-openapi.yml
  format: yaml
  label: Vital Introspect API
  slug: vital-io-introspect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-introspect-api-openapi.yml
- filename: vital-io-lab-account-api-openapi.yml
  format: yaml
  label: Vital Lab Account API
  slug: vital-io-lab-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-lab-account-api-openapi.yml
- filename: vital-io-lab-report-api-openapi.yml
  format: yaml
  label: Vital Lab Report API
  slug: vital-io-lab-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-lab-report-api-openapi.yml
- filename: vital-io-lab-tests-api-openapi.yml
  format: yaml
  label: Vital Lab Tests API
  slug: vital-io-lab-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-lab-tests-api-openapi.yml
- filename: vital-io-link-api-openapi.yml
  format: yaml
  label: Vital Link API
  slug: vital-io-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-link-api-openapi.yml
- filename: vital-io-order-api-openapi.yml
  format: yaml
  label: Vital Order API
  slug: vital-io-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-order-api-openapi.yml
- filename: vital-io-order-transaction-api-openapi.yml
  format: yaml
  label: Vital Order Transaction API
  slug: vital-io-order-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-order-transaction-api-openapi.yml
- filename: vital-io-orders-api-openapi.yml
  format: yaml
  label: Vital Orders API
  slug: vital-io-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-orders-api-openapi.yml
- filename: vital-io-payor-api-openapi.yml
  format: yaml
  label: Vital Payor API
  slug: vital-io-payor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-payor-api-openapi.yml
- filename: vital-io-providers-api-openapi.yml
  format: yaml
  label: Vital Providers API
  slug: vital-io-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-providers-api-openapi.yml
- filename: vital-io-summary-api-openapi.yml
  format: yaml
  label: Vital Summary API
  slug: vital-io-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-summary-api-openapi.yml
- filename: vital-io-team-api-openapi.yml
  format: yaml
  label: Vital Team API
  slug: vital-io-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-team-api-openapi.yml
- filename: vital-io-user-api-openapi.yml
  format: yaml
  label: Vital User API
  slug: vital-io-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-user-api-openapi.yml
- filename: vital-io-aggregation-api-openapi.yml
  format: yaml
  label: Vital Aggregation API
  slug: vital-io-aggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-aggregation-api-openapi.yml
- filename: vital-io-lab-testing-api-openapi.yml
  format: yaml
  label: Vital Lab Testing API
  slug: vital-io-lab-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-lab-testing-api-openapi.yml
- filename: vital-io-time-series-api-openapi.yml
  format: yaml
  label: Vital Time Series API
  slug: vital-io-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-io-time-series-api-openapi.yml
consequence_counts:
  physical: 17
  read: 152
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vital Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/lab_tests/list_order_set_markers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/import
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/resend_events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/testkit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/testkit/register
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v3/order/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v3/order/{order_id}/draw_completed
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/{order_id}/phlebotomy/appointment/book
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v3/order/{order_id}/phlebotomy/appointment/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/{order_id}/phlebotomy/appointment/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v3/order/{order_id}/phlebotomy/appointment/reschedule
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/{order_id}/psc/appointment/book
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v3/order/{order_id}/psc/appointment/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v3/order/{order_id}/psc/appointment/reschedule
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/{order_id}/test
operation_count: 197
overview: 'Vital exposes 197 API operations that an AI agent could call, of which 45 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 152 read, 28 write, and 17 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vital
provider_slug: vital-io
slug: vital-io-agentic-access
source_filename: vital-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/vital-io-aggregate-api-openapi.yml, openapi/vital-io-compendium-api-openapi.yml,\n  openapi/vital-io-insurance-api-openapi.yml, openapi/vital-io-introspect-api-openapi.yml, openapi/vital-io-lab-account-api-openapi.yml,\n  openapi/vital-io-lab-report-api-openapi.yml, openapi/vital-io-lab-tests-api-openapi.yml, openapi/vital-io-link-api-openapi.yml,\n  openapi/vital-io-order-api-openapi.yml, openapi/vital-io-order-transaction-api-openapi.yml,\n  openapi/vital-io-orders-api-openapi.yml, openapi/vital-io-payor-api-openapi.yml, openapi/vital-io-providers-api-openapi.yml,\n  openapi/vital-io-summary-api-openapi.yml, openapi/vital-io-team-api-openapi.yml, openapi/vital-io-time-series-api-openapi.yml,\n  openapi/vital-io-user-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and\
  \ bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 197\n  by_action_class:\n    connected: 152\n    acting: 45\n  by_consequence:\n    read: 152\n    write: 28\n    physical: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /aggregate/v1/user/{user_id}/query\n  method: post\n  operationId: query_one_aggregate_v1_user__user_id__query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregate/v1/user/{user_id}/continuous_query/{query_id_or_slug}/result_table\n  method: get\n  operationId: get_result_table_for_query_aggregate_v1_user__user_id__continuous_query__query_id_or_slug__result_table_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregate/v1/user/{user_id}/continuous_query/{query_id_or_slug}/task_history\n\
  \  method: get\n  operationId: get_task_history_for_query_aggregate_v1_user__user_id__continuous_query__query_id_or_slug__task_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/compendium/search\n  method: post\n  operationId: search_compendium_v3_compendium_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/compendium/convert\n  method: post\n  operationId: convert_compendium_v3_compendium_convert_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/insurance/search/payor\n  method: post\n  operationId: post_insurance_payor_information_v3_insurance_search_payor_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/insurance/search/payor\n  method: get\n  operationId: search_insurance_payor_information_v3_insurance_search_payor_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/insurance/search/diagnosis\n  method: get\n  operationId: search_diagnosis_v3_insurance_search_diagnosis_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/insurance/validate_icd_codes\n  method: post\n  operationId: validate_icd_codes_v3_insurance_validate_icd_codes_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/introspect/resources\n  method: get\n  operationId: introspect_resources_v2_introspect_resources_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/introspect/historical_pull\n  method: get\n  operationId: introspect_historical_pulls_v2_introspect_historical_pull_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_test/lab_account\n  method: get\n  operationId: get_team_lab_accounts_v3_lab_test_lab_account_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /lab_report/v1/parser/job\n  method: post\n  operationId: CreateLabReportParserJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lab_report/v1/parser/job/{job_id}\n  method: get\n  operationId: get_lab_report_parser_job_lab_report_v1_parser_job__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests\n  method: get\n  operationId: get_lab_tests_for_team_v3_lab_tests_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests\n  method: post\n  operationId: create_lab_test_for_team_v3_lab_tests_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/lab_tests/{lab_test_id}\n  method: patch\n  operationId: update_lab_test_for_team_v3_lab_tests__lab_test_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/lab_tests/{lab_test_id}\n  method: get\n  operationId: get_lab_test_for_team_v3_lab_tests__lab_test_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests/markers\n  method: get\n  operationId:\
  \ get_markers_v3_lab_tests_markers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests/list_order_set_markers\n  method: post\n  operationId: get_markers_for_order_set_v3_lab_tests_list_order_set_markers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/lab_tests/{lab_test_id}/markers\n  method: get\n  operationId: get_markers_for_test_v3_lab_tests__lab_test_id__markers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests/{lab_id}/markers/{provider_id}\n\
  \  method: get\n  operationId: get_markers_by_provider_id_v3_lab_tests__lab_id__markers__provider_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests/labs\n  method: get\n  operationId: get_labs_v3_lab_tests_labs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_test\n  method: get\n  operationId: get_paginated_lab_tests_for_team_v3_lab_test_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_test/{lab_test_id}/collection_instruction_pdf\n  method: get\n  operationId: get_lab_test_collection_instructions_url_v3_lab_test__lab_test_id__collection_instruction_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/bulk_op\n  method: get\n  operationId: list_bulk_ops_v2_link_bulk_op_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/bulk_import\n  method: post\n  operationId: bulk_import_connections_v2_link_bulk_import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_trigger_historical_pull\n  method: post\n  operationId: bulk_trigger_historical_pull_v2_link_bulk_trigger_historical_pull_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_export\n  method: post\n  operationId: bulk_export_connections_v2_link_bulk_export_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_pause\n  method: post\n  operationId: bulk_pause_connections_v2_link_bulk_pause_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/token\n  method: post\n  operationId: generate_vital_link_token_v2_link_token_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/code/create\n  method: post\n  operationId: create_token_v2_link_code_create_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/provider/oauth/{oauth_provider}\n  method: get\n  operationId: generate_oauth_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/provider/password/{provider}\n  method: post\n  operationId: connect_password_provider_v2_link_provider_password__provider__post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/provider/password/{provider}/complete_mfa\n  method: post\n  operationId: complete_password_provider_mfa_v2_link_provider_password__provider__complete_mfa_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/provider/email/{provider}\n  method: post\n  operationId: connect_email_auth_provider_v2_link_provider_email__provider__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/providers\n  method: get\n  operationId: get_providers_v2_link_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/connect/demo\n  method: post\n  operationId: create_demo_connection_v2_link_connect_demo_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/testkit/register\n  method: post\n  operationId: register_testkit_v3_order_testkit_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/testkit\n  method: post\n  operationId: create_testkit_order_v3_order_testkit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/phlebotomy/appointment/availability\n  method: post\n  operationId: get_order_appointment_availability_v3_order_phlebotomy_appointment_availability_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/phlebotomy/appointment/book\n\
  \  method: post\n  operationId: book_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_book_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/phlebotomy/appointment/request\n  method: post\n  operationId: request_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/phlebotomy/appointment/reschedule\n\
  \  method: patch\n  operationId: reschedule_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_reschedule_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/phlebotomy/appointment/cancel\n  method: patch\n  operationId: cancel_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_cancel_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/phlebotomy/appointment/cancellation-reasons\n\
  \  method: get\n  operationId: get_phlebotomy_appointment_cancellation_reasons_v3_order_phlebotomy_appointment_cancellation_reasons_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/phlebotomy/appointment\n  method: get\n  operationId: get_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/area/info\n  method: get\n  operationId: get_area_info_v3_order_area_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/psc/info\n  method: get\n  operationId: get_psc_info_v3_order_psc_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/psc/info\n  method: get\n  operationId: get_order_psc_info_v3_order__order_id__psc_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/result/pdf\n  method: get\n  operationId: get_lab_test_result_v3_order__order_id__result_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/result/metadata\n  method: get\n  operationId: get_lab_test_result_metadata_v3_order__order_id__result_metadata_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/result\n  method: get\n  operationId: get_lab_test_result_raw_v3_order__order_id__result_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/labels/pdf\n  method: get\n  operationId: get_order_labels_v3_order__order_id__labels_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/psc/appointment/availability\n  method: post\n  operationId: get_psc_appointment_availability_v3_order_psc_appointment_availability_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/psc/appointment/book\n  method: post\n  operationId: book_phlebotomy_appointment_v3_order__order_id__psc_appointment_book_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/psc/appointment/reschedule\n  method: patch\n  operationId: reschedule_phlebotomy_appointment_v3_order__order_id__psc_appointment_reschedule_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/psc/appointment/cancel\n  method: patch\n  operationId: cancel_phlebotomy_appointment_v3_order__order_id__psc_appointment_cancel_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/psc/appointment/cancellation-reasons\n  method: get\n  operationId: get_phlebotomy_appointment_cancellation_reasons_v3_order_psc_appointment_cancellation_reasons_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/psc/appointment\n  method: get\n  operationId: get_phlebotomy_appointment_v3_order__order_id__psc_appointment_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/resend_events\n  method: post\n  operationId: resend_order_webhook_v3_order_resend_events_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/collection_instruction_pdf\n  method: get\n  operationId: get_order_collection_instructions_url_v3_order__order_id__collection_instruction_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/requisition/pdf\n  method: get\n  operationId: get_order_requisition_url_v3_order__order_id__requisition_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/abn_pdf\n  method: get\n  operationId: get_order_abn_v3_order__order_id__abn_pdf_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}\n  method: get\n  operationId: get_order_v3_order__order_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}\n  method: patch\n  operationId: update_order_v3_order__order_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order\n  method: post\n  operationId: create_order_v3_order_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/import\n  method: post\n  operationId: import_order_v3_order_import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/cancel\n  method: post\n  operationId: cancel_order_v3_order__order_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/test\n  method: post\n  operationId: order_process_simulate_v3_order__order_id__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/draw_completed\n  method: patch\n  operationId: update_on_site_collection_order_draw_completed_v3_order__order_id__draw_completed_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v3/order_transaction/{transaction_id}\n  method: get\n  operationId: get_order_transaction_v3_order_transaction__transaction_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order_transaction/{transaction_id}/result\n  method: get\n  operationId: get_order_transaction_result_v3_order_transaction__transaction_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order_transaction/{transaction_id}/result/pdf\n  method: get\n  operationId: get_order_transaction_result_pdf_v3_order_transaction__transaction_id__result_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/orders\n  method: get\n  operationId: get_orders_v3_orders_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/payor\n  method: post\n  operationId: create_payor_v3_payor_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/providers\n  method: get\n  operationId: get_list_of_providers_v2_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/electrocardiogram/{user_id}\n  method: get\n  operationId: get_user_electrocardiogram_v2_summary_electrocardiogram__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/summary/sleep_cycle/{user_id}\n  method: get\n  operationId: get_user_sleep_cycle_v2_summary_sleep_cycle__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/profile/{user_id}\n  method: get\n  operationId: get_user_profile_v2_summary_profile__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/profile/{user_id}/raw\n  method: get\n  operationId: get_user_profile_raw_v2_summary_profile__user_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/devices/{user_id}/raw\n  method: get\n  operationId: get_user_devices_raw_v2_summary_devices__user_id__raw_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/activity/{user_id}\n  method: get\n  operationId: get_user_activity_v2_summary_activity__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/activity/{user_id}/raw\n  method: get\n  operationId: get_user_activity_raw_v2_summary_activity__user_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/workouts/{user_id}\n  method: get\n  operationId: get_user_workouts_v2_summary_workouts__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/workouts/{user_id}/raw\n  method: get\n\
  \  operationId: get_user_workouts_raw_v2_summary_workouts__user_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/sleep/{user_id}\n  method: get\n  operationId: get_user_sleep_v2_summary_sleep__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/sleep/{user_id}/raw\n  method: get\n  operationId: get_user_sleep_raw_v2_summary_sleep__user_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/body/{user_id}\n  method: get\n  operationId: get_user_body_v2_summary_body__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/summary/body/{user_id}/raw\n  method: get\n  operationId: get_user_body_raw_v2_summary_body__user_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/meal/{user_id}\n  method: get\n  operationId: get_meals_v2_summary_meal__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/menstrual_cycle/{user_id}\n  method: get\n  operationId: get_user_menstrual_cycles_v2_summary_menstrual_cycle__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/team/{team_id}\n  method: get\n  operationId: get_team_v2_team__team_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/team/users/search\n  method: get\n  operationId: search_team_users_by_uuid_or_client_user_id_v2_team_users_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/team/svix/url\n  method: get\n  operationId: get_svix_webhook_url_v2_team_svix_url_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/team/source/priorities\n  method: get\n  operationId: get_source_priorities_v2_team_source_priorities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/team/source/priorities\n  method: patch\n  operationId: update_source_priorities_v2_team_source_priorities_patch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/team/{team_id}/physicians\n  method: get\n  operationId: get_team_physicians_v2_team__team_id__physicians_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (56 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/agentic-access/vital-io-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/agentic-access/vital-io-agentic-access.yml
summary_line: 197 operations · 45 acting
tags:
- Health Data
- Wearables
- Lab Testing
- Digital Health
- Health Tech
- Healthcare
- HIPAA
- HealthKit
- Health Connect
- EHR
- EMR
- Biomarkers
- Diagnostics
- Continuous Glucose Monitoring
- Sleep
- Activity
- Heart Rate
- Webhook
- Phlebotomy
- Lab Orders
---
