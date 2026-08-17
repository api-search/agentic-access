---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 21
api_specs:
- filename: zocdoc-appointments-api-openapi.yml
  format: yaml
  label: Zocdoc appointments API
  slug: zocdoc-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-appointments-api-openapi.yml
- filename: zocdoc-calendar-integration-timeslots-api-openapi.yml
  format: yaml
  label: Zocdoc calendar-integration-timeslots API
  slug: zocdoc-calendar-integration-timeslots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml
- filename: zocdoc-credentials-api-openapi.yml
  format: yaml
  label: Zocdoc credentials API
  slug: zocdoc-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-credentials-api-openapi.yml
- filename: zocdoc-facilities-api-openapi.yml
  format: yaml
  label: Zocdoc facilities API
  slug: zocdoc-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-facilities-api-openapi.yml
- filename: zocdoc-insurance-reference-api-openapi.yml
  format: yaml
  label: Zocdoc insurance-reference API
  slug: zocdoc-insurance-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-insurance-reference-api-openapi.yml
- filename: zocdoc-provider-locations-api-openapi.yml
  format: yaml
  label: Zocdoc provider-locations API
  slug: zocdoc-provider-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-provider-locations-api-openapi.yml
- filename: zocdoc-providers-api-openapi.yml
  format: yaml
  label: Zocdoc providers API
  slug: zocdoc-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-providers-api-openapi.yml
- filename: zocdoc-reference-api-openapi.yml
  format: yaml
  label: Zocdoc reference API
  slug: zocdoc-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-reference-api-openapi.yml
- filename: zocdoc-schedulable-entities-api-openapi.yml
  format: yaml
  label: Zocdoc schedulable-entities API
  slug: zocdoc-schedulable-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-schedulable-entities-api-openapi.yml
- filename: zocdoc-webhook-api-openapi.yml
  format: yaml
  label: Zocdoc webhook API
  slug: zocdoc-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-webhook-api-openapi.yml
- filename: zocdoc-reviews-api-openapi.yml
  format: yaml
  label: Zocdoc reviews API
  slug: zocdoc-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-reviews-api-openapi.yml
- filename: zocdoc-specialties-api-openapi.yml
  format: yaml
  label: Zocdoc specialties API
  slug: zocdoc-specialties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-specialties-api-openapi.yml
- filename: zocdoc-visit-reasons-api-openapi.yml
  format: yaml
  label: Zocdoc visit-reasons API
  slug: zocdoc-visit-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-visit-reasons-api-openapi.yml
consequence_counts:
  read: 21
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zocdoc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Zocdoc exposes 32 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zocdoc
provider_slug: zocdoc
slug: zocdoc-agentic-access
source_filename: zocdoc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: generated\nsource: openapi/zocdoc-appointments-api-openapi.yml, openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml,\n  openapi/zocdoc-credentials-api-openapi.yml, openapi/zocdoc-facilities-api-openapi.yml, openapi/zocdoc-insurance-reference-api-openapi.yml,\n  openapi/zocdoc-provider-locations-api-openapi.yml, openapi/zocdoc-providers-api-openapi.yml,\n  openapi/zocdoc-reference-api-openapi.yml, openapi/zocdoc-reviews-api-openapi.yml, openapi/zocdoc-schedulable-entities-api-openapi.yml,\n  openapi/zocdoc-specialties-api-openapi.yml, openapi/zocdoc-visit-reasons-api-openapi.yml,\n  openapi/zocdoc-webhook-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting:\
  \ 11\n    connected: 21\n  by_consequence:\n    write: 11\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/appointments\n  method: post\n  operationId: createAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - external.appointment.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appointments\n  method: get\n  operationId: getAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - external.appointment.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appointments/{appointment_id}\n  method: get\n  operationId: getAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - external.appointment.read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appointments/{appointment_id}/participants\n  method: get\n  operationId: getAppointmentParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - external.appointment.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appointments/cancel\n  method: post\n  operationId: cancelAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - external.appointment.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appointments/confirm\n  method: post\n  operationId: confirmAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - external.appointment.write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appointments/reschedule\n  method: post\n  operationId: rescheduleAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - external.appointment.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appointments/{appointment_id}/attachments\n  method: post\n  operationId: uploadAppointmentAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - external.appointment.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/appointments/update-status\n  method: put\n  operationId: updateAppointmentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - external.appointment.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/providers/{provider_id}/calendar/timeslots\n  method: get\n  operationId: getProviderCalendarTimeslots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/providers/{provider_id}/calendar/timeslots\n  method: put\n  operationId: putProviderCalendarTimeslots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials/rotate\n  method: post\n  operationId: rotateCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - external.credential.rotate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1-beta/facilities\n  method: get\n  operationId: getFacilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1-beta/facilities/{facility_id}\n  method: get\n  operationId: getFacility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insurance_plans\n  method: get\n  operationId:\
  \ getInsurancePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insurance_plans/{insurance_plan_id}\n  method: get\n  operationId: getInsurancePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provider_locations\n  method: get\n  operationId: getProviderLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provider_locations/{provider_location_id}\n  method: get\n  operationId: getProviderLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provider_locations/availability\n  method: get\n  operationId: getProviderLocationsAvailability\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provider_locations/{provider_location_id}/insurance_mappings\n  method: get\n  operationId: getProviderLocationInsuranceMappings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/provider_locations/{provider_location_id}/insurance_mappings\n  method: post\n  operationId: updateProviderLocationInsuranceMappings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - external.provider_insurance.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/providers\n  method: get\n  operationId: getProviders\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reference/npi\n  method: get\n  operationId: getProviderNpis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/providers/{provider_id}/reviews\n  method: get\n  operationId: getProviderReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/providers/reviews\n  method: get\n  operationId: getProviderReviewsBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schedulable_entities\n  method: get\n  operationId: getSchedulableEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - external.schedulable_entity.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schedulable_entities/overlaps\n  method: put\n  operationId: putSchedulableEntitiesOverlaps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - external.schedulable_entity.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/specialties\n  method: get\n  operationId: getSpecialties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/specialties/{specialty_id}\n  method: get\n  operationId: getSpecialtyById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/visit_reasons\n\
  \  method: get\n  operationId: getVisitReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/visit_reasons/{visit_reason_id}\n  method: get\n  operationId: getVisitReasonById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/mock-request\n  method: post\n  operationId: mockWebhookRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/agentic-access/zocdoc-agentic-access.yml
summary_line: 32 operations · 11 acting
tags:
- Healthcare
- Appointments
- Booking
- Providers
- Insurance
- Telehealth
- Scheduling
---
