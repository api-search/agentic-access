---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 10
api_specs:
- filename: revcontent-stats-management-openapi.yml
  format: yaml
  label: RevContent Stats & Management API
  slug: revcontent-stats-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-stats-management-openapi.yml
consequence_counts:
  read: 10
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Revcontent Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'RevContent exposes 17 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RevContent
provider_slug: revcontent
slug: revcontent-agentic-access
source_filename: revcontent-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/revcontent-stats-management-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 7\n    connected: 10\n  by_consequence:\n    write: 7\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/boosts/add\n  method: post\n  operationId: addBoost\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/boosts/update\n  method: post\n  operationId: updateBoostSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/boosts\n  method: get\n  operationId: getAllBoosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/performance\n  method: get\n  operationId: getBoostPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/update/status\n  method: post\n  operationId: updateBoostStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/boosts/{boost_id}/content\n  method: get\n  operationId: getAllBoostContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/content/{content_id}\n  method: get\n  operationId: getBoostContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/content/{content_id}/widget-stats\n\
  \  method: get\n  operationId: getContentWidgetStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/targets/widgets\n  method: get\n  operationId: getBoostWidgetTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/boosts/{boost_id}/targets/widgets\n  method: post\n  operationId: updateBoostWidgetTargets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/helpers/devices\n  method: get\n  operationId: getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/helpers/operating-systems\n  method: get\n  operationId: getOperatingSystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/helpers/traffic-types\n  method: get\n  operationId: getTrafficTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/helpers/dma\n  method: get\n  operationId: getDMAList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/api/v1.0/account/reactivate\n  method: post\n  operationId: reactivateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats/api/v1.0/data_requests/submit\n  method: post\n  operationId: submitCCPADataRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/agentic-access/revcontent-agentic-access.yml
summary_line: 17 operations · 7 acting
tags:
- Native Advertising
- Content Recommendation
- Ad Network
- Publisher Monetization
- Programmatic Advertising
---
