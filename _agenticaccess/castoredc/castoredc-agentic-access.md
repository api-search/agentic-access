---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 27
api_specs:
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Studies API
  slug: castoredc-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Participants (Records) API
  slug: castoredc-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Institutes API
  slug: castoredc-institutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Users API
  slug: castoredc-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Fields API
  slug: castoredc-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Study Data Points API
  slug: castoredc-study-data-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Reports (Repeating Data) API
  slug: castoredc-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Surveys API
  slug: castoredc-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Audit Trail API
  slug: castoredc-audit-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Data Export API
  slug: castoredc-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
consequence_counts:
  physical: 1
  read: 27
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Castoredc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /study/{study_id}/participant/{participant_id}/data-points/survey-package-instance
operation_count: 34
overview: 'Castor exposes 34 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Castor
provider_slug: castoredc
slug: castoredc-agentic-access
source_filename: castoredc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/castoredc-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    acting: 7\n    connected: 27\n  by_consequence:\n    write: 6\n    read: 27\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study\n  method: get\n  operationId: listStudies\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}\n  method: get\n  operationId: getStudy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/participant\n  method: get\n  operationId: listParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/participant\n  method: post\n  operationId: createParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/{study_id}/participant/{participant_id}\n  method: get\n  operationId: getParticipant\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/institute\n  method: get\n  operationId: listInstitutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/institute\n  method: post\n  operationId: createInstitute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/{study_id}/institute/{institute_id}\n  method: get\n  operationId: getInstitute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method:\
  \ get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{user_id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/user\n  method: get\n  operationId: listStudyUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/field\n  method: get\n  operationId: listFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/field/{field_id}\n  method: get\n  operationId: getField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/field-dependency\n  method: get\n  operationId: listFieldDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/field-optiongroup\n  method: get\n  operationId: listFieldOptionGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/field-validation\n  method: get\n  operationId: listFieldValidations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/data-points/study\n  method: get\n  operationId: listStudyDataPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/participant/{participant_id}/data-points/study\n  method: get\n  operationId: listParticipantStudyDataPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/participant/{participant_id}/data-points/study\n  method: post\n  operationId: updateParticipantStudyDataPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/{study_id}/report\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/report/{report_id}\n\
  \  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/participant/{participant_id}/data-points/repeating-data-instance\n  method: get\n  operationId: listRepeatingDataInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/participant/{participant_id}/data-points/repeating-data-instance/{repeating_data_instance_id}\n  method: post\n  operationId: updateRepeatingDataInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/{study_id}/survey\n  method: get\n  operationId:\
  \ listSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/participant/{participant_id}/data-points/survey-instance\n  method: get\n  operationId: listSurveyInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/participant/{participant_id}/data-points/survey-package-instance\n  method: post\n  operationId: createSurveyPackageInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/{study_id}/compliance\n  method: post\n  operationId: getSurveyCompliance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /study/{study_id}/audit-trail\n  method: get\n  operationId: getAuditTrail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/export/data\n  method: get\n  operationId: exportStudyData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/export/structure\n  method: get\n  operationId: exportStudyStructure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /study/{study_id}/export/optiongroups\n\
  \  method: get\n  operationId: exportOptionGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country/{country_id}\n  method: get\n  operationId: getCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/agentic-access/castoredc-agentic-access.yml
summary_line: 34 operations · 7 acting
tags:
- Clinical Trials
- Electronic Data Capture
- EDC
- Clinical Data Management
- Healthcare
- Life Sciences
- Research
---
