---
acting_count: 36
action_class_counts:
  acting: 36
  connected: 29
api_specs:
- filename: goodlord-agent-api-openapi.yml
  format: yaml
  label: Goodlord Agent API
  slug: goodlord-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-agent-api-openapi.yml
- filename: goodlord-application-api-openapi.yml
  format: yaml
  label: Goodlord Application API
  slug: goodlord-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-application-api-openapi.yml
- filename: goodlord-authentication-api-openapi.yml
  format: yaml
  label: Goodlord Authentication API
  slug: goodlord-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-authentication-api-openapi.yml
- filename: goodlord-company-api-openapi.yml
  format: yaml
  label: Goodlord Company API
  slug: goodlord-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-company-api-openapi.yml
- filename: goodlord-file-api-openapi.yml
  format: yaml
  label: Goodlord File API
  slug: goodlord-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-file-api-openapi.yml
- filename: goodlord-insuranceclaim-api-openapi.yml
  format: yaml
  label: Goodlord Insurance Claim API
  slug: goodlord-insuranceclaim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-insuranceclaim-api-openapi.yml
- filename: goodlord-media-api-openapi.yml
  format: yaml
  label: Goodlord Media API
  slug: goodlord-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-media-api-openapi.yml
- filename: goodlord-payment-api-openapi.yml
  format: yaml
  label: Goodlord Payment API
  slug: goodlord-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-payment-api-openapi.yml
- filename: goodlord-rentschedule-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule API
  slug: goodlord-rentschedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedule-api-openapi.yml
- filename: goodlord-rentschedulerow-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule Row API
  slug: goodlord-rentschedulerow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedulerow-api-openapi.yml
- filename: goodlord-rentschedulerowpostdto-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule Row Post Dto API
  slug: goodlord-rentschedulerowpostdto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedulerowpostdto-api-openapi.yml
- filename: goodlord-rentschedulerowupdate-api-openapi.yml
  format: yaml
  label: Goodlord Rent Schedule Row Update API
  slug: goodlord-rentschedulerowupdate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rentschedulerowupdate-api-openapi.yml
- filename: goodlord-role-api-openapi.yml
  format: yaml
  label: Goodlord Role API
  slug: goodlord-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-role-api-openapi.yml
- filename: goodlord-rolegroup-api-openapi.yml
  format: yaml
  label: Goodlord Role Group API
  slug: goodlord-rolegroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-rolegroup-api-openapi.yml
- filename: goodlord-subject-api-openapi.yml
  format: yaml
  label: Goodlord Subject API
  slug: goodlord-subject-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-subject-api-openapi.yml
consequence_counts:
  read: 29
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Goodlord Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 65
overview: 'Goodlord exposes 65 API operations that an AI agent could call, of which 36 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read and 36 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Goodlord
provider_slug: goodlord
slug: goodlord-agentic-access
source_filename: goodlord-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/goodlord-insurance-app-api-openapi.json, openapi/goodlord-referencing-api-openapi.json,\n  openapi/goodlord-referencing-api-sandbox-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    connected: 29\n    acting: 36\n  by_consequence:\n    read: 29\n    write: 36\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/agents\n  method: get\n  operationId: api_agents_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents\n  method: post\n  operationId: api_agents_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{id}\n  method: get\n  operationId: api_agents_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{id}\n  method: patch\n  operationId: api_agents_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me\n  method: get\n  operationId: get_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/companies\n  method: get\n  operationId: api_companies_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{id}\n  method: get\n  operationId: api_companies_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insurance_claims/{insuranceClaimId}/files\n  method: get\n  operationId: api_insurance_claims_insuranceClaimIdfiles_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insurance_claims/{insuranceClaimId}/files\n  method: post\n  operationId: api_insurance_claims_insuranceClaimIdfiles_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance_claims/{insuranceClaimId}/files/{id}\n  method: get\n  operationId: api_insurance_claims_insuranceClaimIdfiles_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insurance_claims/{insuranceClaimId}/files/{id}\n  method: delete\n  operationId: api_insurance_claims_insuranceClaimIdfiles_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance_claims\n  method: get\n  operationId: api_insurance_claims_get_collection\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insurance_claims\n  method: post\n  operationId: api_insurance_claims_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance_claims/{id}\n  method: get\n  operationId: api_insurance_claims_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insurance_claims/{id}\n  method: patch\n  operationId: api_insurance_claims_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance_claims/{id}/submit\n  method: post\n  operationId: api_insurance_claims_idsubmit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance_claims/{insuranceClaimId}/payments\n  method: get\n  operationId: api_insurance_claims_insuranceClaimIdpayments_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insurance_claims/{insuranceClaimId}/payments/{id}\n  method: get\n  operationId: api_insurance_claims_insuranceClaimIdpayments_id_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insurance_claims/{insuranceClaimId}/rent_schedule\n  method: get\n  operationId: api_insurance_claims_insuranceClaimIdrent_schedule_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insurance_claims/{insuranceClaimId}/rent_schedule/{rentScheduleId}/rent_schedule_rows\n  method: post\n  operationId: api_insurance_claims_insuranceClaimIdrent_schedule_rentScheduleIdrent_schedule_rows_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance_claims/{insuranceClaimId}/rent_schedule/{rentScheduleId}/submit\n\
  \  method: post\n  operationId: api_insurance_claims_insuranceClaimIdrent_schedule_rentScheduleIdsubmit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance_claims/{insuranceClaimId}/rent_schedule/{rentScheduleId}/rent_schedule_row/{id}\n  method: get\n  operationId: api_insurance_claims_insuranceClaimIdrent_schedule_rentScheduleIdrent_schedule_row_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insurance_claims/{insuranceClaimId}/rent_schedule/{rentScheduleId}/rent_schedule_row/{id}\n  method: delete\n  operationId: api_insurance_claims_insuranceClaimIdrent_schedule_rentScheduleIdrent_schedule_row_id_delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance_claims/{insuranceClaimId}/rent_schedule/{rentScheduleId}/rent_schedule_row/{id}\n  method: patch\n  operationId: api_insurance_claims_insuranceClaimIdrent_schedule_rentScheduleIdrent_schedule_row_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/insurance_claims/{insuranceClaimId}/rent_schedule/{rentScheduleId}/rent_schedule_row\n  method: post\n  operationId: api_insurance_claims_insuranceClaimIdrent_schedule_rentScheduleIdrent_schedule_row_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/roles\n  method: get\n  operationId: api_roles_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/roles\n  method: post\n  operationId: api_roles_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/roles/{id}\n  method: get\n  operationId: api_roles_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/roles/{id}\n  method: delete\n  operationId: api_roles_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/roles/{id}\n  method: patch\n  operationId: api_roles_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/role_groups\n  method: get\n  operationId: api_role_groups_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/role_groups\n  method: post\n  operationId: api_role_groups_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/role_groups/{id}\n  method: get\n  operationId: api_role_groups_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/role_groups/{id}\n  method: delete\n  operationId: api_role_groups_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/role_groups/{id}\n \
  \ method: patch\n  operationId: api_role_groups_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/token\n  method: post\n  operationId: getAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/application\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /referencing/application/{applicationId}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/application/{applicationId}\n  method: patch\n  operationId: patchApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/application/{applicationId}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /referencing/subject/{subjectId}/auth/token\n  method: get\n  operationId: getBotToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/subject/{subjectId}/auth/token\n  method: post\n  operationId: createBotToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/subject/{subjectId}\n  method: get\n  operationId: getSubject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/subject/{subjectId}\n  method: patch\n  operationId: patchSubject\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/subject/{subjectId}\n  method: delete\n  operationId: deleteSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/subject/application/{applicationId}\n  method: put\n  operationId: createSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /referencing/subject/{subjectId}/touchpoints\n  method: get\n  operationId: getSubjectTouchpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/subject/{subjectId}/outcome/conditions\n  method: patch\n  operationId: patchSubjectOutcomeConditions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/media/document/{documentId}\n  method: get\n  operationId: getAuthenticatedFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/subject/{subjectId}/emails\n  method: get\n  operationId: getSubjectEmails\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/token\n  method: post\n  operationId: getAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/application\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/application/{applicationId}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/application/{applicationId}\n  method: patch\n  operationId: patchApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/application/{applicationId}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/subject/{subjectId}/auth/token\n  method: get\n  operationId: getBotToken\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/subject/{subjectId}/auth/token\n  method: post\n  operationId: createBotToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/subject/{subjectId}\n  method: get\n  operationId: getSubject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/subject/{subjectId}\n  method: patch\n  operationId: patchSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/subject/{subjectId}\n  method: delete\n  operationId: deleteSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/subject/application/{applicationId}\n  method: put\n  operationId: createSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/subject/{subjectId}/touchpoints\n  method: get\n  operationId: getSubjectTouchpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/subject/{subjectId}/outcome/conditions\n  method: patch\n  operationId: patchSubjectOutcomeConditions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencing/media/document/{documentId}\n  method: get\n  operationId: getAuthenticatedFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referencing/subject/{subjectId}/emails\n  method: get\n  operationId: getSubjectEmails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/agentic-access/goodlord-agentic-access.yml
summary_line: 65 operations · 36 acting
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Management
- Rentals
- Lettings
- Tenant Referencing
- Tenancy Management
- Insurance
- Payments
---
