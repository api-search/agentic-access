---
acting_count: 400
action_class_counts:
  acting: 400
  connected: 343
api_specs:
- filename: extole-integration-consumer-to-extole-openapi.json
  format: json
  label: Extole Integration API - Consumer to Extole
  slug: extole-integration-api-consumer-to-extole
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-integration-consumer-to-extole-openapi.json
- filename: extole-integration-server-to-extole-openapi.json
  format: json
  label: Extole Integration API - Server to Extole
  slug: extole-integration-api-server-to-extole
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-integration-server-to-extole-openapi.json
- filename: extole-management-openapi.json
  format: json
  label: Extole Management API
  slug: extole-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-management-openapi.json
- filename: extole-management-expert-openapi.json
  format: json
  label: Extole Management Expert API
  slug: extole-management-expert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-management-expert-openapi.json
consequence_counts:
  physical: 11
  read: 343
  safety-critical: 151
  write: 238
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 151
kind: agentic-access
layout: agentic-access
method: generated
name: Extole Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/component-grants/{grantId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/approves
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/approves/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/approves/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/cancel-rewards
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/cancel-rewards/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/cancel-rewards/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/create-memberships
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/create-memberships/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/create-memberships/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/creatives
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/creatives/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/creatives/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/creatives/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/data-intelligences
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/data-intelligences/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/data-intelligences/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/declines
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/declines/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/declines/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/displays
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/displays/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/displays/{actionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/campaigns/{campaignId}{version}/controllers/{controllerId}/actions/earn-rewards
operation_count: 743
overview: 'Extole exposes 743 API operations that an AI agent could call, of which 400 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 343 read, 238 write, 11 physical, and 151 safety-critical.


  151 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Extole
provider_slug: extole
slug: extole-agentic-access
source_filename: extole-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/extole-integration-consumer-to-extole-openapi.json, openapi/extole-integration-server-to-extole-openapi.json,\n  openapi/extole-management-expert-openapi.json, openapi/extole-management-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 743\n  by_action_class:\n    connected: 343\n    acting: 400\n  by_consequence:\n    read: 343\n    write: 238\n    physical: 11\n    safety-critical: 151\n  human_in_the_loop_required: 151\noperations:\n- path: /api/v4/events/share/status/{pollingId}\n  method: get\n  operationId: shareEventStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v4/me\n  method: get\n  operationId: getMyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me\n  method: post\n  operationId: updateMyProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/me/advocates\n  method: get\n  operationId: getAdvocateRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v4/me/assets\n  method: post\n  operationId: createAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/me/assets/download\n  method: get\n  operationId: downloadAssetByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/assets/{assetId}\n  method: get\n  operationId: readAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/assets/{assetId}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/me/assets/{assetId}/download\n  method: get\n  operationId: downloadAssetById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/audience-memberships\n  method: get\n  operationId: getAudienceMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/email/status/{polling_id}\n  method: get\n  operationId: getSendEmailStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/friends\n  method: get\n  operationId: getFriends\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/journeys\n  method: get\n  operationId: getJourneys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/parameters\n  method: get\n  operationId: getPersonProfileParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/parameters\n  method: post\n  operationId: editPersonProfileParameters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/me/referrals-from-me\n  method: get\n  operationId: getReferralsFromMe\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/referrals-to-me\n  method: get\n  operationId: getReferralsToMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/rewards/status\n  method: get\n  operationId: getMyRewardStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/send-verification-email/status/{pollingId}\n  method: get\n  operationId: verificationEmailStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/shareables\n  method: get\n  operationId: getMeShareables\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/shareables\n  method: post\n  operationId: createMeShareableV4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/me/shareables/status/{polling_id}\n  method: get\n  operationId: getMeShareableStatusV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/shareables/{shareable_id}\n  method: get\n  operationId: getMeShareable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/shareables/{shareable_id}\n  method:\
  \ put\n  operationId: edit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/me/shares\n  method: get\n  operationId: getShares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/shares/{shareId}\n  method: get\n  operationId: getShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/me/steps\n  method: get\n  operationId: getSteps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/person/profile-picture-url/{personId}\n\
  \  method: get\n  operationId: getPersonProfilePictureUrlV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/person/{personId}\n  method: get\n  operationId: getPublicPersonV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/persons/{personId}/assets\n  method: get\n  operationId: listPersonAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/persons/{personId}/assets/download\n  method: get\n  operationId: downloadPersonAssetByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/persons/{personId}/assets/{assetId}\n  method: get\n  operationId:\
  \ getPersonAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/persons/{personId}/assets/{assetId}/download\n  method: get\n  operationId: downloadPersonAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/shareable\n  method: get\n  operationId: getShareablesV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/shareable\n  method: post\n  operationId: createShareable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v4/shareable/status/{polling_id}\n  method: get\n  operationId: getStatus_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/shareable/{shareable_id}\n  method: get\n  operationId: getShareableV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/shares\n  method: get\n  operationId: getPublicShares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/shares/{share_id}\n  method: get\n  operationId: getPublicShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v5/custom/share/status/{pollingId}\n  method: get\n  operationId: customShareStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v5/token\n  method: get\n  operationId: getConsumerToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v5/token\n  method: post\n  operationId: createConsumerToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v5/token\n  method: delete\n  operationId: deleteConsumerToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v6/me/shareables\n  method: get\n  operationId: getShareables_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v6/me/shareables\n  method: post\n  operationId: createMeShareable_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v6/me/shareables/{code}\n  method: get\n  operationId: getShareable_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_name}\n  method: get\n  operationId: fetchConsumerEventByName\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/events/share\n  method: post\n  operationId: shareEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/me/email\n  method: post\n  operationId: sendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/me/send-verification-email\n  method: post\n  operationId: sendVerificationEmail\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v5/custom/share\n  method: post\n  operationId: customShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v5/email/share/batch\n  method: post\n  operationId: batchEmailShare\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/v6/me/shareables/get-create-or-update\n  method: post\n  operationId: getCreateOrUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v6/me/shareables/get-or-create\n  method: post\n  operationId: getOrCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v6/zones\n  method: post\n  operationId: renderZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v6/zones/{event_name}\n  method: post\n  operationId: renderZoneByEventName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zones\n  method: post\n  operationId: renderZoneWeb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zones/{zone_name}\n  method: post\n  operationId: renderZoneByNameWeb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/me/parameters/{parameter_name}\n  method: put\n  operationId: putPersonProfileParameter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/rewards\n  method: get\n  operationId: listRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/rewards/state_summary\n  method: get\n  operationId: getRewardStateSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/rewards/{reward_id}\n  method: get\n  operationId: getReward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/rewards/{reward_id}\n  method: put\n  operationId: updateReward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/rewards/{reward_id}/cancels\n  method: get\n  operationId: getRewardCancels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/rewards/{reward_id}/fails\n  method: get\n  operationId: getRewardFails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/rewards/{reward_id}/fulfillments\n  method: get\n  operationId: getRewardFulfillments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/rewards/{reward_id}/history\n  method: get\n  operationId: getRewardStateHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/rewards/{reward_id}/redeems\n  method: get\n  operationId: getRewardRedeems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/rewards/{reward_id}/revokes\n  method: get\n  operationId: getRewardRevokes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/rewards/{reward_id}/sends\n  method: get\n  operationId: getRewardSends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/tokens\n  method: get\n  operationId: getCurrentClientAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/tokens\n  method: post\n  operationId: createClientAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/tokens/{token}\n  method: get\n  operationId: getClientAccessTokenByValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/tokens/{token}\n  method: delete\n  operationId: deleteClientAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons\n  method: get\n  operationId: searchPersons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons\n  method: post\n  operationId: createPerson_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons/partner-keys\n\
  \  method: get\n  operationId: getPartnerKeys_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}\n  method: get\n  operationId: getPerson_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}\n  method: put\n  operationId: updatePerson_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons/{person_id}/block\n  method: get\n  operationId: getPersonBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v5/persons/{person_id}/block\n  method: put\n  operationId: updatePersonBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons/{person_id}/data\n  method: get\n  operationId: listPersonData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/data\n  method: post\n  operationId: createPersonData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons/{person_id}/data/{name}\n\
  \  method: get\n  operationId: getPersonData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/data/{name}\n  method: put\n  operationId: updatePersonData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons/{person_id}/data/{name}\n  method: delete\n  operationId: deletePersonData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons/{person_id}/identity-history\n  method: get\n\
  \  operationId: getIdentityHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/journeys\n  method: get\n  operationId: listPersonJourneys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/journeys/{journey_id}\n  method: get\n  operationId: getPersonJourney\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/locations\n  method: get\n  operationId: listPersonLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/memberships\n  method: get\n  operationId: listPersonMemberships\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/memberships\n  method: post\n  operationId: createPersonMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons/{person_id}/relationships\n  method: get\n  operationId: listPersonRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/rewards\n  method: get\n  operationId: listPersonRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/rewards/{reward_id}\n  method: get\n  operationId: getPersonReward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/shareables\n  method: get\n  operationId: listPersonShareables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/shareables\n  method: post\n  operationId: createPersonShareable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons/{person_id}/shareables/{code}\n  method: get\n  operationId:\
  \ getPersonShareable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/shareables/{code}\n  method: put\n  operationId: updatePersonShareable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/persons/{person_id}/shares\n  method: get\n  operationId: listPersonShares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/persons/{person_id}/shares/{share_id}\n  method: get\n  operationId: getPersonShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v5/persons/{person_id}/steps\n  method: get\n  operationId: listPersonSteps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/zones/{zone_name}\n  method: get\n  operationId: fetchZone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/zones/{zone_name}\n  method: post\n  operationId: renderZoneV5\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v6/batches\n  method: get\n  operationId: listBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v6/batches\n  method: post\n  operationId: createBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v6/batches/{batchId}\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v6/batches/{batchId}\n  method: put\n  operationId: updateBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v6/batches/{batchId}\n  method: delete\n \
  \ operationId: deleteBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v6/files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v6/files\n  method: post\n  operationId: createFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v6/files/{fileId}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v6/files/{fileId}\n  method: put\n  operationId: updateFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v6/files/{fileId}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v6/files/{fileId}/download\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v6/sftp-destinations\n\
  \  method: get\n  operationId: listSftpDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v6/sftp-destinations\n  method: post\n  operationId: createSftpDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v6/sftp-destinations/{sftpDestinationId}\n  method: get\n  operationId: getSftpDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v6/sftp-destinations/{sftpDestinationId}\n  method: put\n  operationId: updateSftpDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high\n\n# --- truncated at 32 KB (236 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/agentic-access/extole-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/agentic-access/extole-agentic-access.yml
summary_line: 743 operations · 400 acting · 151 human-in-the-loop
tags:
- Company
- Referral Marketing
- Advocacy
- Loyalty
- Rewards
- Marketing
- Customer Acquisition
- SaaS
---
