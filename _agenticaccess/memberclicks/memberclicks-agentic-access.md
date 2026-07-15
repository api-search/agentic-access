---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 13
api_specs:
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Profiles API
  slug: memberclicks-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Profile Search API
  slug: memberclicks-profile-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Attributes API
  slug: memberclicks-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Member Types and Statuses API
  slug: memberclicks-member-types-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Groups API
  slug: memberclicks-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Events API
  slug: memberclicks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Continuing Education API
  slug: memberclicks-continuing-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
consequence_counts:
  read: 13
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Memberclicks Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'MemberClicks exposes 17 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MemberClicks
provider_slug: memberclicks
slug: memberclicks-agentic-access
source_filename: memberclicks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/memberclicks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 4\n    connected: 13\n  by_consequence:\n    write: 4\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/v1/token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/profile\n  method: get\n  operationId: listProfiles\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/profile\n  method: post\n  operationId: createProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/profile/{profileId}\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/profile/{profileId}\n  method: put\n  operationId: updateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/profile/search\n  method: post\n  operationId: createProfileSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/attribute\n  method: get\n  operationId: listAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/attribute/{attributeId}/selection\n  method: get\n  operationId: listAttributeSelectionOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/member-type\n  method: get\n  operationId: listMemberTypes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/member-status\n  method: get\n  operationId: listMemberStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/continuing-education/credit\n  method: get\n  operationId: listContinuingEducationCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/continuing-education/credit/{creditId}\n  method: get\n  operationId: getContinuingEducationCredit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/country\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/group\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/group/{groupId}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/event\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/event/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/agentic-access/memberclicks-agentic-access.yml
summary_line: 17 operations · 4 acting
tags:
- Membership Management
- Association Management
- AMS
- Nonprofit
- Events
- CRM
- Personify
---
