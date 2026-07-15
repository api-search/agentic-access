---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 9
api_specs:
- filename: delighted-delighted-api-openapi.yml
  format: yaml
  label: Delighted API
  slug: delighted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/openapi/delighted-delighted-api-openapi.yml
consequence_counts:
  physical: 5
  read: 9
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Delighted Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /autopilot/email/memberships.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /autopilot/email/memberships.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /autopilot/sms/memberships.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /autopilot/sms/memberships.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /people.json
operation_count: 18
overview: 'Delighted exposes 18 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 4 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Delighted
provider_slug: delighted
slug: delighted-agentic-access
source_filename: delighted-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/delighted-delighted-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 9\n    connected: 9\n  by_consequence:\n    physical: 5\n    read: 9\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /people.json\n  method: post\n  operationId: sendToPersonOrCreatePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people.json\n  method:\
  \ get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{person_identifier}\n  method: delete\n  operationId: deletePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/{person_email}/survey_requests/pending.json\n  method: delete\n  operationId: deletePendingSurveyRequests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /survey_responses.json\n  method: get\n  operationId:\
  \ listSurveyResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /survey_responses.json\n  method: post\n  operationId: addSurveyResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics.json\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unsubscribes.json\n  method: post\n  operationId: unsubscribePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unsubscribes.json\n  method: get\n  operationId: listUnsubscribedPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bounces.json\n  method: get\n  operationId: listBouncedPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autopilot/email.json\n  method: get\n  operationId: getAutopilotEmailConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autopilot/sms.json\n  method: get\n  operationId: getAutopilotSmsConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /autopilot/email/memberships.json\n  method: get\n  operationId: listAutopilotEmailMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autopilot/email/memberships.json\n  method: post\n  operationId: addPersonToAutopilotEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autopilot/email/memberships.json\n  method: delete\n  operationId: removePersonFromAutopilotEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autopilot/sms/memberships.json\n  method: get\n  operationId: listAutopilotSmsMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autopilot/sms/memberships.json\n  method: post\n  operationId: addPersonToAutopilotSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autopilot/sms/memberships.json\n  method: delete\n  operationId: removePersonFromAutopilotSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delighted/refs/heads/main/agentic-access/delighted-agentic-access.yml
summary_line: 18 operations · 9 acting
tags:
- NPS
- Net Promoter Score
- CSAT
- Customer Satisfaction
- CES
- Customer Effort Score
- Survey
- Customer Experience
- Feedback
- eNPS
---
