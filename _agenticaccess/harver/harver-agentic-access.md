---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 29
api_specs:
- filename: harver-accounts-api-openapi.yml
  format: yaml
  label: Harver Accounts API
  slug: harver-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-accounts-api-openapi.yml
- filename: harver-applications-api-openapi.yml
  format: yaml
  label: Harver Applications API
  slug: harver-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-applications-api-openapi.yml
- filename: harver-candidate-statuses-api-openapi.yml
  format: yaml
  label: Harver Candidate Statuses API
  slug: harver-candidate-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-candidate-statuses-api-openapi.yml
- filename: harver-candidateapplications-api-openapi.yml
  format: yaml
  label: Harver Candidate Applications API
  slug: harver-candidateapplications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-candidateapplications-api-openapi.yml
- filename: harver-scheduling-api-openapi.yml
  format: yaml
  label: Harver Scheduling API
  slug: harver-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-scheduling-api-openapi.yml
- filename: harver-user-profile-api-openapi.yml
  format: yaml
  label: Harver User Profile API
  slug: harver-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-user-profile-api-openapi.yml
- filename: harver-vacancies-api-openapi.yml
  format: yaml
  label: Harver Vacancies API
  slug: harver-vacancies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-vacancies-api-openapi.yml
- filename: harver-webhook-api-openapi.yml
  format: yaml
  label: Harver Webhook API
  slug: harver-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-webhook-api-openapi.yml
- filename: harver-oauth-api-openapi.yml
  format: yaml
  label: Harver OAUTH API
  slug: harver-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/openapi/harver-oauth-api-openapi.yml
consequence_counts:
  read: 29
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Harver Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 54
overview: 'Harver exposes 54 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read and 25 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Harver
provider_slug: harver
slug: harver-agentic-access
source_filename: harver-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/harver-accounts-api-openapi.yml, openapi/harver-applications-api-openapi.yml,\n  openapi/harver-candidate-statuses-api-openapi.yml, openapi/harver-candidateapplications-api-openapi.yml,\n  openapi/harver-oauth-api-openapi.yml, openapi/harver-scheduling-api-openapi.yml, openapi/harver-user-profile-api-openapi.yml,\n  openapi/harver-vacancies-api-openapi.yml, openapi/harver-webhook-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    connected: 29\n    acting: 25\n  by_consequence:\n    read: 29\n    write: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/candidates\n  method: get\n  operationId: getAccountsByAccountIdCandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/candidates/{candidateId}/applications\n  method: get\n  operationId: getAccountsByAccountIdCandidatesByCandidateIdApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/vacancies\n  method: get\n  operationId: getAccountsByAccountIdVacancies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/channels/{channelId}/vacancies\n  method: get\n  operationId:\
  \ getAccountsByAccountIdChannelsByChannelIdVacancies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/location-specific-questions\n  method: get\n  operationId: getAccountsByAccountIdLocationSpecificQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/locations\n  method: get\n  operationId: getAccountsByAccountIdLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/locations\n  method: post\n  operationId: postAccountsByAccountIdLocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/locations/{locationId}\n  method: get\n  operationId: getAccountsByAccountIdLocationsByLocationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/locations/{locationId}\n  method: patch\n  operationId: patchAccountsByAccountIdLocationsByLocationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/locations/ext-{externalLocationId}\n  method: get\n  operationId: getAccountsByAccountIdLocationsExt{externalLocationId}\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/locations/ext-{externalLocationId}\n  method: patch\n  operationId: patchAccountsByAccountIdLocationsExt{externalLocationId}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/regions\n  method: get\n  operationId: getAccountsByAccountIdRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/regions\n  method: post\n  operationId: postAccountsByAccountIdRegions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/regions/{regionId}\n  method: patch\n  operationId: patchAccountsByAccountIdRegionsByRegionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/users/{userProfileId}\n  method: get\n  operationId: getAccountsByAccountIdUsersByUserProfileId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/job-functions\n  method: get\n  operationId: getAccountsByAccountIdJobFunctions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/job-functions\n  method: post\n  operationId: postAccountsByAccountIdJobFunctions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/email-templates\n  method: get\n  operationId: getAccountsByAccountIdEmailTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/jobboard\n  method: get\n  operationId: getAccountsByAccountIdJobboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/rejectionReasons\n\
  \  method: get\n  operationId: getAccountsByAccountIdRejectionReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: get\n  operationId: getApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}\n  method: get\n  operationId: getApplicationsByApplicationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}\n  method: patch\n  operationId: patchApplicationsByApplicationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}\n  method: delete\n  operationId: deleteApplicationsByApplicationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/notes\n  method: get\n  operationId: getApplicationsByApplicationIdNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}/notes\n  method: post\n  operationId: postApplicationsByApplicationIdNotes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/notes/{noteId}\n  method: delete\n  operationId: deleteApplicationsByApplicationIdNotesByNoteId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/ats-parameters\n  method: patch\n  operationId: patchApplicationsByApplicationIdAtsParameters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/locations\n  method: patch\n  operationId: patchApplicationsByApplicationIdLocations\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/locations/ext-{externalLocationId}\n  method: patch\n  operationId: patchApplicationsByApplicationIdLocationsExt{externalLocationId}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/locations/{locationId}\n  method: patch\n  operationId: patchApplicationsByApplicationIdLocationsByLocationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/reapply/status\n  method: get\n  operationId: getApplicationsByApplicationIdReapplyStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}/reports/development-reports\n  method: get\n  operationId: getApplicationsByApplicationIdReportsDevelopmentReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}/reports/interview-guides\n  method: get\n  operationId: getApplicationsByApplicationIdReportsInterviewGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /applications/{applicationId}/reports/reports-hub\n  method: get\n  operationId: getApplicationsByApplicationIdReportsReportsHub\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidate-statuses\n  method: get\n  operationId: getCandidateStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vacancies/{vacancyId}/applications\n  method: post\n  operationId: postVacanciesByVacancyIdApplications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: postOauthToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/authenticate\n  method: post\n  operationId: postOauthAuthenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/userinfo\n  method: post\n  operationId: postOauthUserinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduling/{accountId}\n  method: post\n  operationId: postSchedulingByAccountId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduling/{accountId}/interview-details/{candidateId}\n  method: get\n  operationId: getSchedulingByAccountIdInterviewDetailsByCandidateId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/notifications/devices\n  method: post\n  operationId: postMeNotificationsDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/notifications\n  method: patch\n  operationId: patchMeNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vacancies/{vacancyId}/candidates\n  method: get\n  operationId: getVacanciesByVacancyIdCandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vacancies/{vacancyId}/modules/{moduleId}\n  method: get\n  operationId: getVacanciesByVacancyIdModulesByModuleId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vacancies/{vacancyId}\n  method: get\n\
  \  operationId: getVacanciesByVacancyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vacancies/{vacancyId}\n  method: patch\n  operationId: patchVacanciesByVacancyId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vacancies/{vacancyId}/locations\n  method: patch\n  operationId: patchVacanciesByVacancyIdLocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vacancies/{vacancyId}/locations-v2\n  method: patch\n\
  \  operationId: patchVacanciesByVacancyIdLocationsV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vacancies/{vacancyId}/regions\n  method: patch\n  operationId: patchVacanciesByVacancyIdRegions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhookPath\n  method: post\n  operationId: postWebhookPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harver/refs/heads/main/agentic-access/harver-agentic-access.yml
summary_line: 54 operations · 25 acting
tags:
- Company
- Human Resources
- Recruiting
- Hiring
- Talent Intelligence
- Pre-Employment Assessment
- Candidate Experience
- Applicant Tracking
---
