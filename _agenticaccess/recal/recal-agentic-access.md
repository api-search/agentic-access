---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 19
api_specs:
- filename: recal-organization-api-openapi.yml
  format: yaml
  label: Recal Organization API
  slug: recal-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-organization-api-openapi.yml
- filename: recal-organization-scheduling-api-openapi.yml
  format: yaml
  label: Recal Organization Scheduling API
  slug: recal-organization-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-organization-scheduling-api-openapi.yml
- filename: recal-organizations-calendar-api-openapi.yml
  format: yaml
  label: Recal Organizations Calendar API
  slug: recal-organizations-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-organizations-calendar-api-openapi.yml
- filename: recal-user-calendar-api-openapi.yml
  format: yaml
  label: Recal User Calendar API
  slug: recal-user-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-user-calendar-api-openapi.yml
- filename: recal-user-oauth-api-openapi.yml
  format: yaml
  label: Recal User OAuth API
  slug: recal-user-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-user-oauth-api-openapi.yml
- filename: recal-user-scheduling-api-openapi.yml
  format: yaml
  label: Recal User Scheduling API
  slug: recal-user-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-user-scheduling-api-openapi.yml
- filename: recal-users-api-openapi.yml
  format: yaml
  label: Recal Users API
  slug: recal-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recal/openapi/recal-users-api-openapi.yml
consequence_counts:
  read: 19
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Recal Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 38
overview: 'Recal exposes 38 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Recal
provider_slug: recal
slug: recal-agentic-access
source_filename: recal-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/recal-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 19\n    acting: 19\n  by_consequence:\n    read: 19\n    write: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/organizations\n  method: get\n  operationId: getV1Organizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations\n  method: post\n  operationId: postV1Organizations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgSlug}\n  method: get\n  operationId: getV1OrganizationsByOrgSlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgSlug}\n  method: put\n  operationId: putV1OrganizationsByOrgSlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgSlug}\n  method: delete\n  operationId: deleteV1OrganizationsByOrgSlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgSlug}/members\n  method: get\n  operationId: getV1OrganizationsByOrgSlugMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgSlug}/members\n  method: post\n  operationId: postV1OrganizationsByOrgSlugMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgSlug}/members\n  method: delete\n  operationId: deleteV1OrganizationsByOrgSlugMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgSlug}/calendar/busy\n  method: get\n  operationId: getV1OrganizationsByOrgSlugCalendarBusy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgSlug}/scheduling\n  method: get\n  operationId: getV1OrganizationsByOrgSlugScheduling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: get\n  operationId: getV1Users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: post\n  operationId: postV1Users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}\n  method: get\n  operationId: getV1UsersByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}\n  method: put\n  operationId: putV1UsersByUserId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}\n  method: delete\n  operationId: deleteV1UsersByUserId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/organizations\n  method: get\n  operationId: getV1UsersByUserIdOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/calendar\n  method: get\n  operationId: getV1UsersByUserIdCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/calendar/busy\n  method: get\n  operationId: getV1UsersByUserIdCalendarBusy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/calendar/events\n  method: get\n  operationId: getV1UsersByUserIdCalendarEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/calendar/events/meta\n  method: post\n  operationId: postV1UsersByUserIdCalendarEventsMeta\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/calendar/events/meta/{metaId}\n  method: get\n  operationId: getV1UsersByUserIdCalendarEventsMetaByMetaId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/calendar/events/meta/{metaId}\n  method: put\n  operationId: putV1UsersByUserIdCalendarEventsMetaByMetaId\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/calendar/events/meta/{metaId}\n  method: delete\n  operationId: deleteV1UsersByUserIdCalendarEventsMetaByMetaId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/calendar/events/{provider}/{calendarId}\n  method: post\n  operationId: postV1UsersByUserIdCalendarEventsByProviderByCalendarId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/calendar/events/{provider}/{calendarId}/{eventId}\n  method: get\n  operationId: getV1UsersByUserIdCalendarEventsByProviderByCalendarIdByEventId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/calendar/events/{provider}/{calendarId}/{eventId}\n  method: put\n  operationId: putV1UsersByUserIdCalendarEventsByProviderByCalendarIdByEventId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/calendar/events/{provider}/{calendarId}/{eventId}\n  method: delete\n  operationId: deleteV1UsersByUserIdCalendarEventsByProviderByCalendarIdByEventId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/oauth\n  method: get\n  operationId: getV1UsersByUserIdOauth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/oauth/links\n  method: get\n  operationId: getV1UsersByUserIdOauthLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/oauth/{provider}/link\n  method: get\n  operationId: getV1UsersByUserIdOauthByProviderLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/users/oauth/{provider}/verify\n  method: post\n  operationId: postV1UsersOauthByProviderVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/oauth/{provider}\n  method: get\n  operationId: getV1UsersByUserIdOauthByProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/oauth/{provider}\n  method: post\n  operationId: postV1UsersByUserIdOauthByProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/oauth/{provider}\n  method: delete\n  operationId: deleteV1UsersByUserIdOauthByProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userId}/oauth/{provider}/token\n  method: get\n  operationId: getV1UsersByUserIdOauthByProviderToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/scheduling\n  method: get\n  operationId: getV1UsersByUserIdScheduling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{userId}/scheduling\n\
  \  method: post\n  operationId: postV1UsersByUserIdScheduling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/scheduling\n  method: post\n  operationId: postV1UsersScheduling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/recal/agentic-access/recal-agentic-access.yml
summary_line: 38 operations · 19 acting
tags:
- Calendar API
- Scheduling
- SDK
- Multi-Tenant
- Recruiting
- Marketplace
- AI Agents
---
