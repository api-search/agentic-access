---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 19
api_specs:
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Bonuses API
  slug: bonusly-bonuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Users API
  slug: bonusly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Rewards API
  slug: bonusly-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Redemptions API
  slug: bonusly-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Analytics API
  slug: bonusly-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
- filename: bonusly-openapi.yml
  format: yaml
  label: Bonusly Company API
  slug: bonusly-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/openapi/bonusly-openapi.yml
consequence_counts:
  physical: 1
  read: 19
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bonusly Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /custom_reward_redemptions/fulfill
operation_count: 31
overview: 'Bonusly exposes 31 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 11 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bonusly
provider_slug: bonusly
slug: bonusly-agentic-access
source_filename: bonusly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bonusly-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 19\n    acting: 12\n  by_consequence:\n    read: 19\n    write: 11\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /bonuses\n  method: get\n  operationId: listBonuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bonuses\n  method: post\n  operationId: createBonus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bonuses.atom\n  method: get\n  operationId: listBonusesAtom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bonuses/{id}\n  method: get\n  operationId: retrieveBonus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bonuses/{id}\n  method: put\n  operationId: updateBonus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bonuses/{id}\n  method: delete\n  operationId: deleteBonus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: get\n  operationId: retrieveUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: put\n  operationId:\
  \ updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: delete\n  operationId: deactivateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me\n  method: get\n  operationId: retrieveMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/autocomplete\n  method: get\n  operationId: autocompleteUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/bonuses\n  method: get\n  operationId: listUserBonuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/redemptions\n  method: get\n  operationId: listUserRedemptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/achievements\n  method: get\n  operationId: listUserAchievements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rewards\n  method: get\n  operationId: listRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redemptions\n  method: get\n\
  \  operationId: listRedemptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redemptions/{id}\n  method: get\n  operationId: retrieveRedemption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user_redemptions\n  method: post\n  operationId: createUserRedemption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom_reward_redemptions\n  method: get\n  operationId: listCustomRewardRedemptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /custom_reward_redemptions/approve\n  method: post\n  operationId: approveCustomRewardRedemptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom_reward_redemptions/fulfill\n  method: post\n  operationId: fulfillCustomRewardRedemptions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/health\n  method: get\n  operationId: analyticsHealthcheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/snapshots/analytics_users\n  method: post\n  operationId: queueUsersSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/snapshots/recognition_events\n  method: post\n  operationId: queueRecognitionEventsSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/snapshots/{id}\n  method: get\n  operationId: getSnapshotStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /analytics/analytics_users\n  method: get\n  operationId: listAnalyticsUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/recognition_events\n  method: get\n  operationId: listRecognitionEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company\n  method: get\n  operationId: retrieveCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company\n  method: put\n  operationId: updateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonusly/refs/heads/main/agentic-access/bonusly-agentic-access.yml
summary_line: 31 operations · 12 acting
tags:
- Employee Recognition
- Rewards
- Employee Engagement
- HR
- Company Culture
- Bonuses
---
