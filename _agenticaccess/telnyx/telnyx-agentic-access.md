---
acting_count: 553
action_class_counts:
  acting: 553
  connected: 485
api_specs:
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Voice API
  slug: telnyx-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Messaging API
  slug: telnyx-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Numbers API
  slug: telnyx-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Verify API
  slug: telnyx-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Fax API
  slug: telnyx-fax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Wireless API
  slug: telnyx-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Networking API
  slug: telnyx-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx AI API
  slug: telnyx-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Billing & Reporting API
  slug: telnyx-billing-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
consequence_counts:
  physical: 89
  read: 485
  safety-critical: 61
  write: 403
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 61
kind: agentic-access
layout: agentic-access
method: generated
name: Telnyx Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /addresses/{id}/actions/accept_suggestions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ai/embeddings/buckets/{bucket_name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /call_control_applications
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /call_control_applications/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /call_control_applications/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/ai_assistant_add_messages
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/ai_assistant_join
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/ai_assistant_start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/ai_assistant_stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/answer
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/bridge
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /calls/{call_control_id}/actions/client_state_update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/enqueue
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/fork_start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/fork_stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/gather
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/gather_stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/gather_using_ai
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/gather_using_audio
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/gather_using_speak
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/hangup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/leave_queue
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/playback_start
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/playback_stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /calls/{call_control_id}/actions/record_pause
operation_count: 1038
overview: 'Telnyx exposes 1038 API operations that an AI agent could call, of which 553 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 485 read, 403 write, 89 physical, and 61 safety-critical.


  61 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Telnyx
provider_slug: telnyx
slug: telnyx-agentic-access
source_filename: telnyx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/telnyx-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1038\n  by_action_class:\n    connected: 485\n    acting: 553\n  by_consequence:\n    read: 485\n    write: 403\n    physical: 89\n    safety-critical: 61\n  human_in_the_loop_required: 61\noperations:\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: GetOAuthAuthorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: GetOAuthProtectedResourceMetadata\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/brand\n  method: get\n  operationId: GetBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/brand\n  method: post\n  operationId: CreateBrandPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/brand/feedback/{brandId}\n  method: get\n  operationId: GetBrandFeedbackById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/brand/smsOtp/{referenceId}\n  method: get\n  operationId: GetBrandSmsOtpStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/brand/{brandId}\n  method: delete\n  operationId: DeleteBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/brand/{brandId}\n  method: get\n  operationId: GetBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/brand/{brandId}\n  method: put\n  operationId: UpdateBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /10dlc/brand/{brandId}/2faEmail\n  method: post\n  operationId: ResendBrand2faEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/brand/{brandId}/externalVetting\n  method: get\n  operationId: ListExternalVettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/brand/{brandId}/externalVetting\n  method: post\n  operationId: PostOrderExternalVetting\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/brand/{brandId}/externalVetting\n  method: put\n  operationId: PutExternalVettingRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/brand/{brandId}/revet\n  method: put\n  operationId: RevetBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/brand/{brandId}/smsOtp\n  method: get\n  operationId: GetBrandSmsOtpStatusByBrandId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/brand/{brandId}/smsOtp\n  method: post\n  operationId: TriggerBrandSmsOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/brand/{brandId}/smsOtp\n  method: put\n  operationId: VerifyBrandSmsOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/campaign\n  method: get\n  operationId: GetCampaigns\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/campaign/acceptSharing/{campaignId}\n  method: post\n  operationId: AcceptCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/campaign/usecase/cost\n  method: get\n  operationId: GetCampaignCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/campaign/{campaignId}\n  method: delete\n  operationId: DeactivateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/campaign/{campaignId}\n  method: get\n  operationId: GetCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/campaign/{campaignId}\n  method: put\n  operationId: UpdateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/campaign/{campaignId}/appeal\n  method: post\n  operationId: AppealCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /10dlc/campaign/{campaignId}/mnoMetadata\n  method: get\n  operationId: GetCampaignMnoMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/campaign/{campaignId}/operationStatus\n  method: get\n  operationId: GetCampaignOperationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/campaign/{campaignId}/osr/attributes\n  method: get\n  operationId: GetCampaignOsrAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/campaign/{campaignId}/sharing\n  method: get\n  operationId: GetCampaignSharingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /10dlc/campaignBuilder\n  method: post\n  operationId: PostCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/campaignBuilder/brand/{brandId}/usecase/{usecase}\n  method: get\n  operationId: GetUsecaseQualification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/enum/{endpoint}\n  method: get\n  operationId: GetEnumEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/partnerCampaign/sharedByMe\n  method: get\n  operationId: GetPartnerCampaignsSharedByUser\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/partnerCampaign/{campaignId}/sharing\n  method: get\n  operationId: GetPartnerCampaignSharingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/partner_campaigns\n  method: get\n  operationId: GetSharedCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/partner_campaigns/{campaignId}\n  method: get\n  operationId: GetSharedCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/partner_campaigns/{campaignId}\n  method: patch\n  operationId: UpdateSharedCampaign\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/phoneNumberAssignmentByProfile\n  method: post\n  operationId: PostAssignMessagingProfileToCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/phoneNumberAssignmentByProfile/{taskId}\n  method: get\n  operationId: GetAssignmentTaskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/phoneNumberAssignmentByProfile/{taskId}/phoneNumbers\n  method: get\n  operationId: GetPhoneNumberStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/phone_number_campaigns\n  method: get\n  operationId: GetAllPhoneNumberCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/phone_number_campaigns\n  method: post\n  operationId: CreatePhoneNumberCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/phone_number_campaigns/{phoneNumber}\n  method: delete\n  operationId: DeletePhoneNumberCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /10dlc/phone_number_campaigns/{phoneNumber}\n  method: get\n  operationId: GetSinglePhoneNumberCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /10dlc/phone_number_campaigns/{phoneNumber}\n  method: put\n  operationId: PutPhoneNumberCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access_ip_address\n  method: get\n  operationId: ListAccessIpAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /access_ip_address\n  method: post\n  operationId: CreateAccessIpAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access_ip_address/{access_ip_address_id}\n  method: delete\n  operationId: DeleteAccessIpAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access_ip_address/{access_ip_address_id}\n  method: get\n  operationId: GetAccessIpAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /access_ip_ranges\n  method: get\n  operationId: ListAccessIpRanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access_ip_ranges\n  method: post\n  operationId: CreateAccessIPRange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access_ip_ranges/{access_ip_range_id}\n  method: delete\n  operationId: DeleteAccessIpRange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/purchase/esims\n\
  \  method: post\n  operationId: PurchaseESim\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/register/sim_cards\n  method: post\n  operationId: RegisterSimCards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses\n  method: get\n  operationId: FindAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses\n  method: post\n  operationId:\
  \ CreateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/actions/validate\n  method: post\n  operationId: ValidateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{id}\n  method: delete\n  operationId: DeleteAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /addresses/{id}\n  method: get\n  operationId: GetAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{id}/actions/accept_suggestions\n  method: post\n  operationId: acceptAddressSuggestions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /advanced_orders\n  method: get\n  operationId: list_advanced_orders_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advanced_orders\n  method: post\n  operationId: create_advanced_order_v2\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /advanced_orders/{advanced-order-id}/requirement_group\n  method: patch\n  operationId: update_advanced_order_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /advanced_orders/{order_id}\n  method: get\n  operationId: get_advanced_order_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants\n  method: get\n\
  \  operationId: get_assistants_public_assistants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants\n  method: post\n  operationId: create_new_assistant_public_assistants_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/import\n  method: post\n  operationId: import_assistants_public_assistants_import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/tags\n  method:\
  \ get\n  operationId: get_all_assistant_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/tests\n  method: get\n  operationId: get_assistant_tests_public_assistants_tests_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/tests\n  method: post\n  operationId: create_assistant_test_public_assistants_tests_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/tests/test-suites\n  method: get\n  operationId: fetch_test_suites_public_assistants_tests_test_suites_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/tests/test-suites/{suite_name}/runs\n  method: get\n  operationId: get_test_suite_runs_for_test_public_assistants_tests_test_suites__suite_name__runs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/tests/test-suites/{suite_name}/runs\n  method: post\n  operationId: trigger_test_suite_runs_public_assistants_tests_test_suites__suite_name__runs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/tests/{test_id}\n  method: delete\n  operationId: delete_assistant_test_public_assistants_tests__test_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/tests/{test_id}\n  method: get\n  operationId: get_assistant_test_public_assistants_tests__test_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/tests/{test_id}\n  method: put\n  operationId: update_assistant_test_public_assistants_tests__test_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/tests/{test_id}/runs\n\
  \  method: get\n  operationId: get_test_runs_for_test_public_assistants_tests__test_id__runs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/tests/{test_id}/runs\n  method: post\n  operationId: trigger_test_run_public_assistants_tests__test_id__runs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/tests/{test_id}/runs/{run_id}\n  method: get\n  operationId: get_test_run_public_assistants_tests__test_id__runs__run_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/{assistant_id}\n  method:\
  \ delete\n  operationId: delete_assistant_public_assistants__assistant_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}\n  method: get\n  operationId: get_assistant_public_assistants__assistant_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/{assistant_id}\n  method: post\n  operationId: update_assistant_public_assistants__assistant_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /ai/assistants/{assistant_id}/canary-deploys\n  method: delete\n  operationId: delete_canary_deploy_assistants__assistant_id__canary_deploys_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/canary-deploys\n  method: get\n  operationId: get_canary_deploy_assistants__assistant_id__canary_deploys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/{assistant_id}/canary-deploys\n  method: post\n  operationId: create_canary_deploy_assistants__assistant_id__canary_deploys_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/canary-deploys\n  method: put\n  operationId: update_canary_deploy_assistants__assistant_id__canary_deploys_put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/chat\n  method: post\n  operationId: assistant_chat_public_assistants__assistant_id__chat_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/chat/sms\n  method: post\n  operationId: assistant_sms_chat_assistants__assistant_id__chat_sms_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/clone\n  method: post\n  operationId: clone_assistant_public_assistants__assistant_id__clone_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /ai/assistants/{assistant_id}/scheduled_events\n  method: get\n  operationId: get_scheduled_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/{assistant_id}/scheduled_events\n  method: post\n  operationId: create_scheduled_event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/scheduled_events/{event_id}\n  method: delete\n  operationId: delete_scheduled_event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/scheduled_events/{event_id}\n  method: get\n  operationId: get_scheduled_event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/{assistant_id}/tags\n  method: post\n  operationId: add_assistant_tag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/tags/{tag}\n  method: delete\n  operationId: remove_assistant_tag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/texml\n  method: get\n  operationId: get_assistant_texml_public_assistants__assistant_id__texml_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/{assistant_id}/tools/{tool_id}\n  method: delete\n  operationId: remove_assistant_tool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/tools/{tool_id}\n  method: put\n  operationId: add_assistant_tool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/tools/{tool_id}/test\n  method: post\n  operationId: test_assistant_tool_public_assistants__assistant_id__tools__tool_id__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/versions\n  method: get\n  operationId: get_assistant_versions_public_assistants__assistant_id__versions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/{assistant_id}/versions/{version_id}\n  method: delete\n  operationId: delete_assistant_version_public_assistants__assistant_id__versions__version_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/assistants/{assistant_id}/versions/{version_id}\n  method: get\n  operationId: get_assistant_version_public_assistants__assistant_id__versions__version_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/assistants/{assistant_id}/versions/{version_id}\n  method: post\n  operationId: update_assistant_version_public_assistants__assistant_id__versions__version_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-val\n\n# --- truncated at 32 KB (313 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/agentic-access/telnyx-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/agentic-access/telnyx-agentic-access.yml
summary_line: 1038 operations · 553 acting · 61 human-in-the-loop
tags:
- Communications
- CPaaS
- Voice
- SMS
- IoT
---
