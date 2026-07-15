---
acting_count: 250
action_class_counts:
  acting: 250
  connected: 237
api_specs:
- filename: ringcentral-platform-openapi.yml
  format: yaml
  label: RingCentral Voice API
  slug: ringcentral-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/openapi/ringcentral-platform-openapi.yml
- filename: ringcentral-subscriptions-asyncapi.yaml
  format: yaml
  label: RingCentral Webhooks and Subscriptions API
  slug: ringcentral-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/asyncapi/ringcentral-subscriptions-asyncapi.yaml
consequence_counts:
  physical: 7
  read: 237
  safety-critical: 47
  write: 196
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 47
kind: agentic-access
layout: agentic-access
method: generated
name: Ringcentral Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/oauth/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /restapi/v1.0/account/{accountId}/device/{deviceId}/emergency
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/devices/bulk-assign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/networks
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/networks/{networkId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/networks/{networkId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/switches
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/switches-bulk-create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/switches-bulk-update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/switches-bulk-validate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/switches/{switchId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/switches/{switchId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/users/bulk-assign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/wireless-points
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/wireless-points-bulk-create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/wireless-points-bulk-update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/wireless-points-bulk-validate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/wireless-points/{pointId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /restapi/v1.0/account/{accountId}/emergency-address-auto-update/wireless-points/{pointId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/emergency-locations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /restapi/v1.0/account/{accountId}/emergency-locations/{locationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /restapi/v1.0/account/{accountId}/emergency-locations/{locationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /restapi/v1.0/account/{accountId}/extension/{extensionId}/emergency-locations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /restapi/v1.0/account/{accountId}/extension/{extensionId}/emergency-locations/{locationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /restapi/v1.0/account/{accountId}/extension/{extensionId}/emergency-locations/{locationId}
operation_count: 487
overview: 'RingCentral exposes 487 API operations that an AI agent could call, of which 250 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 237 read, 196 write, 7 physical, and 47 safety-critical.


  47 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RingCentral
provider_slug: ringcentral
slug: ringcentral-agentic-access
source_filename: ringcentral-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ringcentral-platform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 487\n  by_action_class:\n    connected: 237\n    acting: 250\n  by_consequence:\n    read: 237\n    write: 196\n    safety-critical: 47\n    physical: 7\n  human_in_the_loop_required: 47\noperations:\n- path: /webinar/notifications/v1/subscriptions\n  method: get\n  operationId: rcwN11sListSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/notifications/v1/subscriptions\n  method: post\n  operationId: rcwN11sCreateSubscription\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/notifications/v1/subscriptions/{subscriptionId}\n  method: get\n  operationId: rcwN11sGetSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/notifications/v1/subscriptions/{subscriptionId}\n  method: put\n  operationId: rcwN11sUpdateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/notifications/v1/subscriptions/{subscriptionId}\n  method: delete\n  operationId: rcwN11sDeleteSubscription\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/notifications/v1/subscriptions/{subscriptionId}/renew\n  method: post\n  operationId: rcwN11sRenewSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/history/v1/webinars/{webinarId}\n  method: get\n  operationId: rcwHistoryGetWebinar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/webinars/{webinarId}/sessions/{sessionId}\n\
  \  method: get\n  operationId: rcwHistoryGetSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/webinars/{webinarId}/sessions/{sessionId}/participants\n  method: get\n  operationId: rcwHistoryListParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/webinars/{webinarId}/sessions/{sessionId}/participants/self\n  method: get\n  operationId: rcwHistoryGetParticipantInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/webinars/{webinarId}/sessions/{sessionId}/invitees\n  method: get\n  operationId: rcwHistoryListInvitees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/webinars/{webinarId}/sessions/{sessionId}/invitees/{inviteeId}\n  method: get\n  operationId: rcwHistoryGetInvitee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/company/recordings\n  method: get\n  operationId: rcwHistoryAdminListRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/company/recordings/{recordingId}\n  method: get\n  operationId: rcwHistoryAdminGetRecording\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/company/sessions\n  method: get\n  operationId: rcwHistoryListAllCompanySessions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/recordings\n  method: get\n  operationId: rcwHistoryListRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/recordings/{recordingId}\n  method: get\n  operationId: rcwHistoryGetRecording\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/recordings/{recordingId}/download\n  method: get\n  operationId: rcwHistoryGetRecordingDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/history/v1/sessions\n  method: get\n  operationId: rcwHistoryListAllSessions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/registration/v1/sessions/{sessionId}\n  method: get\n  operationId: rcwRegGetSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/registration/v1/sessions/{sessionId}\n  method: patch\n  operationId: rcwRegUpdateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/registration/v1/sessions/{sessionId}/registrants\n  method: get\n  operationId: rcwRegListRegistrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /webinar/registration/v1/sessions/{sessionId}/registrants\n  method: post\n  operationId: rcwRegCreateRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/registration/v1/sessions/{sessionId}/registrants/{registrantId}\n  method: get\n  operationId: rcwRegGetRegistrant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/registration/v1/sessions/{sessionId}/registrants/{registrantId}\n  method: delete\n  operationId: rcwRegDeleteRegistrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/webinars\n  method: post\n  operationId: rcwConfigCreateWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/webinars\n  method: get\n  operationId: rcwConfigListWebinars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/configuration/v1/webinars/{webinarId}\n  method: get\n  operationId: rcwConfigGetWebinar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/configuration/v1/webinars/{webinarId}\n\
  \  method: patch\n  operationId: rcwConfigUpdateWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/webinars/{webinarId}\n  method: delete\n  operationId: rcwConfigDeleteWebinar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/webinars/{webinarId}/sessions\n  method: post\n  operationId: rcwConfigCreateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/webinars/{webinarId}/sessions/{sessionId}\n  method: patch\n  operationId: rcwConfigUpdateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/webinars/{webinarId}/sessions/{sessionId}\n  method: get\n  operationId: rcwConfigGetSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/configuration/v1/webinars/{webinarId}/sessions/{sessionId}\n  method: delete\n  operationId: rcwConfigDeleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/webinars/{webinarId}/sessions/{sessionId}/invitees\n  method: patch\n  operationId: rcwConfigUpdateInvitees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/webinars/{webinarId}/sessions/{sessionId}/invitees\n  method: get\n  operationId: rcwConfigListInvitees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/configuration/v1/webinars/{webinarId}/sessions/{sessionId}/invitees/{inviteeId}\n\
  \  method: get\n  operationId: rcwConfigGetInvitee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/configuration/v1/webinars/{webinarId}/sessions/{sessionId}/invitees/{inviteeId}\n  method: put\n  operationId: rcwConfigUpdateInvitee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/webinars/{webinarId}/sessions/{sessionId}/invitees/{inviteeId}\n  method: delete\n  operationId: rcwConfigDeleteInvitee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /webinar/configuration/v1/company/sessions\n  method: get\n  operationId: rcwConfigListAllCompanySessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webinar/configuration/v1/sessions\n  method: get\n  operationId: rcwConfigListAllSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/recording/{recordingId}/content\n  method: get\n  operationId: readCallRecordingContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/greeting/{greetingId}/content\n  method: get\n  operationId: readAccountGreetingContent\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/extension/{extensionId}/greeting/{greetingId}/content\n  method: get\n  operationId: readGreetingContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/extension/{extensionId}/profile-image/{scaleSize}\n  method: get\n  operationId: readScaledProfileImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/extension/{extensionId}/message-store/{messageId}/content/{attachmentId}\n  method: get\n  operationId: readMessageContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /restapi/v1.0/account/{accountId}/ivr-prompts/{promptId}/content\n  method: get\n  operationId: readIVRPromptContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcvideo/v2/account/{accountId}/extension/{extensionId}/bridges\n  method: post\n  operationId: createBridge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcvideo/v2/account/{accountId}/extension/{extensionId}/bridges/default\n  method: get\n  operationId: getDefaultBridge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcvideo/v2/bridges/pin/pstn/{pin}\n\
  \  method: get\n  operationId: getBridgeByPstnPin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcvideo/v2/bridges/pin/web/{pin}\n  method: get\n  operationId: getBridgeByWebPin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcvideo/v2/bridges/{bridgeId}\n  method: get\n  operationId: getBridge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcvideo/v2/bridges/{bridgeId}\n  method: patch\n  operationId: updateBridge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /rcvideo/v2/bridges/{bridgeId}\n  method: delete\n  operationId: deleteBridge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcvideo/v1/account/{accountId}/recordings\n  method: get\n  operationId: getAccountRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcvideo/v1/account/{accountId}/extension/{extensionId}/recordings\n  method: get\n  operationId: getExtensionRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcvideo/v1/accounts/{accountId}/extensions/{extensionId}/delegators\n  method:\
  \ get\n  operationId: rcvListDelegators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcvideo/v1/history/meetings\n  method: get\n  operationId: listVideoMeetings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcvideo/v1/history/meetings/{meetingId}\n  method: get\n  operationId: getVideoMeeting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi\n  method: get\n  operationId: readAPIVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/oauth/token\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/oauth/authorize\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/oauth/authorize\n  method: post\n  operationId: authorize2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/oauth/revoke\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /restapi/v2/accounts/{accountId}\n  method: get\n  operationId: getAccountInfoV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v2/accounts/{accountId}/device-inventory\n  method: post\n  operationId: addDeviceToInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/device-inventory\n  method: delete\n  operationId: deleteDeviceFromInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/send-welcome-email\n  method: post\n  operationId: sendWelcomeEmailV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/phone-numbers\n  method: get\n  operationId: listAccountPhoneNumbersV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v2/accounts/{accountId}/phone-numbers\n  method: delete\n  operationId: deleteNumbersFromInventoryV2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/phone-numbers/{phoneNumberId}\n  method: patch\n  operationId: assignPhoneNumberV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/phone-numbers/{phoneNumberId}/replace\n  method: post\n  operationId: replacePhoneNumberV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/phone-numbers/bulk-add\n  method: post\n  operationId: addNumbersToInventoryV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/phone-numbers/bulk-add/{taskId}\n  method: get\n  operationId: getBulkAddTaskResultsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v2/accounts/{accountId}/devices/{deviceId}\n  method: delete\n  operationId: removeLineJWSPublic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/devices/bulk-add\n  method: post\n  operationId: bulkAddDevicesV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/send-activation-email\n  method: post\n  operationId: sendActivationEmailV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/batch-provisioning/users\n\
  \  method: post\n  operationId: postBatchProvisionUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/extensions\n  method: delete\n  operationId: bulkDeleteUsersV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v2/accounts/{accountId}/extensions/{extensionId}/devices/{deviceId}/replace\n  method: post\n  operationId: replaceDevicesJWSPublic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v1.0/account/{accountId}\n  method: get\n  operationId: readAccountInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/business-hours\n  method: get\n  operationId: readCompanyBusinessHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/business-hours\n  method: put\n  operationId: updateCompanyBusinessHours\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/device/{deviceId}\n  method: get\n  operationId: readDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/device/{deviceId}\n  method: put\n  operationId: updateDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/device/{deviceId}/sip-info\n  method: get\n  operationId: readDeviceSipInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/device/{deviceId}/emergency\n\
  \  method: put\n  operationId: updateDeviceEmergency\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/custom-fields\n  method: get\n  operationId: listCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/custom-fields\n  method: post\n  operationId: createCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /restapi/v1.0/account/{accountId}/custom-fields/{fieldId}\n  method: put\n  operationId: updateCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/custom-fields/{fieldId}\n  method: delete\n  operationId: deleteCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/call-recording\n  method: get\n  operationId: readCallRecordingSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/call-recording\n  method: put\n  operationId: updateCallRecordingSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/call-recording/custom-greetings\n  method: get\n  operationId: listCallRecordingCustomGreetings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/call-recording/custom-greetings\n  method: delete\n  operationId: deleteCallRecordingCustomGreetingList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/call-recording/custom-greetings/{greetingId}\n  method: delete\n  operationId: deleteCallRecordingCustomGreeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/call-recording/bulk-assign\n  method: post\n  operationId: updateCallRecordingExtensionList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /restapi/v1.0/account/{accountId}/call-recording/extensions\n  method: get\n  operationId: listCallRecordingExtensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/telephony/call-out\n  method: post\n  operationId: createCallOutCallSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/telephony/conference\n  method: post\n  operationId: createConferenceCallSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /restapi/v1.0/account/{accountId}/telephony/sessions/{telephonySessionId}\n  method: get\n  operationId: readCallSessionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapi/v1.0/account/{accountId}/telephony/sessions/{telephonySessionId}\n  method: delete\n  operationId: deleteCallSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: requ\n\n# --- truncated at 32 KB (155 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/agentic-access/ringcentral-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/agentic-access/ringcentral-agentic-access.yml
summary_line: 487 operations · 250 acting · 47 human-in-the-loop
tags:
- Communications
- UCaaS
- Voice
- Video
- Contact Center
- SMS
- Messaging
- Fax
---
