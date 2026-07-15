---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 14
api_specs:
- filename: goto-webinar-openapi.yml
  format: yaml
  label: GoTo Webinar REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-openapi.yml
consequence_counts:
  read: 14
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Goto Webinar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'GoTo Webinar exposes 20 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GoTo Webinar
provider_slug: goto-webinar
slug: goto-webinar-agentic-access
source_filename: goto-webinar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/goto-webinar-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 14\n    acting: 6\n  by_consequence:\n    read: 14\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /organizers/{organizerKey}/webinars\n  method: get\n  operationId: listOrganizerWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars\n  method: post\n  operationId: createWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/upcomingWebinars\n  method: get\n  operationId: listUpcomingWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/historicalWebinars\n  method: get\n  operationId: listHistoricalWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: get\n  operationId: getWebinar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: put\n  operationId: updateWebinar\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}\n  method: delete\n  operationId: cancelWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions\n  method: get\n  operationId: listWebinarSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}\n\
  \  method: get\n  operationId: getWebinarSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/performance\n  method: get\n  operationId: getSessionPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees\n  method: get\n  operationId: listSessionAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/polls\n  method: get\n  operationId: listSessionPolls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/questions\n  method: get\n  operationId: listSessionQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants\n  method: get\n  operationId: listRegistrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants\n  method: post\n  operationId: createRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}\n  method: get\n  operationId: getRegistrant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}\n  method: delete\n  operationId: deleteRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/attendees\n  method: get\n  operationId: listWebinarAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists\n\
  \  method: get\n  operationId: listPanelists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizers/{organizerKey}/webinars/{webinarKey}/panelists\n  method: post\n  operationId: createPanelists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/agentic-access/goto-webinar-agentic-access.yml
summary_line: 20 operations · 6 acting
tags:
- Webinars
- Virtual Events
- Video Conferencing
- Marketing
- Lead Capture
- Registration
---
