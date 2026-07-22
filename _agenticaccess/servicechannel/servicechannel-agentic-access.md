---
acting_count: 368
action_class_counts:
  acting: 368
  connected: 381
api_specs:
- filename: servicechannel-service-automation-openapi-original.json
  format: json
  label: ServiceChannel Service Automation API
  slug: servicechannel-service-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/openapi/servicechannel-service-automation-openapi-original.json
- filename: servicechannel-fixxbook-openapi-original.json
  format: json
  label: ServiceChannel Fixxbook API
  slug: servicechannel-fixxbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/openapi/servicechannel-fixxbook-openapi-original.json
consequence_counts:
  physical: 137
  read: 381
  safety-critical: 9
  write: 222
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 9
kind: agentic-access
layout: agentic-access
method: generated
name: Servicechannel Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/notifications/resetnotify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /checklists/{checkListResponseId}/CheckListResponse
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /doNotDispatch/addProvider/{providerId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /doNotDispatch/removeProvider/{providerId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /notifications/resetnotify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /providers/current/subscribers/{subscriberId}/servicerequest/overrides/props
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /providers/updateDispatchSetting
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscribers/current/servicerequest/overrides/props
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /users/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /AssetTypes/GetSubscriberAssetTypeCategories
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /GlCodes/CreateGlCode
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /GlCodes/DeleteGlCode
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /GlCodes/UpdateGlCode
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ScConnector/CheckInOut
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ScConnector/SubContractorWorkorderCreated
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ScConnector/SubContractorWorkorderUpdated
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ScConnector/UpdateConnectorWorkOrderStatusAfterReassign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ScConnector/WorkorderCreated
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ScConnector/WorkorderUpdated
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /SupplyClick/ProcessItems
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /aiagents/SendImage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /aiagents/SendMessage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/notifications/v2/workorders/ivr/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/notifications/v2/workorders/notes/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/notifications/v2/workorders/resend
operation_count: 749
overview: 'ServiceChannel exposes 749 API operations that an AI agent could call, of which 368 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 381 read, 222 write, 137 physical, and 9 safety-critical.


  9 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ServiceChannel
provider_slug: servicechannel
slug: servicechannel-agentic-access
source_filename: servicechannel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/servicechannel-fixxbook-openapi-original.json, openapi/servicechannel-service-automation-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 749\n  by_action_class:\n    connected: 381\n    acting: 368\n  by_consequence:\n    read: 381\n    safety-critical: 9\n    write: 222\n    physical: 137\n  human_in_the_loop_required: 9\noperations:\n- path: /Clients/GetProvidersInfo\n  method: get\n  operationId: Client_GetProvidersInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doNotDispatch/addProvider/{providerId}\n  method: post\n  operationId: DoNotDispatch_AddProvider\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /doNotDispatch/removeProvider/{providerId}\n  method: delete\n  operationId: DoNotDispatch_RemoveProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /doNotDispatch/getProviders\n  method: get\n  operationId: DoNotDispatch_GetProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitation\n\
  \  method: post\n  operationId: Invitation_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/ProviderData\n  method: put\n  operationId: Providers_ProviderData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/subscribers\n  method: get\n  operationId: Providers_Subscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}/businesshours\n  method: get\n  operationId:\
  \ GETv3_locations_{locationId}_businesshours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}/businesshours\n  method: post\n  operationId: POSTv3_locations_{locationId}_businesshours\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}/holidays\n  method: get\n  operationId: GETv3_locations_{locationId}_holidays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}/holidays\n  method: post\n  operationId: POSTv3_locations_{locationId}_holidays\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}/holidays\n  method: delete\n  operationId: DELETEv3_locations_{locationId}_holidays?holidayName={holidayName}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aiagents/locations/{locationId}/InitConversation\n  method: get\n  operationId: GETv3_aiagents_locations_{locationId}_InitConversation?setupId={setupId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aiagents/SendMessage\n\
  \  method: post\n  operationId: POSTv3_aiagents_SendMessage?threadId={threadId}&message={message}\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aiagents/SendImage\n  method: post\n  operationId: POSTv3_aiagents_SendImage?threadId={threadId}&setupId={setupId}\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aiagents/locations/{locationId}/ProcessMessageStream\n  method: get\n  operationId: GETv3_aiagents_locations_{locationId}_ProcessMessageStream?setupId={setupId}&threadId={threadId}&assistantId={assistantId}&enableMetrics={enableMetrics}\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aiagents/DeleteConversation\n  method: delete\n  operationId: DELETEv3_aiagents_DeleteConversation?threadId={threadId}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aiagents/CreateConversation\n  method: post\n  operationId: POSTv3_aiagents_CreateConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aiagents/ProblemDescription\n  method: get\n  operationId:\
  \ GETv3_aiagents_ProblemDescription?threadId={threadId}&assistantId={assistantId}&enableMetrics={enableMetrics}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aiagents/CreateFeedbackSession\n  method: post\n  operationId: POSTv3_aiagents_CreateFeedbackSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aiagents/AddFeedback\n  method: post\n  operationId: POSTv3_aiagents_AddFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /announcements\n  method: get\n  operationId: GETv3_announcements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /announcements/{messageId}\n  method: put\n  operationId: PUTv3_announcements_{messageId}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ApplicationAccess\n  method: get\n  operationId: GETv3_ApplicationAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetId}\n  method: get\n  operationId: GETv3_assets_{assetId}?locationId={locationId}&storeId={storeId}&tagId={tagId}&trackingNumber={trackingNumber}\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/AssociateAssetCode\n  method: post\n  operationId: POSTv3_assets_AssociateAssetCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/searchassets\n  method: post\n  operationId: POSTv3_assets_searchassets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/assetsforreplacement\n  method: post\n  operationId: POSTv3_assets_assetsforreplacement\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/assetcomponents\n  method: post\n  operationId: POSTv3_assets_assetcomponents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/getfilteredassets\n  method: post\n  operationId: POSTv3_assets_getfilteredassets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /assets/getfilteredassetsV1\n  method: post\n  operationId: POSTv3_assets_getfilteredassetsV1?providerId={providerId}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/getfilteredassetleaks\n  method: post\n  operationId: POSTv3_assets_getfilteredassetleaks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/getwoassettracking\n  method: post\n  operationId: POSTv3_assets_getwoassettracking?woId={woId}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/WoAssetTags\n  method: get\n  operationId: GETv3_assets_WoAssetTags?recIds[0]={recIds[0]}&recIds[1]={recIds[1]}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/locations/{locationId}\n  method: get\n  operationId: GETv3_assets_locations_{locationId}?trade={trade}&tradeId={tradeId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/locationAssetsTree\n  method: post\n  operationId: POSTv3_assets_locationAssetsTree?locationId={locationId}&trade={trade}\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/getassetwohistory\n  method: post\n  operationId: POSTv3_assets_getassetwohistory?workOrdersCount={workOrdersCount}\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets\n  method: put\n  operationId: PUTv3_assets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /assets\n  method: post\n  operationId: POSTv3_assets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/UpdateAssetTypeInAsset\n  method: put\n  operationId: PUTv3_assets_UpdateAssetTypeInAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/AddUpdateAsset\n  method: post\n  operationId: POSTv3_assets_AddUpdateAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/Activation\n  method: post\n  operationId: POSTv3_assets_Activation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/workorders/{workorderId}/attach\n  method: put\n  operationId: PUTv3_assets_workorders_{workorderId}_attach\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/workorders/attachassets\n  method: put\n  operationId: PUTv3_assets_workorders_attachassets\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/workorders/setupassets\n  method: put\n  operationId: PUTv3_assets_workorders_setupassets\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/workrequest/setup\n  method: put\n  operationId: PUTv3_assets_workrequest_setup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/workrequest/remove\n  method: post\n  operationId: POSTv3_assets_workrequest_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/workrequest/{workRequestId}\n  method: get\n  operationId: GETv3_assets_workrequest_{workRequestId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/workorders/removeassets\n  method: post\n  operationId: POSTv3_assets_workorders_removeassets\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/workorders/{workorderId}/detach\n  method: put\n  operationId: PUTv3_assets_workorders_{workorderId}_detach\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetid}/assetwohistory\n  method: get\n  operationId: GETv3_assets_{assetid}_assetwohistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetid}/assetTransferProvider\n  method:\
  \ get\n  operationId: GETv3_assets_{assetid}_assetTransferProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/TransferSettings/{subscriberId}\n  method: get\n  operationId: GETv3_assets_TransferSettings_{subscriberId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/Brands\n  method: get\n  operationId: GETv3_assets_Brands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/v2/Brands\n  method: get\n  operationId: GETv3_assets_v2_Brands?keyword={keyword}&startIndex={startIndex}&pageSize={pageSize}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /assets/v3/Brands\n  method: get\n  operationId: GETv3_assets_v3_Brands?assetTypeId={assetTypeId}&keyword={keyword}&startIndex={startIndex}&pageSize={pageSize}&assetTypeBrandsOnly={assetTypeBrandsOnly}&subscriberId={subscriberId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{brandName}/AddBrand\n  method: post\n  operationId: POSTv3_assets_{brandName}_AddBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/assetrepairstatus\n  method: get\n  operationId: GETv3_assets_assetrepairstatus?assetId={assetId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /assets/assetstatushistory\n  method: get\n  operationId: GETv3_assets_assetstatushistory?assetId={assetId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/updateassetrepairstatus\n  method: put\n  operationId: PUTv3_assets_updateassetrepairstatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/RecordScannedAsset\n  method: post\n  operationId: POSTv3_assets_RecordScannedAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /assets/HasAssetBeenValidated\n  method: post\n  operationId: POSTv3_assets_HasAssetBeenValidated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/GetAssetValidationInformation\n  method: post\n  operationId: POSTv3_assets_GetAssetValidationInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{subscriberId}/ValidationRules\n  method: get\n  operationId: GETv3_assets_{subscriberId}_ValidationRules\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/ValidationRulesByWOId\n  method: get\n  operationId: GETv3_assets_ValidationRulesByWOId?trackingNumber={trackingNumber}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/UnableToValidateReasons\n  method: get\n  operationId: GETv3_assets_UnableToValidateReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/UnableToValidateReasons\n  method: post\n  operationId: POSTv3_assets_UnableToValidateReasons\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /assets/UnableToScanReasons\n  method: get\n  operationId: GETv3_assets_UnableToScanReasons?subscriberId={subscriberId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/UnableToScanReasons\n  method: post\n  operationId: POSTv3_assets_UnableToScanReasons\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/UnableToAddReasons\n  method: get\n  operationId: GETv3_assets_UnableToAddReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/UnableToAddReasons\n  method: post\n  operationId: POSTv3_assets_UnableToAddReasons\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/UnableToScanReasonsNotAttachedAsset\n  method: get\n  operationId: GETv3_assets_UnableToScanReasonsNotAttachedAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/UnableToValidateReasonsNotAttachedAsset\n  method: get\n  operationId: GETv3_assets_UnableToValidateReasonsNotAttachedAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/ValidationRulesForMultipleSubscribers\n  method: post\n  operationId: POSTv3_assets_ValidationRulesForMultipleSubscribers\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/GetAssetValidationHistoryByTrackingNumber\n  method: post\n  operationId: POSTv3_assets_GetAssetValidationHistoryByTrackingNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/updateAssetLocation\n  method: put\n  operationId: PUTv3_assets_updateAssetLocation?assetId={assetId}&locationId={locationId}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{trackingNumber}/IsValidationRequired\n  method: get\n  operationId: GETv3_assets_{trackingNumber}_IsValidationRequired\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/getPrimaryAttachmentsForAssetList\n  method: post\n  operationId: POSTv3_assets_getPrimaryAttachmentsForAssetList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/getPrimaryAttachmentsForAssetList_v1\n  method: post\n  operationId: POSTv3_assets_getPrimaryAttachmentsForAssetList_v1\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{tradeId}/getAssetTypeGroupsByTradeId\n  method: get\n  operationId: GETv3_assets_{tradeId}_getAssetTypeGroupsByTradeId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/GetAssetTypeGroupsByAssetsIds\n  method: post\n  operationId: POSTv3_assets_GetAssetTypeGroupsByAssetsIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/searchassetsByGroupId\n  method: post\n  operationId:\
  \ POSTv3_assets_searchassetsByGroupId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/CanUserEditAsset\n  method: get\n  operationId: GETv3_assets_CanUserEditAsset?assetTypeId={assetTypeId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/CanCreateAsset/{assetTypeId}\n  method: get\n  operationId: GETv3_assets_CanCreateAsset_{assetTypeId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/CanProviderCreateAssetForTrade/{tradeId}\n  method: get\n  operationId: GETv3_assets_CanProviderCreateAssetForTrade_{tradeId}\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/AssetMeterReadings/{assetId}\n  method: get\n  operationId: GETv3_assets_AssetMeterReadings_{assetId}?lastMeterReadingValuesOnly={lastMeterReadingValuesOnly}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/AssetMeterReading\n  method: put\n  operationId: PUTv3_assets_AssetMeterReading\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/AssetMeterReading\n  method: post\n  operationId: POSTv3_assets_AssetMeterReading\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/CreateAssetMeterReadingsBulk\n  method: post\n  operationId: POSTv3_assets_CreateAssetMeterReadingsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/UpdateAssetMeterReadingsBulk\n  method: put\n  operationId: PUTv3_assets_UpdateAssetMeterReadingsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/AssetMeter\n\
  \  method: post\n  operationId: POSTv3_assets_AssetMeter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/AssetMeters\n  method: get\n  operationId: GETv3_assets_AssetMeters?assetMeterId={assetMeterId}&assetId={assetId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/Manufacturer\n  method: get\n  operationId: GETv3_assets_Manufacturer?manufacturerId={manufacturerId}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/WorkorderAreas/{subscriberId}\n  method: get\n  operationId: GETv3_assets_WorkorderAreas_{subscriberId}\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/GetValidationStatusesForMultipleWorkOrders\n  method: post\n  operationId: POSTv3_assets_GetValidationStatusesForMultipleWorkOrders?includeDeactivated={includeDeactivated}\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/updateAssetStatus\n  method: put\n  operationId: PUTv3_assets_updateAssetStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\n# --- truncated at 32 KB (252 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/agentic-access/servicechannel-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/agentic-access/servicechannel-agentic-access.yml
summary_line: 749 operations · 368 acting · 9 human-in-the-loop
tags:
- Company
- Services
- Facilities Management
- Work Orders
- Field Service
- Maintenance
- Asset Management
- Service Providers
- Invoicing
---
