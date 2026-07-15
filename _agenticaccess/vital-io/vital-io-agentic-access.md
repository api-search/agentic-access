---
acting_count: 147
action_class_counts:
  acting: 147
  connected: 444
api_specs:
- filename: vital-users-api-openapi.yml
  format: yaml
  label: Vital Users API
  slug: vital-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-users-api-openapi.yml
- filename: vital-link-api-openapi.yml
  format: yaml
  label: Vital Link API
  slug: vital-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-link-api-openapi.yml
- filename: vital-wearables-api-openapi.yml
  format: yaml
  label: Vital Wearables Data API
  slug: vital-wearables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-wearables-api-openapi.yml
- filename: vital-lab-testing-api-openapi.yml
  format: yaml
  label: Vital Lab Testing API
  slug: vital-lab-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-lab-testing-api-openapi.yml
- filename: vital-lab-report-parser-api-openapi.yml
  format: yaml
  label: Vital Lab Report Parser API
  slug: vital-lab-report-parser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-lab-report-parser-api-openapi.yml
- filename: vital-sense-api-openapi.yml
  format: yaml
  label: Vital Sense API
  slug: vital-sense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-sense-api-openapi.yml
- filename: vital-team-api-openapi.yml
  format: yaml
  label: Vital Team API
  slug: vital-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/openapi/vital-team-api-openapi.yml
consequence_counts:
  physical: 57
  read: 444
  write: 90
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
  path: /v3/lab_tests/list_order_set_markers
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
  path: /v3/order
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
  path: /v3/order/import
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/import
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/phlebotomy/appointment/availability
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/phlebotomy/appointment/availability
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/phlebotomy/appointment/availability
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/psc/appointment/availability
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/psc/appointment/availability
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/psc/appointment/availability
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/resend_events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/order/resend_events
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
  path: /v3/order/testkit
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
  method: POST
  path: /v3/order/testkit/register
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
operation_count: 591
overview: 'Vital exposes 591 API operations that an AI agent could call, of which 147 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 444 read, 90 write, and 57 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vital
provider_slug: vital-io
slug: vital-io-agentic-access
source_filename: vital-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vital-lab-report-parser-api-openapi.yml, openapi/vital-lab-testing-api-openapi.yml,\n  openapi/vital-link-api-openapi.yml, openapi/vital-openapi-original.json, openapi/vital-openapi-original.yml,\n  openapi/vital-sense-api-openapi.yml, openapi/vital-team-api-openapi.yml, openapi/vital-users-api-openapi.yml,\n  openapi/vital-wearables-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 591\n  by_action_class:\n    acting: 147\n    connected: 444\n  by_consequence:\n    write: 90\n    read: 444\n    physical: 57\n  human_in_the_loop_required: 0\noperations:\n- path: /lab_report/v1/parser/job\n  method: post\n  operationId: CreateLabReportParserJob\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lab_report/v1/parser/job/{job_id}\n  method: get\n  operationId: get_lab_report_parser_job_lab_report_v1_parser_job__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests\n  method: get\n  operationId: get_lab_tests_for_team_v3_lab_tests_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests\n  method: post\n  operationId: create_lab_test_for_team_v3_lab_tests_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/lab_tests/{lab_test_id}\n  method: patch\n  operationId: update_lab_test_for_team_v3_lab_tests__lab_test_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/lab_tests/{lab_test_id}\n  method: get\n  operationId: get_lab_test_for_team_v3_lab_tests__lab_test_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests/markers\n  method: get\n  operationId: get_markers_v3_lab_tests_markers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests/list_order_set_markers\n  method: post\n  operationId: get_markers_for_order_set_v3_lab_tests_list_order_set_markers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/lab_tests/{lab_test_id}/markers\n  method: get\n  operationId: get_markers_for_test_v3_lab_tests__lab_test_id__markers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests/{lab_id}/markers/{provider_id}\n  method: get\n  operationId: get_markers_by_provider_id_v3_lab_tests__lab_id__markers__provider_id__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_tests/labs\n  method: get\n  operationId: get_labs_v3_lab_tests_labs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/compendium/search\n  method: post\n  operationId: search_compendium_v3_compendium_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compendium/convert\n  method: post\n  operationId: convert_compendium_v3_compendium_convert_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/lab_test/lab_account\n  method: get\n  operationId: get_team_lab_accounts_v3_lab_test_lab_account_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_test\n  method: get\n  operationId: get_paginated_lab_tests_for_team_v3_lab_test_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/lab_test/{lab_test_id}/collection_instruction_pdf\n  method: get\n  operationId: get_lab_test_collection_instructions_url_v3_lab_test__lab_test_id__collection_instruction_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order_transaction/{transaction_id}\n\
  \  method: get\n  operationId: get_order_transaction_v3_order_transaction__transaction_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order_transaction/{transaction_id}/result\n  method: get\n  operationId: get_order_transaction_result_v3_order_transaction__transaction_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order_transaction/{transaction_id}/result/pdf\n  method: get\n  operationId: get_order_transaction_result_pdf_v3_order_transaction__transaction_id__result_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/orders\n  method: get\n  operationId: get_orders_v3_orders_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/testkit/register\n  method: post\n  operationId: register_testkit_v3_order_testkit_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/testkit\n  method: post\n  operationId: create_testkit_order_v3_order_testkit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/phlebotomy/appointment/availability\n\
  \  method: post\n  operationId: get_order_appointment_availability_v3_order_phlebotomy_appointment_availability_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/phlebotomy/appointment/book\n  method: post\n  operationId: book_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_book_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/phlebotomy/appointment/request\n\
  \  method: post\n  operationId: request_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/phlebotomy/appointment/reschedule\n  method: patch\n  operationId: reschedule_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_reschedule_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/phlebotomy/appointment/cancel\n\
  \  method: patch\n  operationId: cancel_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_cancel_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/phlebotomy/appointment/cancellation-reasons\n  method: get\n  operationId: get_phlebotomy_appointment_cancellation_reasons_v3_order_phlebotomy_appointment_cancellation_reasons_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/phlebotomy/appointment\n  method: get\n  operationId: get_phlebotomy_appointment_v3_order__order_id__phlebotomy_appointment_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/area/info\n  method: get\n  operationId: get_area_info_v3_order_area_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/psc/info\n  method: get\n  operationId: get_psc_info_v3_order_psc_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/psc/info\n  method: get\n  operationId: get_order_psc_info_v3_order__order_id__psc_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/result/pdf\n  method: get\n  operationId: get_lab_test_result_v3_order__order_id__result_pdf_get\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/result/metadata\n  method: get\n  operationId: get_lab_test_result_metadata_v3_order__order_id__result_metadata_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/result\n  method: get\n  operationId: get_lab_test_result_raw_v3_order__order_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/labels/pdf\n  method: get\n  operationId: get_order_labels_v3_order__order_id__labels_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/psc/appointment/availability\n\
  \  method: post\n  operationId: get_psc_appointment_availability_v3_order_psc_appointment_availability_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/psc/appointment/book\n  method: post\n  operationId: book_phlebotomy_appointment_v3_order__order_id__psc_appointment_book_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/psc/appointment/reschedule\n  method: patch\n\
  \  operationId: reschedule_phlebotomy_appointment_v3_order__order_id__psc_appointment_reschedule_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/psc/appointment/cancel\n  method: patch\n  operationId: cancel_phlebotomy_appointment_v3_order__order_id__psc_appointment_cancel_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/psc/appointment/cancellation-reasons\n  method: get\n\
  \  operationId: get_phlebotomy_appointment_cancellation_reasons_v3_order_psc_appointment_cancellation_reasons_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/psc/appointment\n  method: get\n  operationId: get_phlebotomy_appointment_v3_order__order_id__psc_appointment_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/resend_events\n  method: post\n  operationId: resend_order_webhook_v3_order_resend_events_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v3/order/{order_id}/collection_instruction_pdf\n  method: get\n  operationId: get_order_collection_instructions_url_v3_order__order_id__collection_instruction_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/requisition/pdf\n  method: get\n  operationId: get_order_requisition_url_v3_order__order_id__requisition_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}/abn_pdf\n  method: get\n  operationId: get_order_abn_v3_order__order_id__abn_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}\n  method: get\n  operationId: get_order_v3_order__order_id__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/order/{order_id}\n  method: patch\n  operationId: update_order_v3_order__order_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order\n  method: post\n  operationId: create_order_v3_order_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/import\n  method: post\n  operationId:\
  \ import_order_v3_order_import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/cancel\n  method: post\n  operationId: cancel_order_v3_order__order_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/test\n  method: post\n  operationId: order_process_simulate_v3_order__order_id__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/order/{order_id}/draw_completed\n  method: patch\n  operationId: update_on_site_collection_order_draw_completed_v3_order__order_id__draw_completed_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/insurance/search/payor\n  method: post\n  operationId: post_insurance_payor_information_v3_insurance_search_payor_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/insurance/search/payor\n  method: get\n  operationId: search_insurance_payor_information_v3_insurance_search_payor_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/insurance/search/diagnosis\n  method: get\n  operationId: search_diagnosis_v3_insurance_search_diagnosis_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/insurance/validate_icd_codes\n  method: post\n  operationId: validate_icd_codes_v3_insurance_validate_icd_codes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/payor\n  method: post\n  operationId: create_payor_v3_payor_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_op\n  method: get\n  operationId: list_bulk_ops_v2_link_bulk_op_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/bulk_import\n  method: post\n  operationId: bulk_import_connections_v2_link_bulk_import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_trigger_historical_pull\n  method: post\n  operationId: bulk_trigger_historical_pull_v2_link_bulk_trigger_historical_pull_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_export\n  method: post\n  operationId: bulk_export_connections_v2_link_bulk_export_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_pause\n  method: post\n  operationId: bulk_pause_connections_v2_link_bulk_pause_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/token\n  method: post\n  operationId: generate_vital_link_token_v2_link_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/code/create\n  method: post\n  operationId: create_token_v2_link_code_create_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v2/link/provider/oauth/{oauth_provider}\n  method: get\n  operationId: generate_oauth_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/provider/password/{provider}\n  method: post\n  operationId: connect_password_provider_v2_link_provider_password__provider__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/provider/password/{provider}/complete_mfa\n  method: post\n  operationId: complete_password_provider_mfa_v2_link_provider_password__provider__complete_mfa_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/provider/email/{provider}\n  method: post\n  operationId: connect_email_auth_provider_v2_link_provider_email__provider__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/providers\n  method: get\n  operationId: get_providers_v2_link_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/connect/demo\n  method: post\n  operationId: create_demo_connection_v2_link_connect_demo_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/providers\n  method: get\n  operationId: get_list_of_providers_v2_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/bulk_op\n  method: get\n  operationId: list_bulk_ops_v2_link_bulk_op_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/bulk_import\n  method: post\n  operationId: bulk_import_connections_v2_link_bulk_import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_trigger_historical_pull\n  method: post\n  operationId: bulk_trigger_historical_pull_v2_link_bulk_trigger_historical_pull_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_export\n  method: post\n  operationId: bulk_export_connections_v2_link_bulk_export_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/bulk_pause\n  method: post\n  operationId: bulk_pause_connections_v2_link_bulk_pause_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/token\n  method: post\n  operationId: generate_vital_link_token_v2_link_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/code/create\n  method: post\n  operationId: create_token_v2_link_code_create_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v2/link/provider/oauth/{oauth_provider}\n  method: get\n  operationId: generate_oauth_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/provider/password/{provider}\n  method: post\n  operationId: connect_password_provider_v2_link_provider_password__provider__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/provider/password/{provider}/complete_mfa\n  method: post\n  operationId: complete_password_provider_mfa_v2_link_provider_password__provider__complete_mfa_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/provider/email/{provider}\n  method: post\n  operationId: connect_email_auth_provider_v2_link_provider_email__provider__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/link/providers\n  method: get\n  operationId: get_providers_v2_link_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/link/connect/demo\n  method: post\n  operationId: create_demo_connection_v2_link_connect_demo_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/summary/electrocardiogram/{user_id}\n  method: get\n  operationId: get_user_electrocardiogram_v2_summary_electrocardiogram__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/sleep_cycle/{user_id}\n  method: get\n  operationId: get_user_sleep_cycle_v2_summary_sleep_cycle__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/profile/{user_id}\n  method: get\n  operationId: get_user_profile_v2_summary_profile__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/profile/{user_id}/raw\n  method: get\n  operationId: get_user_profile_raw_v2_summary_profile__user_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/devices/{user_id}/raw\n  method: get\n  operationId: get_user_devices_raw_v2_summary_devices__user_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/activity/{user_id}\n  method: get\n  operationId: get_user_activity_v2_summary_activity__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/activity/{user_id}/raw\n  method: get\n  operationId: get_user_activity_raw_v2_summary_activity__user_id__raw_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/workouts/{user_id}\n  method: get\n  operationId: get_user_workouts_v2_summary_workouts__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/workouts/{user_id}/raw\n  method: get\n  operationId: get_user_workouts_raw_v2_summary_workouts__user_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/summary/sleep/{user_id}\n  method: get\n  operationId: get_user_sleep_v2_summary_sleep__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: o\n\n# --- truncated at 32 KB (169 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/agentic-access/vital-io-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vital-io/refs/heads/main/agentic-access/vital-io-agentic-access.yml
summary_line: 591 operations · 147 acting
tags:
- Health Data
- Wearables
- Lab Testing
- Digital Health
- Healthtech
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
- Webhooks
- Phlebotomy
- Lab Orders
---
