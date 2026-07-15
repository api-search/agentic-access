---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 2
api_specs:
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking SMS API
  slug: sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking USSD API
  slug: ussd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Voice API
  slug: voice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Airtime API
  slug: airtime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Mobile Data API
  slug: mobile-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
consequence_counts:
  physical: 7
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Africastalking Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /airtime/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/token/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mobile/b2b/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mobile/b2c/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mobile/checkout/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mobile/data/request
operation_count: 14
overview: 'Africa''s Talking exposes 14 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 5 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Africa's Talking
provider_slug: africastalking
slug: africastalking-agentic-access
source_filename: africastalking-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/africastalking-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 12\n    connected: 2\n  by_consequence:\n    physical: 7\n    read: 2\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /messaging\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging\n  method: get\n  operationId: fetchMessages\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/token/create\n  method: post\n  operationId: createCheckoutToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription/create\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription/delete\n  method: post\n  operationId: deleteSubscription\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription\n  method: get\n  operationId: fetchSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airtime/send\n  method: post\n  operationId: sendAirtime\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /call\n  method: post\n  operationId: makeCall\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /queueStatus\n  method: post\n  operationId: queueStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mediaUpload\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile/data/request\n  method: post\n  operationId: sendMobileData\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile/checkout/request\n  method: post\n  operationId: mobileCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile/b2c/request\n  method: post\n  operationId: mobileB2C\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mobile/b2b/request\n  method: post\n  operationId: mobileB2B\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/agentic-access/africastalking-agentic-access.yml
summary_line: 14 operations · 12 acting
tags:
- Communications
- SMS
- USSD
- Voice
- Airtime
- Mobile Data
- Payments
- Africa
---
