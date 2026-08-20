---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 30
api_specs:
- filename: unify-events-api-openapi.yml
  format: yaml
  label: Unify Analytics Events API
  slug: unify-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-events-api-openapi.yml
- filename: unify-event-query-jobs-api-openapi.yml
  format: yaml
  label: Unify Event Query Jobs API
  slug: unify-event-query-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-event-query-jobs-api-openapi.yml
- filename: unify-objects-api-openapi.yml
  format: yaml
  label: Unify Objects API
  slug: unify-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-objects-api-openapi.yml
- filename: unify-object-attributes-api-openapi.yml
  format: yaml
  label: Unify Object Attributes API
  slug: unify-object-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-attributes-api-openapi.yml
- filename: unify-object-attribute-options-api-openapi.yml
  format: yaml
  label: Unify Object Attribute Options API
  slug: unify-object-attribute-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-attribute-options-api-openapi.yml
- filename: unify-object-records-api-openapi.yml
  format: yaml
  label: Unify Object Records API
  slug: unify-object-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-records-api-openapi.yml
- filename: unify-object-record-query-jobs-api-openapi.yml
  format: yaml
  label: Unify Object Record Query Jobs API
  slug: unify-object-record-query-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-record-query-jobs-api-openapi.yml
- filename: unify-sequences-api-openapi.yml
  format: yaml
  label: Unify Sequences API
  slug: unify-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequences-api-openapi.yml
- filename: unify-sequence-enrollments-api-openapi.yml
  format: yaml
  label: Unify Sequence Enrollments API
  slug: unify-sequence-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequence-enrollments-api-openapi.yml
- filename: unify-sequence-enrollment-steps-api-openapi.yml
  format: yaml
  label: Unify Sequence Enrollment Steps API
  slug: unify-sequence-enrollment-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequence-enrollment-steps-api-openapi.yml
- filename: unify-tasks-api-openapi.yml
  format: yaml
  label: Unify Tasks API
  slug: unify-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-tasks-api-openapi.yml
consequence_counts:
  physical: 3
  read: 30
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Unify Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /identify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /page
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /track
operation_count: 68
overview: 'Unify exposes 68 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 35 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Unify
provider_slug: unify
slug: unify-agentic-access
source_filename: unify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/unify-event-query-jobs-api-openapi.yml, openapi/unify-events-api-openapi.yml,\n  openapi/unify-object-attribute-options-api-openapi.yml, openapi/unify-object-attributes-api-openapi.yml,\n  openapi/unify-object-record-query-jobs-api-openapi.yml, openapi/unify-object-records-api-openapi.yml,\n  openapi/unify-objects-api-openapi.yml, openapi/unify-sequence-enrollment-steps-api-openapi.yml,\n  openapi/unify-sequence-enrollments-api-openapi.yml, openapi/unify-sequences-api-openapi.yml,\n  openapi/unify-tasks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 68\n  by_action_class:\n    acting: 38\n    connected: 30\n  by_consequence:\n    write: 35\n    read: 30\n    physical:\
  \ 3\n  human_in_the_loop_required: 0\noperations:\n- path: /data/v1/events/query-jobs\n  method: post\n  operationId: create_event_query_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/events/query-jobs\n  method: get\n  operationId: list_event_query_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/events/query-jobs/{job_id}\n  method: get\n  operationId: get_event_query_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/events/query-jobs/{job_id}/cancel\n  method: post\n  operationId: cancel_event_query_job\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/events/query-jobs/{job_id}/results\n  method: get\n  operationId: get_event_query_job_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identify\n  method: post\n  operationId: send_identify_event\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /page\n  method: post\n  operationId: send_page_event\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /track\n  method: post\n  operationId: send_track_event\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/attributes/{attribute_name}/options\n  method: get\n  operationId: list_object_attribute_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /data/v1/objects/{object_name}/attributes/{attribute_name}/options\n  method: post\n  operationId: create_object_attribute_option\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/attributes/{attribute_name}/options/{option_name}\n  method: get\n  operationId: get_object_attribute_option\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/objects/{object_name}/attributes/{attribute_name}/options/{option_name}\n  method: patch\n  operationId: update_object_attribute_option\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/attributes/{attribute_name}/options/{option_name}\n  method: delete\n  operationId: delete_object_attribute_option\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/attributes\n  method: get\n  operationId: list_object_attributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/objects/{object_name}/attributes\n  method: post\n  operationId: create_object_attribute\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/attributes/{attribute_name}\n  method: get\n  operationId: get_object_attribute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/objects/{object_name}/attributes/{attribute_name}\n  method: patch\n  operationId: update_object_attribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/attributes/{attribute_name}\n  method: delete\n  operationId: delete_object_attribute\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/query-jobs\n  method: post\n  operationId: create_object_record_query_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/query-jobs\n  method: get\n  operationId: list_object_record_query_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/objects/{object_name}/query-jobs/{job_id}\n  method: get\n\
  \  operationId: get_object_record_query_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/objects/{object_name}/query-jobs/{job_id}/cancel\n  method: post\n  operationId: cancel_object_record_query_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/query-jobs/{job_id}/results\n  method: get\n  operationId: get_object_record_query_job_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/objects/{object_name}/records\n  method: post\n  operationId: create_object_record\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/records/find-unique\n  method: post\n  operationId: find_unique_object_record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/records/upsert\n  method: post\n  operationId: upsert_object_record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/records/{record_id}\n  method: get\n  operationId: get_object_record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/objects/{object_name}/records/{record_id}\n  method: patch\n  operationId: update_object_record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}/records/{record_id}\n  method: delete\n  operationId: delete_object_record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects\n  method: get\n  operationId: list_objects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/objects\n  method: post\n  operationId: create_object\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}\n  method: get\n  operationId: get_object\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/objects/{object_name}\n  method: patch\n  operationId: update_object\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v1/objects/{object_name}\n  method: delete\n  operationId: delete_object\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/enrollment-steps/query-jobs\n  method: post\n  operationId: create_sequence_enrollment_step_query_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /sequences/v1/enrollment-steps/query-jobs\n  method: get\n  operationId: list_sequence_enrollment_step_query_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/enrollment-steps/query-jobs/{job_id}\n  method: get\n  operationId: get_sequence_enrollment_step_query_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/enrollment-steps/query-jobs/{job_id}/cancel\n  method: post\n  operationId: cancel_sequence_enrollment_step_query_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/enrollment-steps/query-jobs/{job_id}/results\n\
  \  method: get\n  operationId: get_sequence_enrollment_step_query_job_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/enrollments\n  method: post\n  operationId: create_sequence_enrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/enrollments\n  method: get\n  operationId: list_sequence_enrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/enrollments/query-jobs\n  method: post\n  operationId: create_sequence_enrollment_query_job\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/enrollments/query-jobs\n  method: get\n  operationId: list_sequence_enrollment_query_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/enrollments/query-jobs/{job_id}\n  method: get\n  operationId: get_sequence_enrollment_query_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/enrollments/query-jobs/{job_id}/cancel\n  method: post\n  operationId: cancel_sequence_enrollment_query_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/enrollments/query-jobs/{job_id}/results\n  method: get\n  operationId: get_sequence_enrollment_query_job_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/enrollments/{id}\n  method: get\n  operationId: get_sequence_enrollment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/enrollments/{id}\n  method: delete\n  operationId: delete_sequence_enrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/enrollments/{id}/pause\n  method: post\n  operationId: pause_sequence_enrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/enrollments/{id}/resume\n  method: post\n  operationId: resume_sequence_enrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/sequences\n  method: get\n  operationId: list_sequences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/sequences/{id}\n  method: get\n  operationId: retrieve_sequence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/sequences/{id}\n  method: delete\n  operationId: delete_sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/sequences/{id}/pause\n  method: post\n  operationId: pause_sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /sequences/v1/sequences/{id}/resume\n  method: post\n  operationId: resume_sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/v1/sequences/{id}/steps\n  method: get\n  operationId: list_sequence_steps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/v1/sequences/{id}/steps/{step_id}\n  method: get\n  operationId: retrieve_sequence_step\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/v1/tasks\n  method: get\n  operationId: list_tasks\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/v1/tasks\n  method: post\n  operationId: create_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/v1/tasks/query-jobs\n  method: post\n  operationId: create_task_query_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/v1/tasks/query-jobs\n  method: get\n  operationId: list_task_query_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /tasks/v1/tasks/query-jobs/{job_id}\n  method: get\n  operationId: get_task_query_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/v1/tasks/query-jobs/{job_id}/cancel\n  method: post\n  operationId: cancel_task_query_job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/v1/tasks/query-jobs/{job_id}/results\n  method: get\n  operationId: get_task_query_job_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/v1/tasks/{id}\n  method: get\n  operationId: retrieve_task\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/v1/tasks/{id}\n  method: patch\n  operationId: update_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/v1/tasks/{id}\n  method: delete\n  operationId: delete_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/v1/tasks/{id}/complete\n  method: post\n  operationId: complete_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/agentic-access/unify-agentic-access.yml
summary_line: 68 operations · 38 acting
tags:
- Sales
- Marketing
- Go-To-Market
- Outbound
- Intent Data
- AI Agents
- B2B
- Data Enrichment
- Sequences
- Analytics
- Task
- Bulk API
- MCP
- Agent Skills
- Webhook
---
