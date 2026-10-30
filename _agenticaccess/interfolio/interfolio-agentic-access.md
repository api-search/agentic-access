---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 36
api_specs:
- filename: interfolio-activities-api-openapi.yml
  format: yaml
  label: Interfolio Activities API
  slug: interfolio-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-activities-api-openapi.yml
- filename: interfolio-activity-classifications-api-openapi.yml
  format: yaml
  label: Interfolio Activity Classifications API
  slug: interfolio-activity-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-activity-classifications-api-openapi.yml
- filename: interfolio-activity-input-api-openapi.yml
  format: yaml
  label: Interfolio Activity Input API
  slug: interfolio-activity-input-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-activity-input-api-openapi.yml
- filename: interfolio-courses-api-openapi.yml
  format: yaml
  label: Interfolio Courses API
  slug: interfolio-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-courses-api-openapi.yml
- filename: interfolio-download-attachments-api-openapi.yml
  format: yaml
  label: Interfolio Download Attachments API
  slug: interfolio-download-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-download-attachments-api-openapi.yml
- filename: interfolio-emails-api-openapi.yml
  format: yaml
  label: Interfolio Emails API
  slug: interfolio-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-emails-api-openapi.yml
- filename: interfolio-evaluations-api-openapi.yml
  format: yaml
  label: Interfolio Evaluations API
  slug: interfolio-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-evaluations-api-openapi.yml
- filename: interfolio-faculty-classifications-api-openapi.yml
  format: yaml
  label: Interfolio Faculty Classifications API
  slug: interfolio-faculty-classifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-faculty-classifications-api-openapi.yml
- filename: interfolio-faq-api-openapi.yml
  format: yaml
  label: Interfolio FAQ API
  slug: interfolio-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-faq-api-openapi.yml
- filename: interfolio-permissions-api-openapi.yml
  format: yaml
  label: Interfolio Permissions API
  slug: interfolio-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-permissions-api-openapi.yml
- filename: interfolio-sections-api-openapi.yml
  format: yaml
  label: Interfolio Sections API
  slug: interfolio-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-sections-api-openapi.yml
- filename: interfolio-sso-api-openapi.yml
  format: yaml
  label: Interfolio SSO API
  slug: interfolio-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-sso-api-openapi.yml
- filename: interfolio-terms-api-openapi.yml
  format: yaml
  label: Interfolio Terms API
  slug: interfolio-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-terms-api-openapi.yml
- filename: interfolio-units-api-openapi.yml
  format: yaml
  label: Interfolio Units API
  slug: interfolio-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-units-api-openapi.yml
- filename: interfolio-user-data-api-openapi.yml
  format: yaml
  label: Interfolio User Data API
  slug: interfolio-user-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-user-data-api-openapi.yml
- filename: interfolio-users-api-openapi.yml
  format: yaml
  label: Interfolio Users API
  slug: interfolio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-users-api-openapi.yml
- filename: interfolio-vitas-api-openapi.yml
  format: yaml
  label: Interfolio Vitas API
  slug: interfolio-vitas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/openapi/interfolio-vitas-api-openapi.yml
consequence_counts:
  physical: 1
  read: 36
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Interfolio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant_id}/vitas_export/send_email
operation_count: 56
overview: 'Interfolio exposes 56 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read, 19 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Interfolio
provider_slug: interfolio
slug: interfolio-agentic-access
source_filename: interfolio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/interfolio-faculty180-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    connected: 36\n    acting: 20\n  by_consequence:\n    read: 36\n    write: 19\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api.php/activityclassifications\n  method: get\n  operationId: activityclassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/activityclassifications/{activityclassificationid}\n  method: get\n  operationId: activityclassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/activities\n  method: get\n  operationId: activities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/activities/{sectionid}\n  method: get\n  operationId: activitiesdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/activities_details/{sectionid}\n  method: get\n  operationId: activitiesdetailsandsection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/activities/{sectionid}/{activityid}\n  method: get\n  operationId: activitiessectionidactivityid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api.php/activities/{sectionid}/{activityid}/attachments\n  method: get\n  operationId: activityattachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity_input/{approval_id}/{faculty_id}/status\n  method: get\n  operationId: getFacultyApprovalStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity_input/form_name_units/{formName}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/courseprefixes\n  method: get\n  operationId: coursePrefix\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api.php/courseprefixes\n  method: post\n  operationId: courseprefixesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/courses\n  method: get\n  operationId: coursesG\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/courses\n  method: post\n  operationId: coursesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/coursestaught\n  method: get\n  operationId: coursesTaught\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/coursestaught\n  method: post\n  operationId: coursestaughtPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/coursestaught\n  method: delete\n  operationId: deletecoursestaught\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/coursestaught/{coursestaughtid}\n  method: get\n  operationId: coursestaughtid\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/coursestaught/{coursestaughtid}\n  method: put\n  operationId: coursestaughtidPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/coursestaught/{coursestaughtid}\n  method: delete\n  operationId: deletecoursestaught\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/coursestaught/{coursestaughtid}/attachments\n  method: get\n  operationId: coursestaughtidattachments\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/coursestaught/{coursestaughtid}/attachments\n  method: post\n  operationId: coursesidattachmentsPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/downloadattachments/{attachmentid}\n  method: get\n  operationId: attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant_id}/vitas_export/send_email\n  method: post\n  operationId: viatBuilderExportEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/evaluations\n  method: get\n  operationId: facultyEvaluations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /evaluations/search\n  method: get\n  operationId: faq\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/facultyclassificationdata\n  method: get\n  operationId: facultyClassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/facultyclassifications\n  method: get\n  operationId: facultyClassifications\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/facultyclassifications/{facultyclassificationid}\n  method: get\n  operationId: facultyClassificationsID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faq\n  method: get\n  operationId: faq\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faq/answer/{id}\n  method: post\n  operationId: answerFaqById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /faq/{id}\n  method: delete\n  operationId: deleteFaq\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/sections\n  method: get\n  operationId: sections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/sections/{sectionid}\n  method: get\n  operationId: sections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenantId}/users/{pid}/users_sso\n  method: delete\n  operationId: deleteSsoId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /api.php/terms\n  method: get\n  operationId: terms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/units\n  method: get\n  operationId: units\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/units\n  method: post\n  operationId: unitCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/units/{unitid}\n  method: get\n  operationId: unitDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api.php/users\n  method: get\n  operationId: users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/users\n  method: post\n  operationId: userCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/users/{userid}\n  method: get\n  operationId: userDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/users/{userid}\n  method: put\n  operationId: userUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fars/{tenant_id}/users/{pid}/subscribe\n  method: post\n  operationId: subscribeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fars/{tenant_id}/users/{pid}\n  method: put\n  operationId: updateUserSubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fars/{tenant_id}/users/{pid}/unsubscribe\n  method: put\n  operationId: userUnsubscribe\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fars/{tenant_id}/users/csv_create\n  method: post\n  operationId: createUsersCSV\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fars/{tenant_id}/users/csv_update\n  method: post\n  operationId: updateUsersCSV\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/userdata\n\
  \  method: get\n  operationId: userdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/users/permissions\n  method: get\n  operationId: facultyPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/users/permissions\n  method: post\n  operationId: createUsersPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api.php/users/{userid}/permissions\n  method: get\n  operationId: facultyPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /users/activity_input_request\n  method: get\n  operationId: ActivityInputRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/current\n  method: get\n  operationId: CurrentUserPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/vitas\n  method: get\n  operationId: vitas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php/vitas/{vitaid}/{userid}\n  method: get\n  operationId: userVita\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant_id}/vita_templates\n  method: get\n  operationId: userVita\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/agentic-access/interfolio-agentic-access.yml
summary_line: 56 operations · 20 acting
tags:
- Company
- Education
- Higher Education
- Faculty Information System
- Faculty Activity Reporting
- Review Promotion Tenure
- Academic
- Research
---
