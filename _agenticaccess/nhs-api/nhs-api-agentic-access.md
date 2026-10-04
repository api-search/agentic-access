---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 28
api_specs:
- filename: nhs-api-codesystem-api-openapi.yml
  format: yaml
  label: NHS API CodeSystem API
  slug: nhs-api-codesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-codesystem-api-openapi.yml
- filename: nhs-api-list-id-api-openapi.yml
  format: yaml
  label: NHS API List{id} API
  slug: nhs-api-list-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-list-id-api-openapi.yml
- filename: nhs-api-metadata-api-openapi.yml
  format: yaml
  label: NHS API Metadata API
  slug: nhs-api-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-metadata-api-openapi.yml
- filename: nhs-api-organization-api-openapi.yml
  format: yaml
  label: NHS API Organization API
  slug: nhs-api-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-organization-api-openapi.yml
- filename: nhs-api-organizationaffiliation-api-openapi.yml
  format: yaml
  label: NHS API OrganizationAffiliation API
  slug: nhs-api-organizationaffiliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-organizationaffiliation-api-openapi.yml
- filename: nhs-api-r4-api-openapi.yml
  format: yaml
  label: NHS API R4 API
  slug: nhs-api-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-r4-api-openapi.yml
- filename: nhs-api-stu3-api-openapi.yml
  format: yaml
  label: NHS API STU3 API
  slug: nhs-api-stu3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-stu3-api-openapi.yml
- filename: nhs-api-valueset-api-openapi.yml
  format: yaml
  label: NHS API ValueSet API
  slug: nhs-api-valueset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/openapi/nhs-api-valueset-api-openapi.yml
consequence_counts:
  physical: 3
  read: 28
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nhs Api Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /STU3/CommunicationRequest/{ubrn}/$ers.sendCommunicationToRequester
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /STU3/ReferralRequest/$ers.createReferralAndSendForTriage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /STU3/ReferralRequest/{ubrn}/$ers.changeShortlistAndSendForTriage
operation_count: 50
overview: 'NHS API exposes 50 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 19 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NHS API
provider_slug: nhs-api
slug: nhs-api-agentic-access
source_filename: nhs-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/nhs-api-codesystem-api-openapi.yml, openapi/nhs-api-list-id-api-openapi.yml,\n  openapi/nhs-api-metadata-api-openapi.yml, openapi/nhs-api-organization-api-openapi.yml, openapi/nhs-api-organizationaffiliation-api-openapi.yml,\n  openapi/nhs-api-r4-api-openapi.yml, openapi/nhs-api-stu3-api-openapi.yml, openapi/nhs-api-valueset-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    connected: 28\n    acting: 22\n  by_consequence:\n    read: 28\n    write: 19\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /CodeSystem/\n  method: get\n  operationId: search-codesystem\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CodeSystem/{id}\n  method: get\n  operationId: get-codesystem-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /List{id}\n  method: get\n  operationId: get-deletion-notices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: get-capability-statement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization\n  method: get\n  operationId: get-organization-resources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization/{id}\n  method:\
  \ get\n  operationId: get-single-organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OrganizationAffiliation/{id}\n  method: get\n  operationId: get-single-organizationaffiliation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organizationaffiliation\n  method: get\n  operationId: get-organizationaffiliation-resources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /R4/Binary/{id}\n  method: get\n  operationId: getR4BinaryById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /R4/PractitionerRole\n  method: get\n  operationId: getR4PractitionerRole\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /R4/HealthcareService/{id}\n  method: get\n  operationId: getR4HealthcareServiceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /R4/HealthcareService/{id}\n  method: head\n  operationId: headR4HealthcareServiceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /R4/HealthcareService\n  method: get\n  operationId: getR4HealthcareService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /R4/Practitioner\n  method: get\n  operationId: getR4Practitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /R4/ServiceRequest\n  method: get\n  operationId: getR4ServiceRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/CodeSystem/{codeSystemType}\n  method: get\n  operationId: getSTU3CodeSystemByCodeSystemType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/ReferralRequest/$ers.fetchworklist\n  method: post\n  operationId: postSTU3ReferralRequest$ersFetchworklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/{ubrn}\n  method: get\n  operationId:\
  \ getSTU3ReferralRequestByUbrn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/Task\n  method: get\n  operationId: getSTU3Task\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/ReferralRequest/{ubrn}/_history/{version}\n  method: get\n  operationId: getSTU3ReferralRequestByUbrnHistoryByVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/Binary/{attachmentLogicalID}\n  method: get\n  operationId: getSTU3BinaryByAttachmentLogicalID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/ReferralRequest/{ubrn}/$ers.generateCRI\n  method: post\n  operationId:\
  \ postSTU3ReferralRequestByUbrn$ersGenerateCRI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/HealthcareService/$ers.searchHealthcareServicesForPatient\n  method: post\n  operationId: postSTU3HealthcareService$ersSearchHealthcareServicesForPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/$ers.createReferral\n  method: post\n  operationId: postSTU3ReferralRequest$ersCreateReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/$ers.createReferralAndSendForTriage\n  method: post\n  operationId: postSTU3ReferralRequest$ersCreateReferralAndSendForTriage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/Slot\n  method: get\n  operationId: getSTU3Slot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/Appointment\n  method: post\n  operationId: postSTU3Appointment\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/Binary\n  method: post\n  operationId: postSTU3Binary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/{ubrn}/$ers.maintainReferralLetter\n  method: post\n  operationId: postSTU3ReferralRequestByUbrn$ersMaintainReferralLetter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /STU3/ReferralRequest/{ubrn}/$ers.acceptReferral\n  method: post\n  operationId: postSTU3ReferralRequestByUbrn$ersAcceptReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/{ubrn}/$ers.rejectReferral\n  method: post\n  operationId: postSTU3ReferralRequestByUbrn$ersRejectReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/{ubrn}/$ers.generatePatientLetter\n  method: post\n  operationId: postSTU3ReferralRequestByUbrn$ersGeneratePatientLetter\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/{ubrn}/$ers.cancelAppointmentActionLater\n  method: post\n  operationId: postSTU3ReferralRequestByUbrn$ersCancelAppointmentActionLater\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/CommunicationRequest/$ers.fetchworklist\n  method: post\n  operationId: postSTU3CommunicationRequest$ersFetchworklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/CommunicationRequest/{ubrn}\n  method: get\n  operationId: getSTU3CommunicationRequestByUbrn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/CommunicationRequest/{ubrn}/_history/{version}\n  method: get\n  operationId: getSTU3CommunicationRequestByUbrnHistoryByVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/Communication\n  method: get\n  operationId: getSTU3Communication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/CommunicationRequest/{ubrn}/$ers.sendCommunicationToRequester\n  method: post\n  operationId: postSTU3CommunicationRequestByUbrn$ersSendCommunicationToRequester\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/$ers.createFromCommunicationRequestActionLater\n  method: post\n  operationId: postSTU3ReferralRequest$ersCreateFromCommunicationRequestActionLater\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/{ubrn}/$ers.recordReviewOutcome\n  method: post\n  operationId: postSTU3ReferralRequestByUbrn$ersRecordReviewOutcome\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/{ubrn}/$ers.changeShortlist\n  method: post\n  operationId: postSTU3ReferralRequestByUbrn$ersChangeShortlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/ReferralRequest/{ubrn}/$ers.changeShortlistAndSendForTriage\n  method: post\n  operationId: postSTU3ReferralRequestByUbrn$ersChangeShortlistAndSendForTriage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/Appointment/{id}\n  method: put\n  operationId: putSTU3AppointmentById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/Appointment/{id}\n  method: get\n  operationId: getSTU3AppointmentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /STU3/Appointment/{id}/_history/{version}\n  method: get\n  operationId: getSTU3AppointmentByIdHistoryByVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /STU3/ReferralRequest/{ubrn}/$ers.cancelReferral\n  method: post\n  operationId: postSTU3ReferralRequestByUbrn$ersCancelReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/CommunicationRequest/{ubrn}/$ers.generateCRI\n  method: post\n  operationId: postSTU3CommunicationRequestByUbrn$ersGenerateCRI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /STU3/CommunicationRequest/$ers.createAdviceAndGuidance\n  method: post\n  operationId: postSTU3CommunicationRequest$ersCreateAdviceAndGuidance\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ValueSet/\n  method: post\n  operationId: search-ods-organization-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ValueSet/{id}\n  method: get\n  operationId: get-valueset-specified-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhs-api/refs/heads/main/agentic-access/nhs-api-agentic-access.yml
summary_line: 50 operations · 22 acting
tags:
- Healthcare
- FHIR
- NHS
- United Kingdom
- HL7
- Electronic Prescriptions
- Patient Demographics
- GP Connect
- NHS Login
- Interoperability
---
