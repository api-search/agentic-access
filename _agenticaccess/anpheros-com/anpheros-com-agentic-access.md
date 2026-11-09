---
acting_count: 58
action_class_counts:
  acting: 58
  connected: 82
api_specs:
- filename: anpheros-com-access-requests-api-openapi.yml
  format: yaml
  label: anpheros-com Access requests API
  slug: anpheros-com-access-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-access-requests-api-openapi.yml
- filename: anpheros-com-admin-api-openapi.yml
  format: yaml
  label: anpheros-com Admin API
  slug: anpheros-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-admin-api-openapi.yml
- filename: anpheros-com-anpheros-search-api-openapi.yml
  format: yaml
  label: anpheros-com Anpheros Search API
  slug: anpheros-com-anpheros-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-anpheros-search-api-openapi.yml
- filename: anpheros-com-fhir-r4-api-openapi.yml
  format: yaml
  label: anpheros-com FHIR R4 API
  slug: anpheros-com-fhir-r4-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-fhir-r4-api-openapi.yml
- filename: anpheros-com-icd-10-to-icd-11-api-openapi.yml
  format: yaml
  label: anpheros-com ICD-10 to ICD-11 API
  slug: anpheros-com-icd-10-to-icd-11-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-icd-10-to-icd-11-api-openapi.yml
- filename: anpheros-com-oauth-api-openapi.yml
  format: yaml
  label: anpheros-com OAuth API
  slug: anpheros-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-oauth-api-openapi.yml
- filename: anpheros-com-patient-me-api-openapi.yml
  format: yaml
  label: anpheros-com Patient (me) API
  slug: anpheros-com-patient-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-patient-me-api-openapi.yml
- filename: anpheros-com-rest-v1-api-openapi.yml
  format: yaml
  label: anpheros-com REST v1 API
  slug: anpheros-com-rest-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-rest-v1-api-openapi.yml
- filename: anpheros-com-smart-health-links-api-openapi.yml
  format: yaml
  label: anpheros-com SMART Health Links API
  slug: anpheros-com-smart-health-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-smart-health-links-api-openapi.yml
- filename: anpheros-com-webhooks-api-openapi.yml
  format: yaml
  label: anpheros-com Webhooks API
  slug: anpheros-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 5
  read: 82
  safety-critical: 8
  write: 45
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Anpheros Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/applications/{application_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/projects/{project_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/projects/{project_id}/sandbox/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /me/patients/{patient_id}/grants/{grant_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /me/patients/{patient_id}/shl/{link_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/webhooks/{endpoint_id}/rotate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/webhooks/{endpoint_id}/deliveries/{delivery_id}/redeliver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/webhooks/{endpoint_id}/ping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{endpoint_id}/deliveries/redeliver-exhausted
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{endpoint_id}/deliveries/{delivery_id}/redeliver
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{endpoint_id}/ping
operation_count: 140
overview: 'anpheros-com exposes 140 API operations that an AI agent could call, of which 58 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 82 read, 45 write, 5 physical, and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: anpheros-com
provider_slug: anpheros-com
slug: anpheros-com-agentic-access
source_filename: anpheros-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/anpheros-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 140\n  by_action_class:\n    connected: 82\n    acting: 58\n  by_consequence:\n    read: 82\n    write: 45\n    safety-critical: 8\n    physical: 5\n  human_in_the_loop_required: 8\noperations:\n- path: /oauth/authorize\n  method: get\n  operationId: authorize_oauth_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: token_oauth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/revoke\n  method: post\n  operationId: revoke_oauth_revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /fhir/R4/metadata\n  method: get\n  operationId: metadata_fhir_R4_metadata_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/CodeSystem/$lookup\n  method: get\n  operationId: codesystem_lookup_fhir_R4_CodeSystem__lookup_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/ConceptMap/$translate\n  method: get\n  operationId: conceptmap_translate_fhir_R4_ConceptMap__translate_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/ValueSet/$expand\n\
  \  method: get\n  operationId: valueset_expand_by_url_fhir_R4_ValueSet__expand_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/CodeSystem\n  method: get\n  operationId: search_fhir_R4_CodeSystem_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n\
  \    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/CodeSystem/{rid}\n  method: get\n  operationId: read_fhir_R4_CodeSystem__rid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/ValueSet\n  method: get\n  operationId: search_fhir_R4_ValueSet_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n\
  \    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/ValueSet/{rid}\n  method: get\n  operationId: read_fhir_R4_ValueSet__rid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/ConceptMap\n  method: get\n  operationId: search_fhir_R4_ConceptMap_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/ConceptMap/{rid}\n  method: get\n  operationId: read_fhir_R4_ConceptMap__rid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4\n  method: post\n  operationId: transaction_fhir_R4_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/R4/Patient/{rid}/$everything\n  method: get\n  operationId: everything_fhir_R4_Patient__rid___everything_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n\
  \    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/Patient/{rid}/$summary\n  method: get\n  operationId: summary_fhir_R4_Patient__rid___summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/{resource_type}/$validate\n  method: post\n  operationId: validate_resource_fhir_R4__resource_type___validate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/R4/{resource_type}\n  method: get\n  operationId: search_fhir_R4__resource_type__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n\
  \    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/{resource_type}\n  method: post\n  operationId: create_fhir_R4__resource_type__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/R4/{resource_type}/{rid}\n  method: get\n  operationId: read_fhir_R4__resource_type___rid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/{resource_type}/{rid}\n  method: put\n  operationId: update_fhir_R4__resource_type___rid__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/R4/{resource_type}/{rid}\n  method: delete\n  operationId: delete_fhir_R4__resource_type___rid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/R4/{resource_type}/{rid}/_history\n  method: get\n  operationId: history_fhir_R4__resource_type___rid___history_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/R4/{resource_type}/{rid}/_history/{vid}\n  method: get\n  operationId: vread_fhir_R4__resource_type___rid___history__vid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/patients\n  method: get\n  operationId: list_patients_v1_patients_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients\n  method: post\n  operationId: create_patient_v1_patients_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n\
  \    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patients/{patient_id}\n  method: get\n  operationId: read_patient_v1_patients__patient_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patient_id}\n  method: put\n  operationId: update_patient_v1_patients__patient_id__put\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patients/{patient_id}/observations\n  method: get\n  operationId: list_observations_v1_patients__patient_id__observations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n\
  \    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patient_id}/observations\n  method: post\n  operationId: create_observations_v1_patients__patient_id__observations_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/observations/{item_id}\n  method: get\n  operationId: read_observations_v1_observations__item_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/observations/{item_id}\n  method: delete\n  operationId: delete_observations_v1_observations__item_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patients/{patient_id}/conditions\n  method: get\n  operationId: list_conditions_v1_patients__patient_id__conditions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patient_id}/conditions\n  method: post\n  operationId: create_conditions_v1_patients__patient_id__conditions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conditions/{item_id}\n  method: get\n  operationId: read_conditions_v1_conditions__item_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n\
  \    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conditions/{item_id}\n  method: delete\n  operationId: delete_conditions_v1_conditions__item_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patients/{patient_id}/medications\n  method: get\n  operationId: list_medications_v1_patients__patient_id__medications_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patient_id}/medications\n  method: post\n  operationId: create_medications_v1_patients__patient_id__medications_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/medications/{item_id}\n  method: get\n  operationId: read_medications_v1_medications__item_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/medications/{item_id}\n  method: delete\n  operationId: delete_medications_v1_medications__item_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n\
  \    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patients/{patient_id}/documents\n  method: get\n  operationId: list_documents_v1_patients__patient_id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patient_id}/documents\n  method: post\n  operationId: create_document_v1_patients__patient_id__documents_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{doc_id}\n  method: get\n  operationId: read_document_v1_documents__doc_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{doc_id}/content\n  method: put\n  operationId: upload_content_v1_documents__doc_id__content_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{doc_id}/content\n  method: get\n  operationId: download_content_v1_documents__doc_id__content_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{doc_id}/finalize\n  method: post\n  operationId: finalize_document_v1_documents__doc_id__finalize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n  \
  \  - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patients/{patient_id}/grants\n  method: get\n  operationId: patient_grants_v1_patients__patient_id__grants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/context\n  method: post\n  operationId: context_v1_context_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patients/{patient_id}/patterns\n  method: get\n  operationId: patterns_v1_patients__patient_id__patterns_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n\
  \    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patient_id}/patterns/{finding_id}\n  method: get\n  operationId: pattern_v1_patients__patient_id__patterns__finding_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patient_id}/patterns/{finding_id}/evidence\n  method: get\n  operationId:\
  \ pattern_evidence_v1_patients__patient_id__patterns__finding_id__evidence_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patient_id}/series\n  method: get\n  operationId: series_v1_patients__patient_id__series_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n\
  \    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patients/{patient_id}/patterns/compare\n  method: post\n  operationId: pattern_compare_v1_patients__patient_id__patterns_compare_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/terminology/symptoms\n  method: get\n  operationId: symptom_concepts_v1_terminology_symptoms_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - anpheros/patterns\n    - fhirUser\n    - offline_access\n    - openid\n    - patient/*.rs\n    - patient/AllergyIntolerance.rs\n    - patient/Condition.rs\n    - patient/DocumentReference.rs\n    - patient/MedicationStatement.rs\n    - patient/Observation.rs\n    - patient/Observation.rs?category=laboratory\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (67 KB total) ---\n# Full source: https://artifacts.apis.io/anpheros-com/agentic-access/anpheros-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/anpheros-com/agentic-access/anpheros-com-agentic-access.yml
summary_line: 140 operations · 58 acting · 8 human-in-the-loop
tags:
- Health
- Digital Health
- FHIR
- Medical Records
---
