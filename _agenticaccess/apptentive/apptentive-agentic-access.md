---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 35
api_specs:
- filename: apptentive-openapi-original.yml
  format: yaml
  label: Apptentive Data API
  slug: apptentive-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apptentive/refs/heads/main/openapi/apptentive-openapi-original.yml
consequence_counts:
  read: 35
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apptentive Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'Apptentive exposes 36 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apptentive
provider_slug: apptentive
slug: apptentive-agentic-access
source_filename: apptentive-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/apptentive-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 35\n    acting: 1\n  by_consequence:\n    read: 35\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /info\n  method: get\n  operationId: showDataEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps\n  method: get\n  operationId: getAllApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/app-health/active-users\n\
  \  method: get\n  operationId: getActiveUsersData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/app-health/interactions/notes\n  method: get\n  operationId: getNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/app-health/interactions/surveys\n  method: get\n  operationId: getSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/app-health/love-percent\n  method: get\n  operationId: getLovePercentData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/app-health/ratings\n\
  \  method: get\n  operationId: getRatings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/app-health/retention\n  method: get\n  operationId: getRetention\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/fan-signals/counts\n  method: get\n  operationId: getFSCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/fan-signals/net-fan-score\n  method: get\n  operationId: getNFSData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/reviews\n  method: get\n  operationId:\
  \ fetchReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/stats/events\n  method: get\n  operationId: getEventStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/stats/event-trend\n  method: get\n  operationId: getEventTrendStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/stats/notes\n  method: get\n  operationId: getNotesStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/stats/surveys\n  method: get\n  operationId: getSurveyStats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/survey/{survey_id}/stats\n  method: get\n  operationId: getOneSurveyStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/survey/{survey_id}/question/{question_id}/responses\n  method: get\n  operationId: getSurveyResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/survey/insights\n  method: get\n  operationId: fetch responses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/v2/apps/{app_id}/gdpr-ccpa/requests\n  method: post\n  operationId: postGDPRRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/v2/apps/{app_id}/gdpr-ccpa/requests/{request_id}\n  method: get\n  operationId: getGDPRRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raw/v2/apps/{app_id}/messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raw/v2/apps/{app_id}/devices\n  method: get\n  operationId: getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /raw/v2/apps/{app_id}/devices/{device_id}\n  method: get\n  operationId: getSingleDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raw/v2/apps/{app_id}/people\n  method: get\n  operationId: getPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raw/v2/apps/{app_id}/people/{person_id}\n  method: get\n  operationId: getSinglePerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raw/v2/apps/{app_id}/conversations\n  method: get\n  operationId: getConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raw/v2/apps/{app_id}/conversations/{conversation_id}\n\
  \  method: get\n  operationId: getSingleConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raw/v2/apps/{app_id}/conversation-all-data/{conversation_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raw/v2/apps/{app_id}/surveys/{survey_id}/responses\n  method: get\n  operationId: getRawSurveyResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /raw/v2/apps/{app_id}/custom-attributes-keys\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experimental/v2/apps/{app_id}/surveys\n  method: get\n  operationId: getBasicSingleSurveyResponses\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experimental/v2/apps/{app_id}/surveys/{survey_id}\n  method: get\n  operationId: getBasicSingleSurveyResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experimental/v2/apps/{app_id}/notes\n  method: get\n  operationId: getBasicNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experimental/v2/apps/{app_id}/notes/{note_id}\n  method: get\n  operationId: getBasicSingleNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experimental/v2/apps/{app_id}/reach/sdk\n  method: get\n  operationId: getSDKDistribution\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experimental/v2/apps/{app_id}/app-health/rating-dialog\n  method: get\n  operationId: getRatingDialog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptentive/refs/heads/main/agentic-access/apptentive-agentic-access.yml
summary_line: 36 operations · 1 acting
tags:
- Company
- Enterprise
- Mobile
- Customer Feedback
- Surveys
- Analytics
- Customer Engagement
- Voice of Customer
---
