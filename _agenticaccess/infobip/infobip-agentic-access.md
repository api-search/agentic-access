---
acting_count: 1172
action_class_counts:
  acting: 1172
  connected: 714
api_specs:
- filename: infobip-ai-hub-api-openapi.yml
  format: yaml
  label: Infobip AI Hub API
  slug: infobip-ai-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-ai-hub-api-openapi.yml
- filename: infobip-channels-api-openapi.yml
  format: yaml
  label: Infobip Channels API
  slug: infobip-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-channels-api-openapi.yml
- filename: infobip-connectivity-api-openapi.yml
  format: yaml
  label: Infobip Connectivity API
  slug: infobip-connectivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-connectivity-api-openapi.yml
- filename: infobip-customer-engagement-api-openapi.yml
  format: yaml
  label: Infobip Customer Engagement API
  slug: infobip-customer-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-customer-engagement-api-openapi.yml
- filename: infobip-platform-api-openapi.yml
  format: yaml
  label: Infobip Platform API
  slug: infobip-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-platform-api-openapi.yml
- filename: infobip-tools-api-openapi.yml
  format: yaml
  label: Infobip Tools API
  slug: infobip-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-tools-api-openapi.yml
consequence_counts:
  physical: 296
  read: 714
  safety-critical: 30
  write: 846
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 30
kind: agentic-access
layout: agentic-access
method: generated
name: Infobip Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bots/1/testing/{testId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bots/1/testing/{testId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/calls/{callId}/stop-media-stream
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/calls/{callId}/stop-media-stream
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/calls/{callId}/stop-play
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/calls/{callId}/stop-play
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/calls/{callId}/stop-recording
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/calls/{callId}/stop-recording
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/calls/{callId}/stop-transcription
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/calls/{callId}/stop-transcription
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/conferences/{conferenceId}/stop-play
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/conferences/{conferenceId}/stop-play
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/conferences/{conferenceId}/stop-recording
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/conferences/{conferenceId}/stop-recording
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/dialogs/{dialogId}/stop-play
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/dialogs/{dialogId}/stop-play
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/dialogs/{dialogId}/stop-recording
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/dialogs/{dialogId}/stop-recording
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/sip-trunks/{sipTrunkId}/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/1/sip-trunks/{sipTrunkId}/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /numbers/2/numbers/{numberKey}/voice/emergency-service
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /numbers/2/numbers/{numberKey}/voice/emergency-service
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /numbers/2/numbers/{numberKey}/voice/emergency-service
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /numbers/2/numbers/{numberKey}/voice/emergency-service
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /numbers/2/numbers/{numberKey}/voice/emergency-service
operation_count: 1886
overview: 'Infobip exposes 1886 API operations that an AI agent could call, of which 1172 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 714 read, 846 write, 296 physical, and 30 safety-critical.


  30 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Infobip
provider_slug: infobip
slug: infobip-agentic-access
source_filename: infobip-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/infobip-2fa-openapi.json, openapi/infobip-account-management-openapi.json, openapi/infobip-ai-assistants-openapi.json,\n  openapi/infobip-answers-openapi.json, openapi/infobip-apple-mfb-openapi.json, openapi/infobip-application-entity-openapi.json,\n  openapi/infobip-billing-usage-api-openapi.json, openapi/infobip-biometrics-openapi.json, openapi/infobip-blocklist-openapi.json,\n  openapi/infobip-camara-openapi.json, openapi/infobip-catalogs-api-openapi.json, openapi/infobip-common-assets-openapi.json,\n  openapi/infobip-conversations-openapi.json, openapi/infobip-email-openapi.json, openapi/infobip-instagram-openapi.json,\n  openapi/infobip-kakao-openapi.json, openapi/infobip-knowledge-base-openapi.json, openapi/infobip-line-openapi.json,\n  openapi/infobip-live-chat-openapi.json, openapi/infobip-messages-api-openapi.json, openapi/infobip-messenger-openapi.json,\n  openapi/infobip-metrics-api-openapi.json, openapi/infobip-mms-openapi.json,\
  \ openapi/infobip-mobile-app-messaging-openapi.json,\n  openapi/infobip-mobile-identity-openapi.json, openapi/infobip-moments-openapi.json, openapi/infobip-number-activation-state-openapi.json,\n  openapi/infobip-number-lookup-openapi.json, openapi/infobip-numbers-openapi.json, openapi/infobip-omni-failover-openapi.json,\n  openapi/infobip-open-channel-openapi.json, openapi/infobip-openapi-openapi.json, openapi/infobip-people-openapi.json,\n  openapi/infobip-platform-full-openapi.json, openapi/infobip-rcs-openapi.json, openapi/infobip-resources-openapi.json,\n  openapi/infobip-sending-strategy-openapi.json, openapi/infobip-signals-openapi.json, openapi/infobip-sms-openapi.json,\n  openapi/infobip-subscriptions-api-openapi.json, openapi/infobip-tiktok-openapi.json, openapi/infobip-viber-openapi.json,\n  openapi/infobip-vocalize-openapi.json, openapi/infobip-voice-openapi.json, openapi/infobip-webrtc-calls-openapi.json,\n  openapi/infobip-whatsapp-openapi.json, openapi/infobip-zalo-openapi.json\n\
  description: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1886\n  by_action_class:\n    connected: 714\n    acting: 1172\n  by_consequence:\n    read: 714\n    write: 846\n    physical: 296\n    safety-critical: 30\n  human_in_the_loop_required: 30\noperations:\n- path: /2fa/2/applications\n  method: get\n  operationId: get-2fa-applications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2fa/2/applications\n  method: post\n  operationId: create-2fa-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/applications/{appId}\n  method: get\n  operationId: get-2fa-application\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2fa/2/applications/{appId}\n  method: put\n  operationId: update-2fa-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/applications/{appId}/messages\n  method: get\n  operationId: get-2fa-message-templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2fa/2/applications/{appId}/messages\n  method: post\n  operationId:\
  \ create-2fa-message-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/applications/{appId}/messages/{msgId}\n  method: get\n  operationId: get-2fa-message-template\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2fa/2/applications/{appId}/messages/{msgId}\n  method: put\n  operationId: update-2fa-message-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/applications/{appId}/email/messages\n\
  \  method: post\n  operationId: create-2fa-email-message-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/applications/{appId}/email/messages/{msgId}\n  method: put\n  operationId: update-2fa-email-message-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/pin\n  method: post\n  operationId: send-2fa-pin-code-over-sms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n   \
  \   purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/pin/{pinId}/resend\n  method: post\n  operationId: resend-2fa-pin-code-over-sms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/pin/voice\n  method: post\n  operationId: send-2fa-pin-code-over-voice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /2fa/2/pin/{pinId}/resend/voice\n  method: post\n  operationId: resend-2fa-pin-code-over-voice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/pin/email\n  method: post\n  operationId: send-2fa-pin-code-over-email\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/pin/{pinId}/resend/email\n  method: post\n  operationId: resend-2fa-pin-code-over-email\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/pin/{pinId}/verify\n  method: post\n  operationId: verify-2fa-phone-number\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2fa/2/applications/{appId}/verifications\n  method: get\n  operationId: get-2fa-verification-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/1/balance\n  method:\
  \ get\n  operationId: get-account-balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/1/free-messages\n  method: get\n  operationId: get-free-messages-count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/1/total-balance\n  method: get\n  operationId: get-total-account-balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/1/accounts\n  method: get\n  operationId: get-all-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/1/accounts/{accountKey}\n  method: put\n  operationId: update-account\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/1/accounts/{accountKey}/api-keys\n  method: get\n  operationId: get-api-keys-by-filter-deprecated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/1/accounts/{accountKey}/api-keys\n  method: post\n  operationId: create-api-key-deprecated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/1/accounts/{accountKey}/api-keys/{key}\n  method: get\n  operationId: get-api-key-deprecated\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/1/accounts/{accountKey}/api-keys/{key}\n  method: put\n  operationId: update-api-key-deprecated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/2/api-keys\n  method: get\n  operationId: get-api-keys-by-filter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/2/api-keys\n  method: post\n  operationId: create-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/2/api-keys/{apiKeyId}\n  method: get\n  operationId: get-api-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/2/api-keys/{apiKeyId}\n  method: put\n  operationId: update-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/1/session\n  method: post\n  operationId: create-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /auth/1/session\n  method: delete\n  operationId: destroy-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/1/oauth2/token\n  method: post\n  operationId: create-oauth2-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audit/1/logs/export\n  method: get\n  operationId: export-audit-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /audit/1/logs\n  method: get\n  operationId: search-audit-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/1/aiassistants/{assistantId}/query\n  method: post\n  operationId: query-ai-assistant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/1/aiassistants/{assistantId}/retrieve-context\n  method: post\n  operationId: retrieve-ai-assistant-context\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bots/1/testing/start\n\
  \  method: post\n  operationId: start-test\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bots/1/testing/{testId}/stop\n  method: post\n  operationId: stop-test\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bots/1/testing/{testId}/send-message\n  method: post\n  operationId: send-test-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apple-mfb/1/messages\n  method: post\n  operationId: send-apple-mfb-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apple-mfb/1/events\n  method: post\n  operationId: send-apple-mfb-event\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apple-mfb/1/reports\n\
  \  method: get\n  operationId: get-outbound-apple-mfb-message-delivery-reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apple-mfb/1/logs\n  method: get\n  operationId: get-outbound-apple-mfb-message-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/1/applications\n  method: get\n  operationId: get-applications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/1/applications\n  method: post\n  operationId: create-application\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/1/applications/{applicationId}\n  method: get\n  operationId: get-application\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/1/applications/{applicationId}\n  method: put\n  operationId: modify-application\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/1/applications/{applicationId}\n  method: delete\n  operationId: delete-application\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/1/entities\n  method: get\n  operationId: get-entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/1/entities\n  method: post\n  operationId: create-entity\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/1/entities/{entityId}\n  method: get\n  operationId: get-entity\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/1/entities/{entityId}\n  method: put\n  operationId: modify-entity\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/1/entities/{entityId}\n  method: delete\n  operationId: delete-entity\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/1/associations\n  method: get\n  operationId:\
  \ get-resource-associations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provisioning/1/associations\n  method: post\n  operationId: create-resource-association\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provisioning/1/associations\n  method: delete\n  operationId: delete-resource-association\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /provisioning/1/associations/single\n  method: get\n  operationId: get-resource-association\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/1/usage/query\n  method: post\n  operationId: query-billing-usage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biometrics/1/scenarios\n  method: get\n  operationId: get-biometrics-scenarios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /biometrics/1/extraction/sessions\n  method: get\n  operationId: get-biometrics-extraction-session\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /biometrics/1/extraction/sessions\n  method: post\n  operationId: create-biometrics-extraction-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biometrics/1/extraction/sessions\n  method: delete\n  operationId: delete-biometrics-extraction-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biometrics/1/kyc/sessions\n  method: get\n  operationId: get-biometrics-kyc-session\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /biometrics/1/kyc/sessions\n  method: post\n  operationId: create-biometrics-kyc-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biometrics/1/kyc/sessions\n  method: delete\n  operationId: delete-biometrics-kyc-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biometrics/1/enrollment/sessions\n  method: get\n  operationId: get-biometrics-enrollment-session\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /biometrics/1/enrollment/sessions\n  method: post\n  operationId: create-biometrics-enrollment-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biometrics/1/enrollment/sessions\n  method: delete\n  operationId: delete-biometrics-enrollment-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biometrics/1/verification/sessions\n  method: get\n  operationId:\
  \ get-biometrics-verification-session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /biometrics/1/verification/sessions\n  method: post\n  operationId: create-biometrics-verification-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /biometrics/1/verification/sessions\n  method: delete\n  operationId: delete-biometrics-verification-session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/1/blocklists\n\
  \  method: get\n  operationId: get-all-blocklists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/1/blocklists\n  method: post\n  operationId: create-blocklists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platform/1/blocklists\n  method: delete\n  operationId: delete-blocklists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /camara/number-verification/v0/authorize\n  method: get\n  operationId: authorize-number-verify\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /camara/number-verification/v0/verify\n  method: post\n  operationId: verify-number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /camara/number-verification/v2/dcql\n  method: post\n  operationId: create-dcql-request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /camara/number-verification/v2/device-phone-number\n  method: get\n  operationId: get-device-phone-number\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /camara/number-verification/v2/verify\n  method: post\n  operationId: verify-number-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /camara/location/v0/verify\n  method: post\n  operationId: verify-device-location\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /camara/sim-swap/v0/check\n  method: post\n  operationId: sim-swap-check\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /camara/sim-swap/v0/retrieve-date\n  method: post\n  operationId: sim-swap-retrieve-date\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /camara/kyc-match/v0.3/match\n  method: post\n  operationId: know-your-customer-match\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/1/catalogs\n\
  \  method: get\n  operationId: get-catalogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/1/catalogs\n  method: post\n  operationId: create-catalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/1/catalogs/{id}\n  method: get\n  operationId: get-catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/1/catalogs/{id}\n  method: delete\n  operationId: delete-catalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/1/catalogs/{id}\n  method: patch\n  operationId: update-catalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/1/catalogs/{catalogId}/fields\n  method: get\n  operationId: get-catalog-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/1/catalogs/{catalogId}/fields\n  method: post\n  operationId: create-catalog-fields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/1/catalogs/{catalogId}/fields/{fieldId}\n  method: get\n  operationId: get-catalog-field\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/1/catalogs/{catalogId}/fields/{fieldId}\n  method: delete\n  operationId: delete-catalog-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/1/catalogs/{catalogId}/fields/{fieldId}\n  method: patch\n  operationId: update-catalog-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: require\n\n# --- truncated at 32 KB (595 KB\
  \ total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/agentic-access/infobip-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/agentic-access/infobip-agentic-access.yml
summary_line: 1886 operations · 1172 acting · 30 human-in-the-loop
tags:
- Telecommunications
- Croatia
- CPaaS
- Messaging
- SMS
- Voice
- RCS
- WhatsApp
- Email
- Network APIs
- CAMARA
- Open Gateway
- Identity Verification
- SIM Swap
- Number Verification
- Omnichannel
- Aggregator
- Customer Engagement
---
