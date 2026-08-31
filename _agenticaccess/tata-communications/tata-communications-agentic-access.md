---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: tata-communications-cdr-by-customer-message-id-api-openapi.yml
  format: yaml
  label: Tata Communications CDR by Customer Message Id API
  slug: tata-communications-cdr-by-customer-message-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-cdr-by-customer-message-id-api-openapi.yml
- filename: tata-communications-destination-api-openapi.yml
  format: yaml
  label: Tata Communications Destination API
  slug: tata-communications-destination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-destination-api-openapi.yml
- filename: tata-communications-number-intelligence-api-openapi.yml
  format: yaml
  label: Tata Communications Number Intelligence API
  slug: tata-communications-number-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-number-intelligence-api-openapi.yml
- filename: tata-communications-report-api-openapi.yml
  format: yaml
  label: Tata Communications Report API
  slug: tata-communications-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-report-api-openapi.yml
- filename: tata-communications-senderid-api-openapi.yml
  format: yaml
  label: Tata Communications Sender ID API
  slug: tata-communications-senderid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-senderid-api-openapi.yml
- filename: tata-communications-top-25-cdr-by-account-id-time-frame-api-openapi.yml
  format: yaml
  label: Tata Communications TOP 25 CDR by account Id & Time Frame API
  slug: tata-communications-top-25-cdr-by-account-id-time-frame-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-top-25-cdr-by-account-id-time-frame-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tata Communications Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /senderId
operation_count: 7
overview: 'Tata Communications exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tata Communications
provider_slug: tata-communications
slug: tata-communications-agentic-access
source_filename: tata-communications-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/tata-communications-mobile-messaging-exchange-account-administration.json, openapi/tata-communications-mobile-messaging-exchange-cdr-report-api.json,\n  openapi/tata-communications-number-intelligence-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /destination\n  method: get\n  operationId: getdestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: get\n  operationId: getreport\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /senderId\n  method: post\n  operationId: postsenderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CDR/account/{accountId}\n  method: get\n  operationId: top_25_cdr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CDR/message/{messageId}\n  method: get\n  operationId: cdr_by_messageId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /number/{phnum}\n  method:\
  \ get\n  operationId: numberLookupDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records\n  method: get\n  operationId: numberLookupRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/agentic-access/tata-communications-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Telecommunications
- India
- Wholesale Carrier
- CPaaS
- Messaging
- Voice
- IoT
- eSIM
- Number Intelligence
- Connectivity
- Subsea Cable
- Partner Gated
---
