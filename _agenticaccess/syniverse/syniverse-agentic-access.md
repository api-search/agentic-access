---
acting_count: 117
action_class_counts:
  acting: 117
  connected: 70
api_specs:
- filename: syniverse-omni-channel-messaging-openapi.yml
  format: yaml
  label: Syniverse Omni-Channel Messaging API (SCG)
  slug: syniverse-omni-channel-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-omni-channel-messaging-openapi.yml
- filename: syniverse-multi-factor-authentication-openapi.yml
  format: yaml
  label: Syniverse Multi-Factor Authentication API
  slug: syniverse-multi-factor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-multi-factor-authentication-openapi.yml
- filename: syniverse-phone-number-verification-openapi.yml
  format: yaml
  label: Syniverse Phone Number Verification API
  slug: syniverse-phone-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-phone-number-verification-openapi.yml
- filename: syniverse-right-party-verification-openapi.yml
  format: yaml
  label: Syniverse Right Party Verification API
  slug: syniverse-right-party-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-right-party-verification-openapi.yml
- filename: syniverse-account-takeover-detection-openapi.yml
  format: yaml
  label: Syniverse Account Takeover Detection API
  slug: syniverse-account-takeover-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-account-takeover-detection-openapi.yml
- filename: syniverse-messaging-trust-resolve-openapi.yml
  format: yaml
  label: Syniverse Messaging Trust Resolve API
  slug: syniverse-messaging-trust-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-messaging-trust-resolve-openapi.yml
- filename: syniverse-messaging-trust-datafeed-openapi.yml
  format: yaml
  label: Syniverse Messaging Trust Spam Datafeed API
  slug: syniverse-messaging-trust-spam-datafeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-messaging-trust-datafeed-openapi.yml
- filename: syniverse-10dlc-openapi.yml
  format: yaml
  label: Syniverse 10DLC API
  slug: syniverse-10dlc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-10dlc-openapi.yml
- filename: syniverse-10dlc-number-pool-openapi.yml
  format: yaml
  label: Syniverse 10DLC Number Pool API (v1, deprecated)
  slug: syniverse-10dlc-number-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-10dlc-number-pool-openapi.yml
- filename: syniverse-whitelisting-service-openapi.json
  format: json
  label: Syniverse Whitelisting Service API
  slug: syniverse-whitelisting-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-whitelisting-service-openapi.json
- filename: syniverse-token-management-openapi.yml
  format: yaml
  label: Syniverse SDC Application Access Token Management API
  slug: syniverse-access-token-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-token-management-openapi.yml
consequence_counts:
  physical: 15
  read: 70
  write: 102
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Syniverse Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /'applications/{Application_ID}/users/{User_ID}/associate'
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /'applications/{Application_ID}/users/{User_ID}/login_start'
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /'messaging/channels/{Channel_ID}/sender_ids'
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /'messaging/channels/{channel_ID}/sender_ids/{sender_ID}'
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /'messaging/sender_ids/purchase'
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /'messaging/sender_ids/{Sender_ID}'
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /'messaging/sender_ids/{Sender_ID}'
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /'sender_ids_import/{import_ID}'
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /'sender_ids_import/{import_ID}'
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /engage/tendlc-services/v2/campaigns/{campaignId}/suspend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/message_requests/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/sender_ids
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /messaging/sender_ids
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sender_ids_import
operation_count: 187
overview: 'Syniverse exposes 187 API operations that an AI agent could call, of which 117 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 70 read, 102 write, and 15 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Syniverse
provider_slug: syniverse
slug: syniverse-agentic-access
source_filename: syniverse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/syniverse-10dlc-number-pool-openapi.yml, openapi/syniverse-10dlc-openapi.yml,\n  openapi/syniverse-account-takeover-detection-openapi.yml, openapi/syniverse-messaging-trust-datafeed-openapi.yml,\n  openapi/syniverse-messaging-trust-resolve-openapi.yml, openapi/syniverse-multi-factor-authentication-openapi.yml,\n  openapi/syniverse-omni-channel-messaging-openapi.yml, openapi/syniverse-phone-number-verification-openapi.yml,\n  openapi/syniverse-right-party-verification-openapi.yml, openapi/syniverse-token-management-openapi.yml,\n  openapi/syniverse-whitelisting-service-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 187\n  by_action_class:\n    acting: 117\n    connected:\
  \ 70\n  by_consequence:\n    write: 102\n    read: 70\n    physical: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /engage/tendlc-services/v1/campaigns/{campaignId}/longcodes/{longcode}\n  method: post\n  operationId: create10DLCNumberUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v1/campaigns/{campaignId}/longcodes/{longcode}\n  method: delete\n  operationId: delete10DLCNumberUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v1/campaigns/{campaignId}/pools/{numberPoolId}/types/{numberPoolType}\n\
  \  method: post\n  operationId: campaignWithNumberPoolAssociationUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v1/campaigns/{campaignId}/pools/{numberPoolId}\n  method: delete\n  operationId: campaignWithNumberPoolRemovalUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v2/campaigns\n  method: get\n  operationId: getCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /engage/tendlc-services/v2/campaigns/{campaignId}/pools/{numberPoolId}/types/{numberPoolType}\n  method: post\n  operationId: campaignWithNumberPoolAssociationV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v2/campaigns/{campaignId}/longcodes/{longcode}\n  method: get\n  operationId: getApplicationAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /engage/tendlc-services/v2/campaigns/{campaignId}/longcodes/{longcode}\n  method: post\n  operationId: create10DLCNumberV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v2/campaigns/{campaignId}/longcodes/{longcode}\n  method: delete\n  operationId: delete10DLCNumberV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v2/campaigns/{campaignId}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /engage/tendlc-services/v2/campaigns/{campaignId}/suspend\n  method: post\n  operationId: suspendCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v2/campaigns/{campaignId}/resume\n  method: post\n  operationId: resumeCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v2/campaigns/{campaignId}/pools/{numberPoolId}\n  method: delete\n  operationId: campaignWithNumberPoolRemovalV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /engage/tendlc-services/v2/campaigns/att/{campaignId}\n  method: get\n  operationId: getCampaign_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /engage/tendlc-services/v2/att/application-address/{applicationAddress}\n  method: get\n  operationId: getApplicationAddress_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/simCheck\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spam/report\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mms/resolve\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/txt/resolve\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'applications/{Application_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'applications/{Application_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{Application_ID}/users\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'applications/{Application_ID}/users/{User_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'applications/{Application_ID}/users/{User_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'applications/{Application_ID}/users/{User_ID}/associate'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'applications/{Application_ID}/users/{User_ID}/associate'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'applications/{Application_ID}/users/{User_ID}/validate'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'applications/{Application_ID}/users/{User_ID}/login_start'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/sender_ids\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/sender_ids\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/sender_ids\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/sender_ids/purchase'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/sender_ids/{Sender_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/sender_ids/{Sender_ID}'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/sender_ids/{Sender_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/sender_ids/list\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/channels\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/channels\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/channels/{Channel_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/channels/{Channel_ID}'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/channels/{Channel_ID}'\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/channels/{Channel_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/channels/{Channel_ID}/sender_ids'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/channels/{Channel_ID}/sender_ids'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/channels/{channel_ID}/sender_ids/{sender_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/message_requests/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/message_requests/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/message_requests/{MessageRequest_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/message_requests/{MessageRequest_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/message_requests/{MessageRequest_ID}/messages'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/message_requests/scheduled/{MessageRequest_Scheduled_ID}'\n\
  \  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/messages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/messages\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/messages/{Message_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/messages/{Message_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/messages/{Message_ID}/attachments'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/messages/scheduled/{Message_Scheduled_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/attachments\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/attachments\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/attachments/{Attachment_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/attachments/{Attachment_ID}'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /'messaging/attachments/{Attachment_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/attachments/{Attachment_ID}/access_tokens'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/attachments/{Attachment_ID}/content'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/attachments/{Attachment_ID}/content'\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/message_templates\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/message_templates\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/message_templates/{Template_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /'messaging/message_templates/{Template_ID}'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/message_templates/{Template_ID}'\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/message_templates/{Template_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/keywords\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/keywords\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/keywords/{Keyword_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'messaging/keywords/{Keyword_ID}'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/keywords/{Keyword_ID}'\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'messaging/keywords/{Keyword_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calling/calls\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /calling/calls\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/calls/{Call_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'calling/calls/{Call_ID}'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/calls/{Call_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/calls/{call_id}/play_dtmf'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/calls/{call_id}/play_tts'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/calls/{call_id}/play_audio'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calling/bridges\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calling/bridges\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/bridges/{Bridge_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'calling/bridges/{Bridge_ID}'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/bridges/{Bridge_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/bridges/{Bridge_ID}/calls'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calling/conferences\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calling/conferences\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/conferences/{Conference_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'calling/conferences/{Conference_ID}'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/conferences/{Conference_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/conferences/{Conference_ID}/play_tts'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/conferences/{Conference_ID}/play_audio'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calling/conferences/{Conference_ID}/members\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calling/conferences/{Conference_ID}/members\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/conferences/{Conference_ID}/members/{Member_ID}'\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /'calling/conferences/{Conference_ID}/members/{Member_ID}'\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /'calling/conferences/{Conference_ID}/members/{Member_ID}'\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calling/calls/{Call_ID}/digits_collector\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calling/calls/{Call_ID}/digits_collector\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /'calling/calls/{Call_ID}/digits_collector/{Collector_ID}'\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subje\n\n# --- truncated at 32 KB (54 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/agentic-access/syniverse-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/agentic-access/syniverse-agentic-access.yml
summary_line: 187 operations · 117 acting
tags:
- Telecommunications
- United States
- CPaaS
- Messaging
- SMS
- Roaming
- IPX
- Wholesale
- Identity Verification
- SIM Swap
- 10DLC
- Open Gateway
- Network APIs
- Aggregator
---
