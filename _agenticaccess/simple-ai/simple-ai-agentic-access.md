---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 27
api_specs:
- filename: simple-ai-agents-api-openapi.yml
  format: yaml
  label: Simple AI Agents API
  slug: simple-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-agents-api-openapi.yml
- filename: simple-ai-call-notes-api-openapi.yml
  format: yaml
  label: Simple AI Call Notes API
  slug: simple-ai-call-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-call-notes-api-openapi.yml
- filename: simple-ai-call-tags-api-openapi.yml
  format: yaml
  label: Simple AI Call Tags API
  slug: simple-ai-call-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-call-tags-api-openapi.yml
- filename: simple-ai-calls-api-openapi.yml
  format: yaml
  label: Simple AI Calls API
  slug: simple-ai-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-calls-api-openapi.yml
- filename: simple-ai-contacts-api-openapi.yml
  format: yaml
  label: Simple AI Contacts API
  slug: simple-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-contacts-api-openapi.yml
- filename: simple-ai-custom-data-api-openapi.yml
  format: yaml
  label: Simple AI Custom Data API
  slug: simple-ai-custom-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-custom-data-api-openapi.yml
- filename: simple-ai-external-calls-api-openapi.yml
  format: yaml
  label: Simple AI External Calls API
  slug: simple-ai-external-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-external-calls-api-openapi.yml
- filename: simple-ai-feedback-api-openapi.yml
  format: yaml
  label: Simple AI Feedback API
  slug: simple-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-feedback-api-openapi.yml
- filename: simple-ai-interactions-api-openapi.yml
  format: yaml
  label: Simple AI Interactions API
  slug: simple-ai-interactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-interactions-api-openapi.yml
- filename: simple-ai-journeys-api-openapi.yml
  format: yaml
  label: Simple AI Journeys API
  slug: simple-ai-journeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-journeys-api-openapi.yml
- filename: simple-ai-numbers-api-openapi.yml
  format: yaml
  label: Simple AI Numbers API
  slug: simple-ai-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-numbers-api-openapi.yml
- filename: simple-ai-voices-api-openapi.yml
  format: yaml
  label: Simple AI Voices API
  slug: simple-ai-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-voices-api-openapi.yml
- filename: simple-ai-webhooks-api-openapi.yml
  format: yaml
  label: Simple AI Webhooks API
  slug: simple-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simple-ai/openapi/simple-ai-webhooks-api-openapi.yml
consequence_counts:
  read: 27
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Simple Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 58
overview: 'Simple AI exposes 58 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 31 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Simple AI
provider_slug: simple-ai
slug: simple-ai-agentic-access
source_filename: simple-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/simple-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 58\n  by_action_class:\n    acting: 31\n    connected: 27\n  by_consequence:\n    write: 31\n    read: 27\n  human_in_the_loop_required: 0\noperations:\n- path: /journeys/{key}/enrollments\n  method: post\n  operationId: enroll_contact_journeys_key_enrollments_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journeys/{key}/enrollments/cancel\n  method: post\n  operationId: cancel_enrollment_journeys_key_enrollments_cancel_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external_calls/upload_url\n  method: post\n  operationId: request_external_call_upload_url\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external_calls\n  method: get\n  operationId: list_external_calls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external_calls\n  method: post\n  operationId: create_external_call\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external_calls/{uuid}\n  method: get\n  operationId: get_external_call\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback/{uuid}/resolve\n  method: post\n  operationId: resolve_feedback_feedback__uuid__resolve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feedback/{uuid}/notes\n  method: post\n  operationId: add_feedback_note_feedback__uuid__notes_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feedback\n  method: get\n  operationId: list_feedback_feedback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls\n  method: post\n  operationId: create_call_calls_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls\n  method: get\n  operationId: list_calls_calls_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /calls/{uuid}\n  method: get\n  operationId: get_call_details_calls__uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{uuid}\n  method: delete\n  operationId: delete_call_calls__uuid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{uuid}/cancel\n  method: post\n  operationId: cancel_call_calls__uuid__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /calls/find_by_attribute\n  method: get\n  operationId: find_call_by_attribute_calls_find_by_attribute_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call_tags\n  method: get\n  operationId: list_call_tags_call_tags_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call_tags\n  method: post\n  operationId: create_call_tag_call_tags_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{uuid}/call_notes\n  method: get\n  operationId: list_call_notes_calls__uuid__call_notes_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{uuid}/call_notes\n  method: post\n  operationId: create_call_note_calls__uuid__call_notes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{uuid}/tags\n  method: patch\n  operationId: update_call_tags_calls__uuid__tags_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents\n  method: get\n  operationId: list_agents_agents_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}\n  method: get\n  operationId: get_agent_agents__agent_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers\n  method: get\n  operationId: list_numbers_numbers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers/{uuid}\n  method: get\n  operationId: get_number_details_numbers__uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers/{uuid}\n  method: patch\n  operationId: update_number_numbers__uuid__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/{uuid}\n  method: delete\n  operationId: delete_number_numbers__uuid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/search_available\n  method: get\n  operationId: search_available_numbers_numbers_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers/buy_number\n  method: post\n  operationId: buy_number_numbers_buy_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/{uuid}/assign_agent\n  method: post\n  operationId: assign_agent_numbers__uuid__assign_agent_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: create_webhook_webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: list_webhooks_webhooks_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{endpoint_id}\n  method: delete\n  operationId: delete_webhook_webhooks__endpoint_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /interactions\n  method: get\n  operationId: list_interactions_interactions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interactions/{uuid}\n  method: get\n  operationId: get_interaction_details_interactions__uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices\n\
  \  method: get\n  operationId: list_voices_voices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices/{uuid}\n  method: get\n  operationId: get_voice_details_voices__uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: get\n  operationId: list_contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactId}\n  method: get\n  operationId: get_contact_by_uuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactId}\n  method: delete\n  operationId: delete_contact_by_uuid\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/upsert\n  method: post\n  operationId: upsert_synced_contact_contacts_upsert_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/fields/{fieldKey}\n  method: delete\n  operationId: delete_synced_contact_field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /contacts/{phoneNumber}/data\n  method: put\n  operationId: replace_contact_data_contacts__phoneNumber__data_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{phoneNumber}/data\n  method: patch\n  operationId: merge_contact_data_contacts__phoneNumber__data_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{phoneNumber}/data\n  method: get\n  operationId: read_contact_data_contacts__phoneNumber__data_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{phoneNumber}/data\n  method: delete\n  operationId: delete_contact_data_contacts__phoneNumber__data_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/tables\n  method: get\n  operationId: list_custom_data_tables_data_tables_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/tables\n  method: post\n  operationId: create_custom_data_table_data_tables_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /data/tables/reference-tables\n  method: get\n  operationId: list_custom_data_reference_tables_data_tables_reference_tables_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/tables/{id}\n  method: patch\n  operationId: update_custom_data_table_data_tables__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/tables/{id}\n  method: delete\n  operationId: delete_custom_data_table_data_tables__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/query\n  method: post\n  operationId: query_custom_data_data_query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/facets/{table_name}\n  method: get\n  operationId: get_custom_data_facets_data_facets__table_name__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/{table_name}\n  method: get\n  operationId: list_custom_data_records_data__table_name__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/{table_name}\n  method: put\n  operationId: create_custom_data_record_data__table_name__put\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/{table_name}\n  method: delete\n  operationId: delete_all_custom_data_records_data__table_name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/{table_name}/{id}\n  method: get\n  operationId: get_custom_data_record_data__table_name___id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/{table_name}/{id}\n  method: patch\n  operationId: update_custom_data_record_data__table_name___id__patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/{table_name}/{id}\n  method: delete\n  operationId: delete_custom_data_record_data__table_name___id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/simple-ai/agentic-access/simple-ai-agentic-access.yml
summary_line: 58 operations · 31 acting
tags:
- Artificial Intelligence
- Voice
- Telephony
- Software-as-a-Service
- Automation
- Contact Center
---
