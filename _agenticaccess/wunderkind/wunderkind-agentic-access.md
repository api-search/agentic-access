---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 2
api_specs:
- filename: wunderkind-email-openapi.yml
  format: yaml
  label: Wunderkind Email API
  slug: wunderkind-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-email-openapi.yml
- filename: wunderkind-identity-openapi.yml
  format: yaml
  label: Wunderkind Identity API
  slug: wunderkind-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-identity-openapi.yml
- filename: wunderkind-ucrm-openapi.yml
  format: yaml
  label: Wunderkind UCRM API
  slug: wunderkind-ucrm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-ucrm-openapi.yml
- filename: wunderkind-event-ingestion-openapi.yml
  format: yaml
  label: Wunderkind Event Ingestion API
  slug: wunderkind-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/openapi/wunderkind-event-ingestion-openapi.yml
consequence_counts:
  physical: 12
  read: 2
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wunderkind Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /email/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/add-to-cart
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/app-push-action
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/app-push-toggle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/app-push-token-set
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/custom
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/empty-cart
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/order-transaction
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/page-view
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/track-link
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/user-identified
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events/visit
operation_count: 23
overview: 'Wunderkind exposes 23 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 9 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wunderkind
provider_slug: wunderkind
slug: wunderkind-agentic-access
source_filename: wunderkind-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/wunderkind-email-openapi.yml, openapi/wunderkind-event-ingestion-openapi.yml,\n  openapi/wunderkind-identity-openapi.yml, openapi/wunderkind-signals-wunderhook-openapi.yml,\n  openapi/wunderkind-ucrm-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 21\n    connected: 2\n  by_consequence:\n    physical: 12\n    write: 9\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /email/send\n  method: post\n  operationId: sendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/add-to-cart\n  method: post\n  operationId: Service_AddToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/app-push-action\n  method: post\n  operationId: Service_AppPushAction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/app-push-toggle\n  method:\
  \ post\n  operationId: Service_AppPushToggle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/app-push-token-set\n  method: post\n  operationId: Service_AppPushTokenSet\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/custom\n  method: post\n  operationId: Service_Custom\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/empty-cart\n  method: post\n  operationId: Service_EmptyCart\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/order-transaction\n  method: post\n  operationId: Service_OrderTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /events/page-view\n  method: post\n  operationId: Service_Pageview\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/track-link\n  method: post\n  operationId: Service_TrackLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/user-identified\n  method: post\n  operationId: Service_UserIdentified\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/visit\n  method: post\n  operationId: Service_Visit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /id-resolution/v1/identity/lookup/batch\n  method: post\n  operationId: post_id-resolutionv1identitylookupbatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: //v1/identity/lookup\n  method: post\n  operationId: get_v1identitylookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /id-resolution/v1/identity/enckey\n  method: post\n  operationId: post_id-resolutionv1identityenckey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /id-resolution/v1/identity/enckey\n  method: get\n  operationId: get_id-resolutionv1identityenckey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: //id-resolution/v1/identity/enckey\n  method: get\n  operationId: get_id-resolutionv1identityenckey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /id-resolution/v1/identity/lookup/batch\n  method: post\n  operationId: post_id-resolutionv1identitylookupbatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identity/lookup\n  method: post\n  operationId: post_v1identitylookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /id-resolution/v1/identity/enckey\n  method: post\n  operationId: post_id-resolutionv1identityenckey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: get_new-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ucrm/v1/unsubscribe\n  method: put\n  operationId: external_unsubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ucrm/v1/subscribe\n  method: put\n  operationId: external_subscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wunderkind/refs/heads/main/agentic-access/wunderkind-agentic-access.yml
summary_line: 23 operations · 21 acting
tags:
- Company
- Marketing
- Personalization
- Identity Resolution
- Email
- SMS
- Behavioral Data
- eCommerce
- Webhooks
---
