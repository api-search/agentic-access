---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 3
api_specs:
- filename: bluecore-openapi.yml
  format: yaml
  label: Bluecore API
  slug: bluecore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-openapi.yml
consequence_counts:
  physical: 3
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bluecore Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/direct-send-campaigns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/direct-send-messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/transactional-messages/{id}
operation_count: 9
overview: 'Bluecore exposes 9 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 3 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bluecore
provider_slug: bluecore
slug: bluecore-agentic-access
source_filename: bluecore-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/bluecore-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 3\n    acting: 6\n  by_consequence:\n    read: 3\n    write: 3\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /namespaces/{namespace}/customers\n  method: get\n  operationId: Profile_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customers.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/customers\n  method: post\n  operationId: Profile_CreateOrUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - customers.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/direct-send-campaigns\n  method: post\n  operationId: CampaignsAPIPublic_CreateDirectSendCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - directsend.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/direct-send-messages\n  method: post\n  operationId: DirectSend_Send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - direct_send.api\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/eligibility\n  method: get\n  operationId: Eligibility_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - eligibility.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/eligibility_events\n  method: post\n  operationId: Eligibility_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - eligibility.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /namespaces/{namespace}/transactional-messages/{id}\n  method: get\n  operationId: Transactional_Get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - transactional.api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /namespaces/{namespace}/transactional-messages/{id}\n  method: post\n  operationId: Transactional_Send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - transactional.api\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: Authn_GetAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/agentic-access/bluecore-agentic-access.yml
summary_line: 9 operations · 6 acting
tags:
- Company
- Retail
- Marketing
- Customer Data Platform
- Personalization
- Email
- SMS
- Messaging
- eCommerce
- Consent
---
