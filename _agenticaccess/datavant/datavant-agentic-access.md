---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 26
api_specs:
- filename: datavant-rest-api-openapi.yml
  format: yaml
  label: Datavant REST API
  slug: datavant-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-rest-api-openapi.yml
consequence_counts:
  physical: 15
  read: 26
  safety-critical: 2
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Datavant Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /orders/{order_id}/dispatch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /orders/{order_id}/start-record-retrieval
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/prematch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/prematch/{order_uuid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}/close-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}/queries
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/{order_id}/queries/{query_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/{order_id}/queries/{query_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}/queries/{query_id}/supporting-documents/patient-authorizations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/{order_id}/queries/{query_id}/supporting-documents/patient-authorizations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/{order_id}/queries/{query_id}/supporting-documents/patient-authorizations/{filename}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}/roster
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}/supplemental-data
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_uuid}/cancel
operation_count: 54
overview: 'Datavant exposes 54 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 11 write, 15 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Datavant
provider_slug: datavant
slug: datavant-agentic-access
source_filename: datavant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/datavant-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    connected: 26\n    acting: 28\n  by_consequence:\n    read: 26\n    physical: 15\n    safety-critical: 2\n    write: 11\n  human_in_the_loop_required: 2\noperations:\n- path: /orders/\n  method: get\n  operationId: list_orders_orders__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/\n  method: post\n  operationId: create_order_orders__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/order\n  method: get\n  operationId: get_order_by_specific_id_orders_order_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}\n  method: get\n  operationId: get_order_orders__order_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}\n  method: put\n  operationId: update_order_orders__order_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/order/validation/stats\n  method: get\n  operationId: get_order_validation_results_by_specific_id_orders_order_validation_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/validation/stats\n  method: get\n  operationId: get_order_validation_results_orders__order_id__validation_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_uuid}/validation/report\n  method: get\n  operationId: get_order_validation_report_orders__order_uuid__validation_report_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_uuid}/validation/supplemental-data-report\n\
  \  method: get\n  operationId: get_order_supplemental_data_validation_report_orders__order_uuid__validation_supplemental_data_report_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_uuid}/error-and-warning-counts\n  method: get\n  operationId: get_order_errors_and_warnings_orders__order_uuid__error_and_warning_counts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/reporting/retrievals\n  method: get\n  operationId: get_order_retrievals_reporting_data_orders__order_id__reporting_retrievals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_uuid}/cancel\n  method: post\n  operationId: cancel_order_orders__order_uuid__cancel_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/close-request\n  method: post\n  operationId: close_order_orders__order_id__close_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/roster\n  method: post\n  operationId: attach_roster_orders__order_id__roster_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/supplemental-data\n  method: post\n  operationId: attach_supplemental_data_orders__order_id__supplemental_data_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/dispatch\n  method: post\n  operationId: dispatch_order_orders__order_id__dispatch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /orders/{order_id}/submit\n  method: post\n  operationId: submit_order_orders__order_id__submit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/queries\n  method: get\n  operationId: list_queries_orders__order_id__queries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/queries\n  method: post\n  operationId: add_query_to_order_orders__order_id__queries_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/queries/{query_id}\n  method: get\n  operationId: get_query_in_order_orders__order_id__queries__query_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/queries/{query_id}\n  method: put\n  operationId: update_query_in_order_orders__order_id__queries__query_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /orders/{order_id}/queries/{query_id}\n  method: delete\n  operationId: delete_query_orders__order_id__queries__query_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/queries/{query_id}/supporting-documents/patient-authorizations\n  method: get\n  operationId: list_patient_authorization_filenames_orders__order_id__queries__query_id__supporting_documents_patient_authorizations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/queries/{query_id}/supporting-documents/patient-authorizations\n  method:\
  \ post\n  operationId: create_patient_authorization_orders__order_id__queries__query_id__supporting_documents_patient_authorizations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}/queries/{query_id}/supporting-documents/patient-authorizations\n  method: delete\n  operationId: delete_all_patient_authorizations_orders__order_id__queries__query_id__supporting_documents_patient_authorizations_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /orders/{order_id}/queries/{query_id}/supporting-documents/patient-authorizations/{filename}\n  method: get\n  operationId: get_patient_authorization_orders__order_id__queries__query_id__supporting_documents_patient_authorizations__filename__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/queries/{query_id}/supporting-documents/patient-authorizations/{filename}\n  method: delete\n  operationId: delete_patient_authorization_orders__order_id__queries__query_id__supporting_documents_patient_authorizations__filename__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /orders/prematch\n  method: post\n  operationId: create_prematch_order_orders_prematch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/prematch/all\n  method: get\n  operationId: list_prematch_orders_orders_prematch_all_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/prematch/{order_uuid}\n  method: delete\n  operationId: delete_prematch_orders_prematch__order_uuid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/prematch/{order_id}/counts\n  method: get\n  operationId: get_prematch_result_counts_orders_prematch__order_id__counts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/start-record-retrieval\n  method: put\n  operationId: dispatch_instructions_orders__order_id__start_record_retrieval_put\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /documents\n  method: get\n  operationId: list_documents_documents_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_uuid}\n  method: get\n  operationId: download_document_documents__document_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/\n  method: get\n  operationId: get_configuration_configuration__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/\n  method: put\n  operationId: put_configuration_configuration__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /configuration/supporting-documents/letter-of-representation\n  method: get\n  operationId: get_letter_of_representation_configuration_supporting_documents_letter_of_representation_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/supporting-documents/letter-of-representation\n  method: put\n  operationId: update_letter_of_representation_configuration_supporting_documents_letter_of_representation_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/supporting-documents/letter-of-representation\n  method: delete\n  operationId: delete_letter_of_representation_configuration_supporting_documents_letter_of_representation_delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/supporting-documents/health-plan-letter\n  method: get\n  operationId: get_health_plan_letter_configuration_supporting_documents_health_plan_letter_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/supporting-documents/health-plan-letter\n  method: put\n  operationId: update_health_plan_letter_configuration_supporting_documents_health_plan_letter_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /configuration/supporting-documents/health-plan-letter\n  method: delete\n  operationId: delete_health_plan_letter_configuration_supporting_documents_health_plan_letter_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/\n  method: get\n  operationId: list_projects_projects__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/\n  method: post\n  operationId: create_project_projects__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: get\n  operationId: get_project_by_id_projects__project_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: put\n  operationId: update_project_projects__project_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: delete\n  operationId: delete_project_projects__project_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/uuid/{project_uuid}\n  method: get\n  operationId: get_project_by_uuid_projects_uuid__project_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/supporting-documents/{document_type}\n  method: get\n  operationId: get_supporting_document_projects__project_id__supporting_documents__document_type__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/supporting-documents/{document_type}\n  method: put\n  operationId: upload_supporting_document_projects__project_id__supporting_documents__document_type__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/supporting-documents/{document_type}\n  method: delete\n  operationId: delete_request_letter_projects__project_id__supporting_documents__document_type__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/queries/{query_id}/visits/{visit_uuid}\n  method: get\n  operationId: get_visit_details_projects__project_id__queries__query_id__visits__visit_uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/queries/{query_id}/visits\n\
  \  method: get\n  operationId: get_query_visits_projects__project_id__queries__query_id__visits_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/agentic-access/datavant-agentic-access.yml
summary_line: 54 operations · 28 acting · 2 human-in-the-loop
tags:
- Healthcare
- United States
- Interoperability
- Health Data
- De-Identification
- Tokenization
- Real-World Data
- Record Retrieval
- Data Connectivity
- Life Sciences
- HIPAA
- Medical Records
- Release of Information
- Privacy
- Authentication
- Health Information Exchange
---
