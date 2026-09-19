---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 38
api_specs:
- filename: gotowebinar-attendees-api-openapi.yml
  format: yaml
  label: GoToWebinar Attendees API
  slug: gotowebinar-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-attendees-api-openapi.yml
- filename: gotowebinar-co-organizers-api-openapi.yml
  format: yaml
  label: GoToWebinar Co-Organizers API
  slug: gotowebinar-co-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-co-organizers-api-openapi.yml
- filename: gotowebinar-panelists-api-openapi.yml
  format: yaml
  label: GoToWebinar Panelists API
  slug: gotowebinar-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-panelists-api-openapi.yml
- filename: gotowebinar-polls-api-openapi.yml
  format: yaml
  label: GoToWebinar Polls API
  slug: gotowebinar-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-polls-api-openapi.yml
- filename: gotowebinar-questions-api-openapi.yml
  format: yaml
  label: GoToWebinar Questions API
  slug: gotowebinar-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-questions-api-openapi.yml
- filename: gotowebinar-recordings-api-openapi.yml
  format: yaml
  label: GoToWebinar Recordings API
  slug: gotowebinar-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-recordings-api-openapi.yml
- filename: gotowebinar-registrants-api-openapi.yml
  format: yaml
  label: GoToWebinar Registrants API
  slug: gotowebinar-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-registrants-api-openapi.yml
- filename: gotowebinar-sessions-api-openapi.yml
  format: yaml
  label: GoToWebinar Sessions API
  slug: gotowebinar-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-sessions-api-openapi.yml
- filename: gotowebinar-surveys-api-openapi.yml
  format: yaml
  label: GoToWebinar Surveys API
  slug: gotowebinar-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-surveys-api-openapi.yml
- filename: gotowebinar-user-subscriptions-api-openapi.yml
  format: yaml
  label: GoToWebinar User Subscriptions API
  slug: gotowebinar-user-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-user-subscriptions-api-openapi.yml
- filename: gotowebinar-webhooks-api-openapi.yml
  format: yaml
  label: GoToWebinar Webhooks API
  slug: gotowebinar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-webhooks-api-openapi.yml
- filename: gotowebinar-webinars-api-openapi.yml
  format: yaml
  label: GoToWebinar Webinars API
  slug: gotowebinar-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-webinars-api-openapi.yml
- filename: gotowebinar-recording-assets-api-openapi.yml
  format: yaml
  label: GoToWebinar Recording Assets API
  slug: gotowebinar-recording-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-recording-assets-api-openapi.yml
consequence_counts:
  physical: 2
  read: 38
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gotowebinar Agentic Access
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
operation_count: 63
overview: 'GoToWebinar exposes 63 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 23 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoToWebinar
provider_slug: gotowebinar
slug: gotowebinar-agentic-access
source_filename: gotowebinar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/gotowebinar-attendees-api-openapi.yml, openapi/gotowebinar-co-organizers-api-openapi.yml,\n  openapi/gotowebinar-panelists-api-openapi.yml, openapi/gotowebinar-polls-api-openapi.yml,\n  openapi/gotowebinar-questions-api-openapi.yml, openapi/gotowebinar-recording-assets-api-openapi.yml,\n  openapi/gotowebinar-recordings-api-openapi.yml, openapi/gotowebinar-registrants-api-openapi.yml,\n  openapi/gotowebinar-sessions-api-openapi.yml, openapi/gotowebinar-surveys-api-openapi.yml,\n  openapi/gotowebinar-user-subscriptions-api-openapi.yml, openapi/gotowebinar-webhooks-api-openapi.yml,\n  openapi/gotowebinar-webinars-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 63\n  by_action_class:\n\
  \    connected: 38\n    acting: 25\n  by_consequence:\n    read: 38\n    write: 23\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees\n  method: get\n  operationId: getAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}\n  method: get\n  operationId: getAttendee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/polls\n  method: get\n  operationId: getAttendeePollAnswers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/questions\n  method: get\n  operationId: getAttendeeQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/surveys\n  method: get\n  operationId: getAttendeeSurveyAnswers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/attendees\n  method: get\n  operationId: listAllAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers\n\
  \  method: get\n  operationId: getCoorganizers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers\n  method: post\n  operationId: createCoorganizers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers/{coorganizerKey}\n  method: delete\n  operationId: deleteCoorganizer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/coorganizers/{coorganizerKey}/resendInvitation\n  method: post\n  operationId: resendCoorganizerInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists\n  method: get\n  operationId: getPanelists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists\n  method: post\n  operationId: createPanelists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}/resendInvitation\n  method: post\n  operationId: resendPanelistInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}\n  method: delete\n  operationId: deleteWebinarPanelist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/polls\n  method: get\n  operationId: getSessionPolls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/questions\n  method: get\n  operationId: getSessionQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recordingassets/search\n  method: post\n  operationId: searchAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountKey}/recordingassets/search\n\
  \  method: post\n  operationId: searchAssetsForAdmin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/recordingassets\n  method: get\n  operationId: listRecordingAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants\n  method: post\n  operationId: createRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants\n\
  \  method: get\n  operationId: getAllRegistrantsForWebinar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}\n  method: delete\n  operationId: deleteRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}\n  method: get\n  operationId: getRegistrant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/fields\n  method: get\n  operationId:\
  \ getRegistrationFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/sessions\n  method: get\n  operationId: getOrganizerSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions\n  method: get\n  operationId: getAllSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}\n  method: get\n  operationId: getWebinarSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/performance\n\
  \  method: get\n  operationId: getPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/polls\n  method: get\n  operationId: getPolls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/questions\n  method: get\n  operationId: getQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/surveys\n  method: get\n  operationId: getSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/surveys\n  method: get\n  operationId: getSessionSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userSubscriptions\n  method: get\n  operationId: listUserSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userSubscriptions\n  method: post\n  operationId: createUserSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions/{subscriptionKey}\n  method: get\n  operationId: getUserSubscription\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userSubscriptions/{subscriptionKey}\n  method: put\n  operationId: updateUserSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions/{subscriptionKey}\n  method: delete\n  operationId: deleteUserSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/secretkey\n  method: post\n  operationId: createSecretKey\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: createWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: put\n  operationId: updateWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: delete\n  operationId: deleteWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookKey}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userSubscriptions\n  method: post\n  operationId: createUserSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions\n  method: put\n  operationId: updateUserSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userSubscriptions\n  method: get\n  operationId: getUserSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userSubscriptions\n  method: delete\n  operationId: deleteUserSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /userSubscriptions/{userSubscriptionsKey}\n  method: get\n  operationId: getUserSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountKey}/webinars\n  method: get\n  operationId: getAllAccountWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars\n  method: get\n  operationId: getWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars\n  method: post\n  operationId: createWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/insessionWebinars\n  method: get\n  operationId: getInSessionWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: get\n  operationId: getWebinar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: put\n  operationId: updateWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n\
  \  method: delete\n  operationId: cancelWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/attendees\n  method: get\n  operationId: getAttendeesForAllWebinarSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/meetingtimes\n  method: get\n  operationId: getWebinarMeetingTimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/audio\n  method: get\n  operationId: getAudioInformation\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/audio\n  method: post\n  operationId: updateAudioInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/performance\n  method: get\n  operationId: getPerformanceForAllWebinarSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinars/{webinarKey}/startUrl\n  method: get\n  operationId: getStartUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /webinars/{webinarKey}/copy\n  method: put\n  operationId: copyWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinars/{webinarKey}/recordingAssets\n  method: get\n  operationId: getRecordingAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/agentic-access/gotowebinar-agentic-access.yml
summary_line: 63 operations · 25 acting
tags:
- Attendees
- Collaboration
- Communications
- Event
- Meetings
- Registrants
- Sessions
- Surveys
- Video Conferencing
- Virtual Events
- Webhook
- Webinars
---
