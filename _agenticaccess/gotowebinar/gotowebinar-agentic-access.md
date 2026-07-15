---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 17
api_specs:
- filename: gotowebinar-rest-openapi.yml
  format: yaml
  label: GoToWebinar REST API
  slug: gotowebinar-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-rest-openapi.yml
- filename: gotowebinar-webhooks-openapi.yml
  format: yaml
  label: GoToWebinar Webhooks API
  slug: gotowebinar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-webhooks-openapi.yml
consequence_counts:
  read: 17
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gotowebinar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'GoToWebinar exposes 30 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoToWebinar
provider_slug: gotowebinar
slug: gotowebinar-agentic-access
source_filename: gotowebinar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gotowebinar-rest-openapi.yml, openapi/gotowebinar-webhooks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 17\n    acting: 13\n  by_consequence:\n    read: 17\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /organizers/{organizerKey}/webinars\n  method: get\n  operationId: getWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars\n  method: post\n  operationId: createWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: get\n  operationId: getWebinar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: put\n  operationId: updateWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: delete\n  operationId: cancelWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants\n  method: get\n  operationId: listRegistrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants\n  method: post\n  operationId: createRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}\n  method: get\n  operationId: getRegistrant\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}\n  method: delete\n  operationId: deleteRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/attendees\n  method: get\n  operationId: listAllAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees\n  method: get\n  operationId: listSessionAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}\n  method: get\n  operationId: getSessionAttendee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/polls\n  method: get\n  operationId: getSessionPolls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/questions\n\
  \  method: get\n  operationId: getSessionQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/surveys\n  method: get\n  operationId: getSessionSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers\n  method: get\n  operationId: listCoorganizers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers\n  method: post\n  operationId: createCoorganizers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists\n  method: get\n  operationId: listPanelists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists\n  method: post\n  operationId: createPanelists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/recordingassets\n  method: get\n  operationId: listRecordingAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: put\n  operationId: updateWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookKey}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/secretkey\n  method: post\n\
  \  operationId: createWebhookSecretKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions\n  method: get\n  operationId: listUserSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userSubscriptions\n  method: post\n  operationId: createUserSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions/{subscriptionKey}\n  method: get\n  operationId: getUserSubscription\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userSubscriptions/{subscriptionKey}\n  method: put\n  operationId: updateUserSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions/{subscriptionKey}\n  method: delete\n  operationId: deleteUserSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/agentic-access/gotowebinar-agentic-access.yml
summary_line: 30 operations · 13 acting
tags:
- Attendees
- Collaboration
- Communications
- Events
- Meetings
- Registrants
- Sessions
- Surveys
- Video Conferencing
- Virtual Events
- Webhooks
- Webinars
---
