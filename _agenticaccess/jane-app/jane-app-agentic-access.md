---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 28
api_specs:
- filename: jane-app-appointments-api-openapi.yml
  format: yaml
  label: Jane Appointments API
  slug: jane-app-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-appointments-api-openapi.yml
- filename: jane-app-careplans-api-openapi.yml
  format: yaml
  label: Jane Care Plans API
  slug: jane-app-careplans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-careplans-api-openapi.yml
- filename: jane-app-catalog-api-openapi.yml
  format: yaml
  label: Jane Catalog API
  slug: jane-app-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-catalog-api-openapi.yml
- filename: jane-app-company-api-openapi.yml
  format: yaml
  label: Jane Company API
  slug: jane-app-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-company-api-openapi.yml
- filename: jane-app-disciplines-api-openapi.yml
  format: yaml
  label: Jane Disciplines API
  slug: jane-app-disciplines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-disciplines-api-openapi.yml
- filename: jane-app-documentuploads-api-openapi.yml
  format: yaml
  label: Jane Document Uploads API
  slug: jane-app-documentuploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-documentuploads-api-openapi.yml
- filename: jane-app-extensions-api-openapi.yml
  format: yaml
  label: Jane Extensions API
  slug: jane-app-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-extensions-api-openapi.yml
- filename: jane-app-locations-api-openapi.yml
  format: yaml
  label: Jane Locations API
  slug: jane-app-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-locations-api-openapi.yml
- filename: jane-app-medications-api-openapi.yml
  format: yaml
  label: Jane Medications API
  slug: jane-app-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-medications-api-openapi.yml
- filename: jane-app-observations-api-openapi.yml
  format: yaml
  label: Jane Observations API
  slug: jane-app-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-observations-api-openapi.yml
- filename: jane-app-patients-api-openapi.yml
  format: yaml
  label: Jane Patients API
  slug: jane-app-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-patients-api-openapi.yml
- filename: jane-app-staffmembers-api-openapi.yml
  format: yaml
  label: Jane Staff Members API
  slug: jane-app-staffmembers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-staffmembers-api-openapi.yml
- filename: jane-app-treatments-api-openapi.yml
  format: yaml
  label: Jane Treatments API
  slug: jane-app-treatments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-treatments-api-openapi.yml
- filename: jane-app-webhooks-api-openapi.yml
  format: yaml
  label: Jane Webhooks API
  slug: jane-app-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/openapi/jane-app-webhooks-api-openapi.yml
consequence_counts:
  read: 28
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jane App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 43
overview: 'Jane exposes 43 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jane
provider_slug: jane-app
slug: jane-app-agentic-access
source_filename: jane-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/jane-app-jdp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    acting: 15\n    connected: 28\n  by_consequence:\n    write: 15\n    read: 28\n  human_in_the_loop_required: 0\noperations:\n- path: /api/2026-01-01/medical-record/care-plans\n  method: post\n  operationId: createCarePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - care_plans:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/medical-record/care-plans\n \
  \ method: get\n  operationId: listCarePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - care_plans:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/care-plans/{care_plan_id}/activities\n  method: post\n  operationId: createCarePlanActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - care_plans:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2025-02-28-beta/extensions\n  method: post\n  operationId: createExtension\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /api/2025-02-28-beta/extensions\n  method: get\n  operationId: getExtensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/medications\n  method: post\n  operationId: createMedication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - medications:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/medical-record/medications\n  method: get\n  operationId: listMedications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - medications:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/observations\n\
  \  method: post\n  operationId: createObservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - observations:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/medical-record/observations\n  method: get\n  operationId: listObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - observations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2025-02-28-beta/extensions/{extension_id}\n  method: delete\n  operationId: deleteExtension\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/2025-02-28-beta/extensions/{extension_id}\n  method: get\n  operationId: getExtension\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2025-02-28-beta/extensions/{extension_id}\n  method: put\n  operationId: updateExtension\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/webhooks/{webhook_id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/appointments/{appointment_id}\n  method: get\n  operationId: getAnAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - appointments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/staff_members/{staff_member_id}\n  method: get\n  operationId: getAStaffMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - staff_members:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/care-plans/{care_plan_id}\n  method: get\n  operationId: getCarePlan\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - care_plans:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/care-plans/{care_plan_id}\n  method: patch\n  operationId: updateCarePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - care_plans:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/medical-record/care-plans/{care_plan_id}/activities/{care_plan_activity_id}\n  method: get\n  operationId: getCarePlanActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - care_plans:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/care-plans/{care_plan_id}/activities/{care_plan_activity_id}\n\
  \  method: patch\n  operationId: updateCarePlanActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - care_plans:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2025-02-28-beta/catalog/extensions/{id}\n  method: get\n  operationId: getCatalogExtension\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2025-02-28-beta/catalog/extensions\n  method: get\n  operationId: getCatalogExtensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/company\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - companies:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/disciplines/{discipline_id}\n  method: get\n  operationId: getDiscipline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - disciplines:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/document-uploads/{document_id}\n  method: get\n  operationId: getDocumentUploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - document_uploads:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/locations/{location_id}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - locations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/locations\n  method:\
  \ get\n  operationId: getLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - locations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/medications/{medication_id}\n  method: get\n  operationId: getMedication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - medications:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/medications/{medication_id}\n  method: patch\n  operationId: updateMedication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - medications:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/medical-record/medications/{medication_id}/history\n\
  \  method: get\n  operationId: getMedicationHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - medications:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/observations/{observation_id}\n  method: get\n  operationId: getObservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - observations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/medical-record/observations/{observation_id}\n  method: patch\n  operationId: updateObservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - observations:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/patients/{patient_id}\n\
  \  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patients:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/patients\n  method: get\n  operationId: getPatients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - patients:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/treatments/{id}\n  method: get\n  operationId: getTreatment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - treatments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/2026-01-01/webhooks\n  method: post\n  operationId: postWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/appointments\n  method: get\n  operationId: listAppointmentsVersioned\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - appointments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/disciplines\n  method: get\n  operationId: listDisciplinesVersioned\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - disciplines:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/staff_members\n  method: get\n \
  \ operationId: listStaffMembersVersioned\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - staff_members:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/treatments\n  method: get\n  operationId: listTreatmentsVersioned\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - treatments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/2026-01-01/document-uploads\n  method: post\n  operationId: postDocumentUploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - document_uploads:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/2026-01-01/patients/search\n  method: post\n  operationId: searchPatients\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - patients:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jane-app/refs/heads/main/agentic-access/jane-app-agentic-access.yml
summary_line: 43 operations · 15 acting
tags:
- Healthcare
- Canada
- Practice Management
- EHR
- EMR
- Scheduling
- Clinical Documentation
- Telehealth
- Health and Wellness
- REST API
- Authentication
- Webhook
---
