---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 19
api_specs:
- filename: ably-apps-api-openapi.yml
  format: yaml
  label: Ably apps API
  slug: ably-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-apps-api-openapi.yml
- filename: ably-authentication-api-openapi.yml
  format: yaml
  label: Ably Authentication API
  slug: ably-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-authentication-api-openapi.yml
- filename: ably-history-api-openapi.yml
  format: yaml
  label: Ably History API
  slug: ably-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-history-api-openapi.yml
- filename: ably-keys-api-openapi.yml
  format: yaml
  label: Ably keys API
  slug: ably-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-keys-api-openapi.yml
- filename: ably-namespaces-api-openapi.yml
  format: yaml
  label: Ably namespaces API
  slug: ably-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-namespaces-api-openapi.yml
- filename: ably-publishing-api-openapi.yml
  format: yaml
  label: Ably Publishing API
  slug: ably-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-publishing-api-openapi.yml
- filename: ably-push-api-openapi.yml
  format: yaml
  label: Ably Push API
  slug: ably-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-push-api-openapi.yml
- filename: ably-queues-api-openapi.yml
  format: yaml
  label: Ably queues API
  slug: ably-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-queues-api-openapi.yml
- filename: ably-rules-api-openapi.yml
  format: yaml
  label: Ably rules API
  slug: ably-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-rules-api-openapi.yml
- filename: ably-stats-api-openapi.yml
  format: yaml
  label: Ably Stats API
  slug: ably-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-stats-api-openapi.yml
- filename: ably-status-api-openapi.yml
  format: yaml
  label: Ably Status API
  slug: ably-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-status-api-openapi.yml
- filename: ably-tokens-api-openapi.yml
  format: yaml
  label: Ably tokens API
  slug: ably-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-tokens-api-openapi.yml
consequence_counts:
  read: 19
  safety-critical: 1
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Ably Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /apps/{app_id}/keys/{key_id}/revoke
operation_count: 44
overview: 'Ably exposes 44 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 24 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ably
provider_slug: ably
slug: ably-agentic-access
source_filename: ably-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ably-control-api-openapi.yml, openapi/ably-platform-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 19\n    acting: 25\n  by_consequence:\n    read: 19\n    write: 24\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /accounts/{account_id}/apps\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/apps\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{id}/pkcs12\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/keys\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id}/keys\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/keys/{key_id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/keys/{key_id}/revoke\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /apps/{app_id}/namespaces\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id}/namespaces\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/namespaces/{namespace_id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/namespaces/{namespace_id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/queues\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id}/queues\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /apps/{app_id}/queues/{queue_id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/rules\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id}/rules\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/rules/{rule_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id}/rules/{rule_id}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id}/rules/{rule_id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{channel_id}/messages\n  method: get\n  operationId: getMessagesByChannel\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{channel_id}/messages\n  method: post\n  operationId: publishMessagesToChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels/{channel_id}/presence\n  method: get\n  operationId: getPresenceOfChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{channel_id}/presence/history\n  method: get\n  operationId: getPresenceHistoryOfChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /channels/{channel_id}\n  method: get\n  operationId: getMetadataOfChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels\n  method: get\n  operationId: getMetadataOfAllChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/deviceRegistrations\n  method: get\n  operationId: getRegisteredPushDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/deviceRegistrations\n  method: post\n  operationId: registerPushDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /push/deviceRegistrations\n  method: delete\n  operationId: unregisterAllPushDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/deviceRegistrations/{device_id}\n  method: get\n  operationId: getPushDeviceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/deviceRegistrations/{device_id}\n  method: put\n  operationId: putPushDeviceDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /push/deviceRegistrations/{device_id}\n  method: patch\n  operationId: patchPushDeviceDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/deviceRegistrations/{device_id}\n  method: delete\n  operationId: unregisterPushDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/deviceRegistrations/{device_id}/resetUpdateToken\n  method: get\n  operationId: updatePushDeviceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/channelSubscriptions\n  method: get\n  operationId: getPushSubscriptionsOnChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/channelSubscriptions\n  method: post\n  operationId: subscribePushDeviceToChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/channelSubscriptions\n  method: delete\n  operationId: deletePushDeviceDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /push/channels\n  method: get\n  operationId: getChannelsWithPushSubscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/publish\n  method: post\n  operationId: publishPushNotificationToDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/{keyName}/requestToken\n  method: post\n  operationId: requestAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time\n  method: get\n  operationId: getTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/agentic-access/ably-agentic-access.yml
summary_line: 44 operations · 25 acting · 1 human-in-the-loop
tags:
- Realtime
- WebSockets
- Pub/Sub
- Messaging
- Streaming
- Push Notifications
- Chat
- LiveSync
---
