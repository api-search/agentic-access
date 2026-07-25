---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 31
api_specs:
- filename: bandwidth-phone-numbers-api-openapi.yml
  format: yaml
  label: Bandwidth Phone Numbers API
  slug: phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-phone-numbers-api-openapi.yml
- filename: bandwidth-mfa-api-openapi.yml
  format: yaml
  label: Bandwidth Multi-Factor Authentication API
  slug: multi-factor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-mfa-api-openapi.yml
- filename: bandwidth-toll-free-verification-api-openapi.yml
  format: yaml
  label: Bandwidth Toll-Free Verification API
  slug: toll-free-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-toll-free-verification-api-openapi.yml
- filename: bandwidth-available-numbers-api-openapi.yml
  format: yaml
  label: Bandwidth Available Numbers API
  slug: bandwidth-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-available-numbers-api-openapi.yml
- filename: bandwidth-calls-api-openapi.yml
  format: yaml
  label: Bandwidth Calls API
  slug: bandwidth-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-calls-api-openapi.yml
- filename: bandwidth-conferences-api-openapi.yml
  format: yaml
  label: Bandwidth Conferences API
  slug: bandwidth-conferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-conferences-api-openapi.yml
- filename: bandwidth-disconnects-api-openapi.yml
  format: yaml
  label: Bandwidth Disconnects API
  slug: bandwidth-disconnects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-disconnects-api-openapi.yml
- filename: bandwidth-emergency-notification-recipients-api-openapi.yml
  format: yaml
  label: Bandwidth Emergency Notification Recipients API
  slug: bandwidth-emergency-notification-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-emergency-notification-recipients-api-openapi.yml
- filename: bandwidth-endpoints-api-openapi.yml
  format: yaml
  label: Bandwidth Endpoints API
  slug: bandwidth-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-endpoints-api-openapi.yml
- filename: bandwidth-locations-api-openapi.yml
  format: yaml
  label: Bandwidth Locations API
  slug: bandwidth-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-locations-api-openapi.yml
- filename: bandwidth-media-api-openapi.yml
  format: yaml
  label: Bandwidth Media API
  slug: bandwidth-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-media-api-openapi.yml
- filename: bandwidth-messages-api-openapi.yml
  format: yaml
  label: Bandwidth Messages API
  slug: bandwidth-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-messages-api-openapi.yml
- filename: bandwidth-number-features-api-openapi.yml
  format: yaml
  label: Bandwidth Number Features API
  slug: bandwidth-number-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-number-features-api-openapi.yml
- filename: bandwidth-orders-api-openapi.yml
  format: yaml
  label: Bandwidth Orders API
  slug: bandwidth-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-orders-api-openapi.yml
- filename: bandwidth-port-ins-api-openapi.yml
  format: yaml
  label: Bandwidth Port-Ins API
  slug: bandwidth-port-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-port-ins-api-openapi.yml
- filename: bandwidth-recordings-api-openapi.yml
  format: yaml
  label: Bandwidth Recordings API
  slug: bandwidth-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-recordings-api-openapi.yml
- filename: bandwidth-sip-peers-api-openapi.yml
  format: yaml
  label: Bandwidth SIP Peers API
  slug: bandwidth-sip-peers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-sip-peers-api-openapi.yml
- filename: bandwidth-sites-api-openapi.yml
  format: yaml
  label: Bandwidth Sites API
  slug: bandwidth-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/openapi/bandwidth-sites-api-openapi.yml
consequence_counts:
  physical: 5
  read: 31
  safety-critical: 1
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Bandwidth Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{accountId}/e911s/notificationRecipients
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/code/messaging
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/code/voice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/tns/{phoneNumber}/tnfeatureorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /users/{accountId}/messages
operation_count: 62
overview: 'Bandwidth exposes 62 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 25 write, 5 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bandwidth
provider_slug: bandwidth
slug: bandwidth-agentic-access
source_filename: bandwidth-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bandwidth-emergency-calling-api-openapi.yml, openapi/bandwidth-messaging-api-openapi.yml,\n  openapi/bandwidth-mfa-api-openapi.yml, openapi/bandwidth-phone-numbers-api-openapi.yml, openapi/bandwidth-toll-free-verification-api-openapi.yml,\n  openapi/bandwidth-voice-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 62\n  by_action_class:\n    connected: 31\n    acting: 31\n  by_consequence:\n    read: 31\n    write: 25\n    safety-critical: 1\n    physical: 5\n  human_in_the_loop_required: 1\noperations:\n- path: /accounts/{accountId}/e911s\n  method: get\n  operationId: listEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/e911s\n  method: post\n  operationId: createEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/e911s/{endpointId}\n  method: get\n  operationId: getEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/e911s/{endpointId}\n  method: put\n  operationId: updateEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /accounts/{accountId}/e911s/{endpointId}\n  method: delete\n  operationId: deleteEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/e911s/locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/e911s/locations\n  method: post\n  operationId: createLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /accounts/{accountId}/e911s/locations/{locationId}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/e911s/locations/{locationId}\n  method: put\n  operationId: updateLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/e911s/locations/{locationId}\n  method: delete\n  operationId: deleteLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /accounts/{accountId}/e911s/notificationRecipients\n  method: get\n  operationId: listNotificationRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/e911s/notificationRecipients\n  method: post\n  operationId: createNotificationRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/{accountId}/messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n     \
  \ purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{accountId}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{accountId}/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{accountId}/media/{mediaName}\n  method: put\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{accountId}/media/{mediaName}\n\
  \  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{accountId}/media/{mediaName}\n  method: delete\n  operationId: deleteMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/code/messaging\n  method: post\n  operationId: createMessagingMfa\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/code/voice\n\
  \  method: post\n  operationId: createVoiceMfa\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/code/verify\n  method: post\n  operationId: verifyMfaCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/availableNumbers\n  method: get\n  operationId: searchAvailableNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /accounts/{accountId}/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/orders/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/portins\n  method: post\n  operationId: createPortIn\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/portins\n  method: get\n  operationId: listPortIns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/portins/{portInId}\n  method: get\n  operationId: getPortIn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/disconnects\n  method: post\n  operationId: createDisconnect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/sites\n  method: post\n  operationId: createSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/sites/{siteId}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/sites/{siteId}\n  method: put\n  operationId: updateSite\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/sites/{siteId}\n  method: delete\n  operationId: deleteSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/sites/{siteId}/sippeers\n  method: get\n  operationId: listSipPeers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/sites/{siteId}/sippeers\n  method: post\n  operationId: createSipPeer\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/sites/{siteId}/sippeers/{sipPeerId}\n  method: get\n  operationId: getSipPeer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/sites/{siteId}/sippeers/{sipPeerId}\n  method: put\n  operationId: updateSipPeer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/sites/{siteId}/sippeers/{sipPeerId}\n  method: delete\n  operationId: deleteSipPeer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/tns\n  method: get\n  operationId: listPhoneNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/tns/{phoneNumber}\n  method: get\n  operationId: getPhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/sites/{siteId}/sippeers/{sipPeerId}/tns\n  method: get\n  operationId: listSipPeerPhoneNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/tns/{phoneNumber}/tnfeatureorder\n\
  \  method: post\n  operationId: updateNumberFeatures\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/tollFreeVerification\n  method: get\n  operationId: listTollFreeVerifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/tollFreeVerification\n  method: post\n  operationId: createTollFreeVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /accounts/{accountId}/tollFreeVerification/{verificationId}\n  method: get\n  operationId: getTollFreeVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/tollFreeVerification/{verificationId}\n  method: put\n  operationId: updateTollFreeVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/calls\n  method: post\n  operationId: createCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/calls/{callId}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/calls/{callId}\n  method: post\n  operationId: updateCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/calls/{callId}/recordings\n  method: get\n  operationId: getCallRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/calls/{callId}/recordings/{recordingId}\n  method: get\n  operationId:\
  \ getCallRecording\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/calls/{callId}/recordings/{recordingId}\n  method: delete\n  operationId: deleteCallRecording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/calls/{callId}/recordings/{recordingId}/media\n  method: get\n  operationId: getCallRecordingMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/calls/{callId}/recordings/{recordingId}/transcription\n  method: post\n  operationId: createRecordingTranscription\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/calls/{callId}/recordings/{recordingId}/transcription\n  method: get\n  operationId: getRecordingTranscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/recordings\n  method: get\n  operationId: listAccountRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/conferences\n  method: get\n  operationId: listConferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /accounts/{accountId}/conferences/{conferenceId}\n  method: get\n  operationId: getConference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/conferences/{conferenceId}\n  method: post\n  operationId: updateConference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/conferences/{conferenceId}/members/{memberId}\n  method: put\n  operationId: updateConferenceMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/conferences/{conferenceId}/recordings\n  method: get\n  operationId: getConferenceRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/agentic-access/bandwidth-agentic-access.yml
summary_line: 62 operations · 31 acting · 1 human-in-the-loop
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
---
