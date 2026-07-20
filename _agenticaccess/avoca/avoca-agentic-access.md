---
acting_count: 0
action_class_counts:
  connected: 31
api_specs:
- filename: avoca-openapi-original.json
  format: json
  label: Avoca Enterprise API
  slug: avoca-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/openapi/avoca-openapi-original.json
consequence_counts:
  read: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Avoca Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'Avoca exposes 31 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Avoca
provider_slug: avoca
slug: avoca-agentic-access
source_filename: avoca-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/avoca-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 31\n  by_consequence:\n    read: 31\n  human_in_the_loop_required: 0\noperations:\n- path: /api/calls\n  method: get\n  operationId: listCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calls/{id}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calls/{id}/transcript\n  method: get\n  operationId: getCallTranscript\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calls/latest-by-phone\n  method: get\n  operationId: getLatestCallByPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calls/pre-call-transfers\n  method: get\n  operationId: listPreCallTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/leads\n  method: get\n  operationId: listLeadsV0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/teams\n  method: get\n  operationId: listTeamsV0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/coach\n  method: get\n  operationId: listCoachCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/coach/{id}\n  method: get\n  operationId: getCoachCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/coach/rubrics\n  method: get\n  operationId: listCoachRubrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/scheduler-analytics\n  method: get\n  operationId: getSchedulerAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/scheduler-analytics/summary\n  method: get\n  operationId: getSchedulerAnalyticsSummary\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/simple_scheduler_booking_requests\n  method: get\n  operationId: listSimpleSchedulerBookingRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/simple_scheduler_config\n  method: get\n  operationId: listSimpleSchedulerConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/schedulers\n  method: get\n  operationId: listSchedulers\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/sessions\n  method: get\n  operationId: listTeamSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/sessions/{sessionId}\n  method: get\n  operationId: getTeamSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/bookings\n  method: get\n  operationId: listTeamBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/bookings/{bookingId}\n  method: get\n  operationId: getTeamBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/analytics/funnel\n  method: get\n  operationId: getTeamFunnel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/analytics/utm\n  method: get\n  operationId: getTeamUtm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/analytics/service-areas\n  method: get\n  operationId: getTeamServiceAreas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/analytics/issue-types\n  method: get\n  operationId: getTeamIssueTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/leads\n  method: get\n  operationId: listTeamLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/outbound/campaign-texts\n  method: get\n  operationId: listCampaignTexts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/teams/{teamId}/outbound/events\n  method: get\n  operationId: listOutboundEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/enterprise/{enterpriseId}/leads\n  method: get\n  operationId: listEnterpriseLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bookings\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analytics/funnel\n  method: get\n  operationId: getFunnel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avoca/refs/heads/main/agentic-access/avoca-agentic-access.yml
summary_line: 31 operations
tags:
- Company
- AI
- Voice AI
- Conversational AI
- Customer Service
- Contact Center
- Home Services
- Field Service
- Scheduling
- Analytics
- Webhooks
- Enterprise API
---
