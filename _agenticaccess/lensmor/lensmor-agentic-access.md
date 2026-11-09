---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 20
api_specs:
- filename: lensmor-actions-api-openapi.yml
  format: yaml
  label: Lensmor Actions API
  slug: lensmor-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-actions-api-openapi.yml
- filename: lensmor-contacts-api-openapi.yml
  format: yaml
  label: Lensmor Contacts API
  slug: lensmor-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-contacts-api-openapi.yml
- filename: lensmor-credits-api-openapi.yml
  format: yaml
  label: Lensmor Credits API
  slug: lensmor-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-credits-api-openapi.yml
- filename: lensmor-events-api-openapi.yml
  format: yaml
  label: Lensmor Events API
  slug: lensmor-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-events-api-openapi.yml
- filename: lensmor-exhibitors-api-openapi.yml
  format: yaml
  label: Lensmor Exhibitors API
  slug: lensmor-exhibitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-exhibitors-api-openapi.yml
- filename: lensmor-personnel-api-openapi.yml
  format: yaml
  label: Lensmor Personnel API
  slug: lensmor-personnel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-personnel-api-openapi.yml
- filename: lensmor-profile-matching-api-openapi.yml
  format: yaml
  label: Lensmor Profile Matching API
  slug: lensmor-profile-matching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lensmor/openapi/lensmor-profile-matching-api-openapi.yml
consequence_counts:
  read: 20
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lensmor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'Lensmor exposes 31 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lensmor
provider_slug: lensmor
slug: lensmor-agentic-access
source_filename: lensmor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/lensmor-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 20\n    acting: 11\n  by_consequence:\n    read: 20\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /external/credits/balance\n  method: get\n  operationId: getExternalCreditsBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/actions/precheck\n  method: post\n  operationId: precheckExternalAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/events/list\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/events/{id}\n  method: get\n  operationId: getEventDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/events/brief\n  method: get\n  operationId: getEventBrief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/events/fit-score\n  method: post\n  operationId: scoreEventFit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/events/rank\n  method: post\n  operationId: rankEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/events/{id}/unlock\n  method: post\n  operationId: unlockEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/events/{id}/visitors/unlock\n  method: post\n  operationId: unlockEventVisitors\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/events/{id}/full-access/unlock\n  method: post\n  operationId: unlockEventFullAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/exhibitors/list\n  method: get\n  operationId: listExhibitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/exhibitors/search\n  method: post\n  operationId: searchExhibitors\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/exhibitors/search-by-company-name\n  method: post\n  operationId: searchExhibitorsByCompanyName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/exhibitors/search-events\n  method: post\n  operationId: searchEventsByExhibitorCompanyName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/exhibitors/profile\n  method: get\n  operationId: getExhibitorProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/exhibitors/events\n  method: get\n  operationId: listExhibitorEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/personnel/list\n  method: get\n  operationId: listPersonnel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/personnel/profile\n  method: get\n  operationId: getPersonnelProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/personnel/events\n  method: get\n  operationId: listPersonnelEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/personnel/events/by-linkedin\n  method: get\n  operationId: listPersonnelEventsByLinkedin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /external/personnel/events/by-name\n  method: get\n  operationId: searchPersonnelEventsByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/personnel/unlock-linkedin-activity\n  method: post\n  operationId: unlockLinkedinActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/contacts/search\n  method: get\n  operationId: searchContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/contacts/unlock\n  method: post\n  operationId: unlockContactEmails\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/contacts/unlock-tasks/{taskId}\n  method: get\n  operationId: getContactUnlockTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/profile-matching/actions/apply-recommended-events/paged\n  method: post\n  operationId: applyRecommendedEventsPaged\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/profile-matching/recommendations/exhibitors\n  method: get\n  operationId: getRecommendedExhibitors\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/contacts/unlock-phone\n  method: post\n  operationId: unlockContactPhones\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/contacts/unlock-phone-tasks/{taskId}\n  method: get\n  operationId: getPhoneUnlockTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/personnel/generate-outreach-message\n  method: post\n  operationId: generateOutreachMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/personnel/outreach\n  method: get\n  operationId: getOutreachDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/lensmor/agentic-access/lensmor-agentic-access.yml
summary_line: 31 operations · 11 acting
tags:
- Event-Intelligence
- B2B
- Software-as-a-Service
- Lead Generation
- Trade Shows
---
