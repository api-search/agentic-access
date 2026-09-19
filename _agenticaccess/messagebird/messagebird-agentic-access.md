---
acting_count: 139
action_class_counts:
  acting: 139
  connected: 215
api_specs:
- filename: messagebird-bird-api-openapi.yml
  format: yaml
  label: Bird API
  slug: bird-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-bird-api-openapi.yml
- filename: messagebird-available-numbers-api-openapi.yml
  format: yaml
  label: messagebird Available Numbers API
  slug: messagebird-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-available-numbers-api-openapi.yml
- filename: messagebird-balance-api-openapi.yml
  format: yaml
  label: messagebird Balance API
  slug: messagebird-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-balance-api-openapi.yml
- filename: messagebird-call-flows-api-openapi.yml
  format: yaml
  label: messagebird Call Flows API
  slug: messagebird-call-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-call-flows-api-openapi.yml
- filename: messagebird-calls-api-openapi.yml
  format: yaml
  label: messagebird Calls API
  slug: messagebird-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-calls-api-openapi.yml
- filename: messagebird-contacts-api-openapi.yml
  format: yaml
  label: messagebird Contacts API
  slug: messagebird-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-contacts-api-openapi.yml
- filename: messagebird-conversations-api-openapi.yml
  format: yaml
  label: messagebird Conversations API
  slug: messagebird-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-conversations-api-openapi.yml
- filename: messagebird-groups-api-openapi.yml
  format: yaml
  label: messagebird Groups API
  slug: messagebird-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-groups-api-openapi.yml
- filename: messagebird-hlr-api-openapi.yml
  format: yaml
  label: messagebird HLR API
  slug: messagebird-hlr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-hlr-api-openapi.yml
- filename: messagebird-legs-api-openapi.yml
  format: yaml
  label: messagebird Legs API
  slug: messagebird-legs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-legs-api-openapi.yml
- filename: messagebird-lookup-api-openapi.yml
  format: yaml
  label: messagebird Lookup API
  slug: messagebird-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-lookup-api-openapi.yml
- filename: messagebird-messages-api-openapi.yml
  format: yaml
  label: messagebird Messages API
  slug: messagebird-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-messages-api-openapi.yml
- filename: messagebird-purchased-numbers-api-openapi.yml
  format: yaml
  label: messagebird Purchased Numbers API
  slug: messagebird-purchased-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-purchased-numbers-api-openapi.yml
- filename: messagebird-recordings-api-openapi.yml
  format: yaml
  label: messagebird Recordings API
  slug: messagebird-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-recordings-api-openapi.yml
- filename: messagebird-templates-api-openapi.yml
  format: yaml
  label: messagebird Templates API
  slug: messagebird-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-templates-api-openapi.yml
- filename: messagebird-transcriptions-api-openapi.yml
  format: yaml
  label: messagebird Transcriptions API
  slug: messagebird-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-transcriptions-api-openapi.yml
- filename: messagebird-verify-api-openapi.yml
  format: yaml
  label: messagebird Verify API
  slug: messagebird-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-verify-api-openapi.yml
- filename: messagebird-voice-messages-api-openapi.yml
  format: yaml
  label: messagebird Voice Messages API
  slug: messagebird-voice-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-voice-messages-api-openapi.yml
- filename: messagebird-webhooks-api-openapi.yml
  format: yaml
  label: messagebird Webhooks API
  slug: messagebird-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-webhooks-api-openapi.yml
consequence_counts:
  physical: 17
  read: 215
  safety-critical: 1
  write: 121
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Messagebird Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/realtime/apps/{realtime_app_id}/keys/{realtime_app_key_id}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /conversations/{conversationId}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /phone-numbers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /phone-numbers/{number}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /phone-numbers/{number}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/email/broadcasts/{broadcast_id}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/email/domains
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/email/domains/{domain_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/email/domains/{domain_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/email/inbox-insights/domain-monitoring
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/email/inbox-insights/domains/{sending_domain}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/numbers/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/realtime/apps/{realtime_app_id}/members/{member_id}/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/whatsapp/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/whatsapp/messages/{message_id}/read
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /voicemessages
operation_count: 354
overview: 'Messagebird exposes 354 API operations that an AI agent could call, of which 139 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 215 read, 121 write, 17 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Messagebird
provider_slug: messagebird
slug: messagebird-agentic-access
source_filename: messagebird-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: generated\nsource: openapi/messagebird-available-numbers-api-openapi.yml, openapi/messagebird-balance-api-openapi.yml,\n  openapi/messagebird-bird-api-openapi.yml, openapi/messagebird-call-flows-api-openapi.yml,\n  openapi/messagebird-calls-api-openapi.yml, openapi/messagebird-contacts-api-openapi.yml, openapi/messagebird-conversations-api-openapi.yml,\n  openapi/messagebird-groups-api-openapi.yml, openapi/messagebird-hlr-api-openapi.yml, openapi/messagebird-legs-api-openapi.yml,\n  openapi/messagebird-lookup-api-openapi.yml, openapi/messagebird-messages-api-openapi.yml,\n  openapi/messagebird-purchased-numbers-api-openapi.yml, openapi/messagebird-recordings-api-openapi.yml,\n  openapi/messagebird-templates-api-openapi.yml, openapi/messagebird-transcriptions-api-openapi.yml,\n  openapi/messagebird-verify-api-openapi.yml, openapi/messagebird-voice-messages-api-openapi.yml,\n  openapi/messagebird-webhooks-api-openapi.yml\ndescription: Recommended\
  \ x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 354\n  by_action_class:\n    connected: 215\n    acting: 139\n  by_consequence:\n    read: 215\n    write: 121\n    physical: 17\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /available-phone-numbers/{countryCode}\n  method: get\n  operationId: listAvailableNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/docs/search\n  method: get\n  operationId: getDocsSearch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/docs/pages\n  method: get\n  operationId: getDocsPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace\n  method: get\n  operationId: getCurrentWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/regions\n  method: get\n  operationId: listRealtimeRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/apps\n  method: post\n  operationId: createRealtimeApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/apps\n  method: get\n  operationId: listRealtimeApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/apps/{realtime_app_id}\n  method: get\n  operationId: getRealtimeApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/apps/{realtime_app_id}\n  method: patch\n  operationId: updateRealtimeApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/apps/{realtime_app_id}\n\
  \  method: delete\n  operationId: deleteRealtimeApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/apps/{realtime_app_id}/events\n  method: post\n  operationId: publishRealtimeAppEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/apps/{realtime_app_id}/batch-events\n  method: post\n  operationId: publishRealtimeAppBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/apps/{realtime_app_id}/channels\n  method: get\n  operationId: listRealtimeAppChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/apps/{realtime_app_id}/channels/{channel_name}\n  method: get\n  operationId: getRealtimeAppChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/apps/{realtime_app_id}/channels/{channel_name}/members\n  method: get\n  operationId: listRealtimeAppChannelMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/apps/{realtime_app_id}/members/{member_id}/disconnect\n  method: post\n  operationId:\
  \ disconnectRealtimeAppMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/apps/{realtime_app_id}/members/{member_id}/events\n  method: post\n  operationId: sendRealtimeAppMemberEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/apps/{realtime_app_id}/keys\n  method: get\n  operationId: listRealtimeAppKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/realtime/apps/{realtime_app_id}/keys\n  method: post\n  operationId: createRealtimeAppKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/apps/{realtime_app_id}/keys/{realtime_app_key_id}/revoke\n  method: post\n  operationId: revokeRealtimeAppKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/email/messages\n  method: post\n  operationId: createEmailMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/messages\n  method: get\n  operationId: listEmailMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/batches\n  method: post\n  operationId: createEmailMessageBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/messages/{message_id}\n  method: get\n  operationId: getEmailMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/email/messages/{message_id}/cancel\n  method: post\n  operationId: cancelEmailMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/messages/{message_id}/recipients\n  method: get\n  operationId: listEmailMessageRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/messages/{message_id}/events\n  method: get\n  operationId: listEmailMessageEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/messages/{message_id}/content\n  method: get\n  operationId: getEmailMessageContent\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/messages/{message_id}/attachments/{attachment_id}\n  method: get\n  operationId: getEmailMessageAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts\n  method: post\n  operationId: createEmailBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/broadcasts\n  method: get\n  operationId: listEmailBroadcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts/export\n\
  \  method: get\n  operationId: getEmailBroadcastsExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts/{broadcast_id}\n  method: get\n  operationId: getEmailBroadcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts/{broadcast_id}\n  method: patch\n  operationId: updateEmailBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/broadcasts/{broadcast_id}\n  method: delete\n  operationId: deleteEmailBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/broadcasts/{broadcast_id}/counts\n  method: get\n  operationId: getEmailBroadcastCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts/{broadcast_id}/send-quota\n  method: get\n  operationId: getEmailBroadcastSendQuota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts/{broadcast_id}/recipients\n  method: get\n  operationId: listEmailBroadcastRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts/{broadcast_id}/recipients/export\n\
  \  method: get\n  operationId: getEmailBroadcastRecipientsExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts/{broadcast_id}/events\n  method: get\n  operationId: listEmailBroadcastEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts/{broadcast_id}/clicked-links\n  method: get\n  operationId: listEmailBroadcastClickedLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/broadcasts/{broadcast_id}/send\n  method: post\n  operationId: sendEmailBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/broadcasts/{broadcast_id}/cancel\n  method: post\n  operationId: cancelEmailBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/batch\n  method: post\n  operationId: createContactBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/{contact_id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/{contact_id}\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /v1/contacts/{contact_id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contacts/{contact_id}/preferences\n  method: get\n  operationId: listContactPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/preferences\n  method: get\n  operationId: listPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/preferences\n  method: post\n  operationId: createPreference\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/preferences/{preference_id}\n  method: get\n  operationId: getPreference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/preferences/{preference_id}\n  method: delete\n  operationId: deletePreference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contact-properties\n  method: post\n  operationId: createContactProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contact-properties\n  method: get\n  operationId: listContactProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contact-properties/{property_id}\n  method: get\n  operationId: getContactProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contact-properties/{property_id}\n  method: patch\n  operationId: updateContactProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/contact-properties/{property_id}/archive\n  method: post\n  operationId: archiveContactProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contact-properties/{property_id}/unarchive\n  method: post\n  operationId: unarchiveContactProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences\n  method: post\n  operationId: createAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences\n  method: get\n  operationId: listAudiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/{audience_id}\n  method: get\n  operationId: getAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/{audience_id}\n  method: patch\n  operationId: updateAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences/{audience_id}\n  method: delete\n\
  \  operationId: deleteAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences/{audience_id}/contacts\n  method: get\n  operationId: listAudienceContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audiences/{audience_id}/contacts\n  method: post\n  operationId: assignAudienceContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences/{audience_id}/contacts/remove\n  method: post\n\
  \  operationId: unassignAudienceContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audiences/{audience_id}/contacts/{contact_id}\n  method: delete\n  operationId: unassignAudienceContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/messages\n  method: post\n  operationId: createSMSMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/messages\n  method: get\n  operationId: listSMSMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/batches\n  method: post\n  operationId: createSMSMessageBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/messages/{message_id}\n  method: get\n  operationId: getSMSMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/messages/{message_id}/events\n  method: get\n  operationId: listSMSMessageEvents\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/templates\n  method: get\n  operationId: listSMSTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/templates/{template_ref}\n  method: get\n  operationId: getSMSTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/templates/{template_ref}/versions\n  method: get\n  operationId: listSMSTemplateVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/templates/{template_ref}/versions/{version_id}\n  method: get\n  operationId: getSMSTemplateVersion\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/templates/{template_ref}/versions/{version_id}/languages\n  method: get\n  operationId: listSMSTemplateVersionLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/templates/{template_ref}/versions/{version_id}/languages/{language}\n  method: get\n  operationId: getSMSTemplateVersionLanguage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/suppressions\n  method: get\n  operationId: listSMSSuppressions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/suppressions\n  method: post\n  operationId: createSMSSuppression\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/suppressions/{suppression_id}\n  method: get\n  operationId: getSMSSuppression\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/suppressions/{suppression_id}\n  method: delete\n  operationId: deleteSMSSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/keyword-rules\n  method: get\n  operationId: listSMSKeywordRules\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/keyword-rules\n  method: post\n  operationId: createSMSKeywordRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/keyword-rules/{id}\n  method: get\n  operationId: getSMSKeywordRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/keyword-rules/{id}\n  method: patch\n  operationId: updateSMSKeywordRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/sms/keyword-rules/{id}\n  method: delete\n  operationId: deleteSMSKeywordRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/stats/summary\n  method: get\n  operationId: getSMSStatsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/daily\n  method: get\n  operationId: getSMSStatsDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/hourly\n  method: get\n  operationId: getSMSStatsHourly\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/originators\n  method: get\n  operationId: getSMSStatsByOriginator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/countries\n  method: get\n  operationId: getSMSStatsByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/categories\n  method: get\n  operationId: getSMSStatsByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/error-codes\n  method: get\n  operationId: getSMSStatsByErrorCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/sms/stats/carriers\n  method: get\n  operationId: getSMSStatsByCarrier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/tags\n  method: get\n  operationId: getSMSStatsByTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/statuses\n  method: get\n  operationId: getSMSStatsByStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/inbound/summary\n  method: get\n  operationId: getSMSInboundStatsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/inbound/daily\n  method: get\n  operationId:\
  \ getSMSInboundStatsDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/inbound/hourly\n  method: get\n  operationId: getSMSInboundStatsHourly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/inbound/countries\n  method: get\n  operationId: getSMSInboundStatsByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/inbound/operators\n  method: get\n  operationId: getSMSInboundStatsByOperator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sms/stats/inbound/numbers\n  method: get\n  operationId: getSMSInboundStatsByNumber\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookup/phone-number\n  method: post\n  operationId: createPhoneNumberLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lookup/phone-number/{number}\n  method: get\n  operationId: getPhoneNumberLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookup/email\n  method: post\n  operationId: createEmailLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lookup/email/{address}\n  method: get\n  operationId: getEmailLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify/verifications\n  method: post\n  operationId: createVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify/verifications/check\n  method: post\n  operationId: createVerificationCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-val\n\n# --- truncated at 32 KB (99 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/agentic-access/messagebird-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/agentic-access/messagebird-agentic-access.yml
summary_line: 354 operations · 139 acting · 1 human-in-the-loop
tags:
- Communications
- Messaging
- SMS
- Email
- WhatsApp
- Voice
- Verification
- CPaaS
- Webhook
- Agents
---
