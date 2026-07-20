---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra SMS API
  slug: kaleyra-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra WhatsApp API
  slug: kaleyra-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra RCS API
  slug: kaleyra-rcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra Voice API
  slug: kaleyra-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra Verify (OTP) API
  slug: kaleyra-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra Video API
  slug: kaleyra-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
consequence_counts:
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the modeled OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Kaleyra sends real-world messages, calls, and OTPs, so acting operations carry outbound-communication risk (spend + recipient contact) and default to human-in-the-loop on abnormal/high-value triggers. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kaleyra Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Kaleyra exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kaleyra
provider_slug: kaleyra
slug: kaleyra-agentic-access
source_filename: kaleyra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/kaleyra-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the modeled OpenAPI. A governance starting point for exposing this API to AI agents - review and bind\n  audience per deployment. Kaleyra sends real-world messages, calls, and OTPs, so acting operations\n  carry outbound-communication risk (spend + recipient contact) and default to human-in-the-loop on\n  abnormal/high-value triggers. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 5\n    connected: 2\n  by_consequence:\n    write: 5\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/{sid}/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n      - outbound-communication\n    audit: required\n- path: /v2/{sid}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{sid}/messages/{message_id}\n  method: get\n  operationId: getMessageStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{sid}/verify\n  method: post\n  operationId: generateOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n      - outbound-communication\n    audit: required\n- path: /v1/{sid}/verify/validate\n  method:\
  \ get\n  operationId: validateOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{sid}/voice/click-to-call\n  method: post\n  operationId: clickToCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n      - outbound-communication\n    audit: required\n- path: /v2/rooms\n  method: post\n  operationId: createVideoRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/agentic-access/kaleyra-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- CPaaS
- Messaging
- SMS
- WhatsApp
- Voice
- OTP
- India
---
