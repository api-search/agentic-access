---
acting_count: 576
action_class_counts:
  acting: 576
  connected: 367
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
  physical: 143
  read: 367
  safety-critical: 15
  write: 418
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 15
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
  method: POST
  path: /numbers/2/numbers/{numberKey}/voice/emergency-service/validate-address
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /vocalize/2/campaigns/{campaignId}/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2fa/2/pin
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2fa/2/pin/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2fa/2/pin/voice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2fa/2/pin/{pinId}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2fa/2/pin/{pinId}/resend/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2fa/2/pin/{pinId}/resend/voice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apple-mfb/1/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apple-mfb/1/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bots/1/testing/{testId}/send-message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /callrouting/1/routes/{routeId}
operation_count: 943
overview: 'Infobip exposes 943 API operations that an AI agent could call, of which 576 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 367 read, 418 write, 143 physical, and 15 safety-critical.


  15 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Infobip
provider_slug: infobip
slug: infobip-agentic-access
source_filename: infobip-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/infobip-ai-hub-api-openapi.yml, openapi/infobip-channels-api-openapi.yml, openapi/infobip-connectivity-api-openapi.yml,\n  openapi/infobip-customer-engagement-api-openapi.yml, openapi/infobip-platform-api-openapi.yml,\n  openapi/infobip-tools-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 943\n  by_action_class:\n    connected: 367\n    acting: 576\n  by_consequence:\n    read: 367\n    physical: 143\n    write: 418\n    safety-critical: 15\n  human_in_the_loop_required: 15\noperations:\n- path: /ai/1/aiassistants/{assistantId}/query\n  method: post\n  operationId: query-ai-assistant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/1/aiassistants/{assistantId}/retrieve-context\n  method: post\n  operationId: retrieve-ai-assistant-context\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/3/messages\n  method: post\n  operationId: send-sms-messages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/3/text/query\n  method: get\n  operationId: send-sms-messages-over-query-parameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/1/text/query\n\
  \  method: get\n  operationId: send-sms-message-over-query-parameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/1/preview\n  method: post\n  operationId: preview-sms-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/2/text/advanced\n  method: post\n  operationId: send-sms-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/2/binary/advanced\n\
  \  method: post\n  operationId: send-binary-sms-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/1/bulks\n  method: get\n  operationId: get-scheduled-sms-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/1/bulks\n  method: put\n  operationId: reschedule-sms-messages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/1/bulks/status\n \
  \ method: get\n  operationId: get-scheduled-sms-messages-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/1/bulks/status\n  method: put\n  operationId: update-scheduled-sms-messages-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ct/1/log/end/{messageId}\n  method: post\n  operationId: log-end-tag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/1/inbox/reports\n  method: get\n  operationId:\
  \ get-inbound-sms-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/3/reports\n  method: get\n  operationId: get-outbound-sms-message-delivery-reports-v3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/3/logs\n  method: get\n  operationId: get-outbound-sms-message-logs-v3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/1/reports\n  method: get\n  operationId: get-outbound-sms-message-delivery-reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/1/logs\n  method: get\n  operationId: get-outbound-sms-message-logs\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mms/2/messages\n  method: post\n  operationId: send-mms-messages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mms/1/advanced\n  method: post\n  operationId: send-mms-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mms/1/content\n  method: post\n  operationId: upload-binary\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mms/1/inbox/reports\n  method: get\n  operationId: get-inbound-mms-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mms/2/reports\n  method: get\n  operationId: get-outbound-mms-message-delivery-reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mms/1/reports\n  method: get\n  operationId: deprecated-get-outbound-mms-message-delivery-reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /mms/2/logs\n  method: get\n  operationId: get-outbound-mms-message-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mms/1/logs\n  method: get\n  operationId: deprecated-get-outbound-mms-message-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/configurations\n  method: get\n  operationId: get-calls-configurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/configurations\n  method: post\n  operationId: create-calls-configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/configurations/{callsConfigurationId}\n  method: get\n  operationId: get-calls-configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/configurations/{callsConfigurationId}\n  method: put\n  operationId: update-calls-configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/configurations/{callsConfigurationId}\n  method: delete\n  operationId: delete-calls-configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls\n  method: get\n  operationId: get-calls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/calls\n  method: post\n  operationId: create-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}\n  method: get\n  operationId: get-call\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/calls/history\n  method: get\n  operationId: get-calls-history\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/calls/{callId}/history\n  method: get\n  operationId: get-call-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/connect\n  method: post\n  operationId: connect-calls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/connect\n  method: post\n  operationId: connect-with-new-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/send-ringing\n  method: post\n  operationId: send-ringing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/pre-answer\n  method: post\n  operationId: pre-answer-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/answer\n  method: post\n  operationId: answer-call\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/hangup\n  method: post\n  operationId: hangup-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/play\n  method: post\n  operationId: call-play-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/stop-play\n  method: post\n  operationId:\
  \ call-stop-playing-file\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calls/1/calls/{callId}/say\n  method: post\n  operationId: call-say-text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/send-dtmf\n  method: post\n  operationId: call-send-dtmf\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/capture/dtmf\n  method: post\n  operationId: call-capture-dtmf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/capture/speech\n  method: post\n  operationId: call-capture-speech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/start-transcription\n  method: post\n  operationId: call-start-transcription\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/stop-transcription\n  method: post\n  operationId: call-stop-transcription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calls/1/calls/{callId}/start-recording\n  method: post\n  operationId: call-start-recording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/stop-recording\n  method: post\n  operationId: call-stop-recording\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calls/1/calls/{callId}/start-media-stream\n  method: post\n  operationId: start-media-stream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/stop-media-stream\n  method: post\n  operationId: stop-media-stream\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calls/1/calls/{callId}/send-message\n  method: post\n  operationId: call-send-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/application-transfer\n  method: post\n  operationId: application-transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/application-transfer/{transferId}/accept\n  method: post\n  operationId: application-transfer-accept\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/calls/{callId}/application-transfer/{transferId}/reject\n  method: post\n  operationId: application-transfer-reject\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences\n  method: get\n  operationId: get-conferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/conferences\n  method: post\n  operationId: create-conference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}\n  method: get\n  operationId: get-conference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/conferences/{conferenceId}\n  method: patch\n  operationId: update-conference\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/history\n  method: get\n  operationId: get-conferences-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/conferences/{conferenceId}/history\n  method: get\n  operationId: get-conference-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/conferences/{conferenceId}/call\n  method: post\n  operationId: add-new-conference-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/call/{callId}\n  method: put\n  operationId: add-existing-conference-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/call/{callId}\n  method: delete\n  operationId: remove-conference-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/call/{callId}\n  method: patch\n  operationId: update-conference-call\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/hangup\n  method: post\n  operationId: hangup-conference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/play\n  method: post\n  operationId: conference-play-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/stop-play\n  method: post\n  operationId: conference-stop-playing-file\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/say\n  method: post\n  operationId: conference-say-text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/start-recording\n  method: post\n  operationId: conference-start-recording\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/stop-recording\n  method: post\n  operationId: conference-stop-recording\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/broadcast-webrtc-text\n  method: post\n  operationId: conference-broadcast-webrtc-text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/conferences/{conferenceId}/send-message\n  method: post\n  operationId: conference-send-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs\n  method: get\n  operationId: get-dialogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/dialogs\n  method: post\n  operationId: create-dialog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs/parent-call/{parentCallId}/child-call/{childCallId}\n  method: post\n  operationId: create-dialog-with-existing-calls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs/{dialogId}\n  method: get\n  operationId: get-dialog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/dialogs/history\n  method: get\n  operationId: get-dialogs-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/dialogs/{dialogId}/history\n\
  \  method: get\n  operationId: get-dialog-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/dialogs/{dialogId}/hangup\n  method: post\n  operationId: hangup-dialog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs/{dialogId}/play\n  method: post\n  operationId: dialog-play-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs/{dialogId}/say\n  method: post\n  operationId:\
  \ dialog-say-text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs/{dialogId}/stop-play\n  method: post\n  operationId: dialog-stop-playing-file\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calls/1/dialogs/{dialogId}/start-recording\n  method: post\n  operationId: dialog-start-recording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs/{dialogId}/stop-recording\n  method: post\n  operationId: dialog-stop-recording\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /calls/1/dialogs/{dialogId}/broadcast-webrtc-text\n  method: post\n  operationId: dialog-broadcast-webrtc-text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs/{dialogId}/send-message\n  method: post\n  operationId: dialog-send-message\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs/{dialogId}/transfer/accept\n  method: post\n  operationId: dialog-transfer-accept\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/dialogs/{dialogId}/transfer/reject\n  method: post\n  operationId: dialog-transfer-reject\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/sip-trunks\n  method: get\n  operationId: get-sip-trunks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/1/sip-trunks\n  method: post\n  operationId: create-sip-trunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/sip-trunks/{sipTrunkId}\n  method: get\n  operationId: get-sip-trunk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /calls/1/sip-trunks/{sipTrunkId}\n  method: put\n  operationId: update-sip-trunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/1/sip-trunks/{sipTrunkId}\n  method: delete\n  operationId: delete-sip-trunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (295 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/agentic-access/infobip-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/agentic-access/infobip-agentic-access.yml
summary_line: 943 operations · 576 acting · 15 human-in-the-loop
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
- Communications
---
