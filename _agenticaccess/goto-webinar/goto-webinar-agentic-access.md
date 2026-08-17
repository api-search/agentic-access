---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 31
api_specs:
- filename: goto-webinar-openapi.yml
  format: yaml
  label: GoTo Webinar REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/_original/goto-webinar-openapi.yml
- filename: goto-webinar-attendees-api-openapi.yml
  format: yaml
  label: GoTo Webinar Attendees API
  slug: goto-webinar-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-attendees-api-openapi.yml
- filename: goto-webinar-panelists-api-openapi.yml
  format: yaml
  label: GoTo Webinar Panelists API
  slug: goto-webinar-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-panelists-api-openapi.yml
- filename: goto-webinar-registrants-api-openapi.yml
  format: yaml
  label: GoTo Webinar Registrants API
  slug: goto-webinar-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-registrants-api-openapi.yml
- filename: goto-webinar-sessions-api-openapi.yml
  format: yaml
  label: GoTo Webinar Sessions API
  slug: goto-webinar-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-sessions-api-openapi.yml
- filename: goto-webinar-webinars-api-openapi.yml
  format: yaml
  label: GoTo Webinar Webinars API
  slug: goto-webinar-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-webinars-api-openapi.yml
- filename: goto-webinar-co-organizers-api-openapi.yml
  format: yaml
  label: GoTo Webinar Co Organizers API
  slug: goto-webinar-co-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-co-organizers-api-openapi.yml
- filename: goto-webinar-recordingassets-api-openapi.yml
  format: yaml
  label: GoTo Webinar Recording Assets API
  slug: goto-webinar-recordingassets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-recordingassets-api-openapi.yml
- filename: goto-webinar-webhooks-api-openapi.yml
  format: yaml
  label: GoTo Webinar Webhooks API
  slug: goto-webinar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 31
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Goto Webinar Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers/{coorganizerKey}/resendInvitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}/resendInvitation
operation_count: 53
overview: 'GoTo Webinar exposes 53 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 20 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoTo Webinar
provider_slug: goto-webinar
slug: goto-webinar-agentic-access
source_filename: goto-webinar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/goto-webinar-attendees-api-openapi.yml, openapi/goto-webinar-co-organizers-api-openapi.yml,\n  openapi/goto-webinar-panelists-api-openapi.yml, openapi/goto-webinar-recordingassets-api-openapi.yml,\n  openapi/goto-webinar-registrants-api-openapi.yml, openapi/goto-webinar-sessions-api-openapi.yml,\n  openapi/goto-webinar-webhooks-api-openapi.yml, openapi/goto-webinar-webinars-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 31\n    acting: 22\n  by_consequence:\n    read: 31\n    write: 20\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees\n\
  \  method: get\n  operationId: getAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}\n  method: get\n  operationId: getAttendee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/polls\n  method: get\n  operationId: getAttendeePollAnswers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/questions\n  method: get\n  operationId: getAttendeeQuestions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/surveys\n  method: get\n  operationId: getAttendeeSurveyAnswers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers\n  method: get\n  operationId: getCoorganizers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers\n  method: post\n  operationId: createCoorganizers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers/{coorganizerKey}\n  method: delete\n  operationId: deleteCoorganizer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers/{coorganizerKey}/resendInvitation\n  method: post\n  operationId: resendCoorganizerInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists\n\
  \  method: get\n  operationId: getPanelists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists\n  method: post\n  operationId: createPanelists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}/resendInvitation\n  method: post\n  operationId: resendPanelistInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}\n  method: delete\n  operationId: deleteWebinarPanelist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordingassets/search\n  method: post\n  operationId: searchAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountKey}/recordingassets/search\n  method: post\n  operationId: searchAssetsForAdmin\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants\n  method: post\n  operationId: createRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants\n  method: get\n  operationId: getAllRegistrantsForWebinar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}\n  method: delete\n\
  \  operationId: deleteRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}\n  method: get\n  operationId: getRegistrant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/fields\n  method: get\n  operationId: getRegistrationFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/sessions\n  method: get\n  operationId: getOrganizerSessions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions\n  method: get\n  operationId: getAllSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}\n  method: get\n  operationId: getWebinarSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/performance\n  method: get\n  operationId: getPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/polls\n\
  \  method: get\n  operationId: getPolls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/questions\n  method: get\n  operationId: getQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/surveys\n  method: get\n  operationId: getSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/secretkey\n  method: post\n  operationId: createSecretKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: createWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: put\n  operationId: updateWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n\
  \  method: delete\n  operationId: deleteWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookKey}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userSubscriptions\n  method: post\n  operationId: createUserSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions\n  method: put\n  operationId: updateUserSubscriptions\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions\n  method: get\n  operationId: getUserSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userSubscriptions\n  method: delete\n  operationId: deleteUserSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions/{userSubscriptionsKey}\n  method: get\n  operationId: getUserSubscription\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountKey}/webinars\n  method: get\n  operationId: getAllAccountWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars\n  method: get\n  operationId: getWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars\n  method: post\n  operationId: createWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/insessionWebinars\n  method:\
  \ get\n  operationId: getInSessionWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: get\n  operationId: getWebinar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: put\n  operationId: updateWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: delete\n  operationId: cancelWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/attendees\n  method: get\n  operationId: getAttendeesForAllWebinarSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/meetingtimes\n  method: get\n  operationId: getWebinarMeetingTimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/audio\n  method: get\n  operationId: getAudioInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/audio\n  method: post\n  operationId: updateAudioInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/performance\n  method: get\n  operationId: getPerformanceForAllWebinarSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinars/{webinarKey}/startUrl\n  method: get\n  operationId: getStartUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinars/{webinarKey}/copy\n  method: put\n  operationId: copyWebinar\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinars/{webinarKey}/recordingAssets\n  method: get\n  operationId: getRecordingAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/agentic-access/goto-webinar-agentic-access.yml
summary_line: 53 operations · 22 acting
tags:
- Webinars
- Virtual Events
- Video Conferencing
- Marketing
- Lead Capture
- Registration
- Webhooks
- Event Management
- Collaboration
- Analytics
---
