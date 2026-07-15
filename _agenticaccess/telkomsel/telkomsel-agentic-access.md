---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 2
api_specs:
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub SMS API
  slug: telkomsel-digihub-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub USSD API
  slug: telkomsel-digihub-ussd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Subscriber Check API
  slug: telkomsel-digihub-subscriber-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Identity Verification API
  slug: telkomsel-digihub-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Location API
  slug: telkomsel-digihub-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub SIM Swap API
  slug: telkomsel-digihub-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Consent Management API
  slug: telkomsel-digihub-consent-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
- filename: telkomsel-openapi.yml
  format: yaml
  label: Telkomsel DigiHub Scoring and Insights API
  slug: telkomsel-digihub-scoring-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-openapi.yml
consequence_counts:
  physical: 3
  read: 2
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Telkomsel Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /digihub/sms/premium
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /digihub/ussd/broadcast
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /digihub/v1/reguler/sendsms
operation_count: 27
overview: 'Telkomsel exposes 27 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 22 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Telkomsel
provider_slug: telkomsel
slug: telkomsel-agentic-access
source_filename: telkomsel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/telkomsel-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 25\n    connected: 2\n  by_consequence:\n    physical: 3\n    read: 2\n    write: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /digihub/v1/reguler/sendsms\n  method: post\n  operationId: sendSMS\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/sms/premium\n  method: post\n\
  \  operationId: sendSMS-84\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/delivery\n  method: get\n  operationId: getDeliveryStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digihub/ussd/broadcast\n  method: post\n  operationId: sendUSSD\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/ussd/deliverystatus\n\
  \  method: get\n  operationId: getUssdDeliveryStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digihub/subscheck/activestatus\n  method: post\n  operationId: activeStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/subscheck/v2/activestatus\n  method: post\n  operationId: activeStatus-137\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/subscheck/subscribertype\n  method: post\n  operationId:\
  \ subscriberType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/subscheck/roamingstatus\n  method: post\n  operationId: roamingStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/subscheck/callforward\n  method: post\n  operationId: callForwarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /digihub/subscheck/recyclev2\n  method: post\n  operationId: Recycle-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/subscheck/nikmatchingv4\n  method: post\n  operationId: NIK-Matching-v4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/ktp/match/v2\n  method: post\n  operationId: ktpMatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/v2/idverification\n  method: post\n  operationId: idVerV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/subscheck/locationverificationv3\n  method: post\n  operationId: Location-Verification-v3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/subscheck/lastlocation\n  method: post\n  operationId: lastLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/subscheck/simswapv2\n  method: post\n  operationId: addSms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check\n  method: post\n  operationId: checkSimSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bc-authorize\n  method: post\n  operationId: API-Documentation\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token\n  method: post\n  operationId: API-Documentation-192\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/v2/consentmgmt\n  method: post\n  operationId: consentManagement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/v1/tscore/premium\n  method: post\n  operationId:\
  \ telcoScore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/v1/generic/telco/score\n  method: post\n  operationId: telcoScore-125\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/subscheck/sesv2\n  method: post\n  operationId: SES-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /digihub/subscheck/interestv2\n  method: post\n  operationId: Interest-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/lifestyle-score\n  method: post\n  operationId: lifestyleScore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digihub/loyalist\n  method: post\n  operationId: customerLoyalty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/agentic-access/telkomsel-agentic-access.yml
summary_line: 27 operations · 25 acting
tags:
- Telecommunications
- Indonesia
- SMS
- Mobile Network
- CPaaS
- Network APIs
- Identity Verification
---
