---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 21
api_specs:
- filename: bird-faq-api-openapi.yml
  format: yaml
  label: Bird FAQ API
  slug: bird-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-faq-api-openapi.yml
- filename: bird-intent-api-openapi.yml
  format: yaml
  label: Bird Intent API
  slug: bird-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-intent-api-openapi.yml
- filename: bird-sms-messaging-api-openapi.yml
  format: yaml
  label: Bird SMS Messaging API
  slug: bird-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-sms-messaging-api-openapi.yml
- filename: bird-channels-api-openapi.yml
  format: yaml
  label: Bird Channels API
  slug: bird-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-channels-api-openapi.yml
- filename: bird-contacts-api-openapi.yml
  format: yaml
  label: Bird Contacts API
  slug: bird-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-contacts-api-openapi.yml
- filename: bird-conversations-api-openapi.yml
  format: yaml
  label: Bird Conversations API
  slug: bird-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-conversations-api-openapi.yml
- filename: bird-legacy-messagebird-api-openapi.yml
  format: yaml
  label: Bird Legacy MessageBird API
  slug: bird-legacy-messagebird-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-legacy-messagebird-api-openapi.yml
- filename: bird-messaging-api-openapi.yml
  format: yaml
  label: Bird Messaging API
  slug: bird-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-messaging-api-openapi.yml
- filename: bird-numbers-api-openapi.yml
  format: yaml
  label: Bird Numbers API
  slug: bird-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-numbers-api-openapi.yml
- filename: bird-language-detection-api-openapi.yml
  format: yaml
  label: Bird Language Detection API
  slug: bird-language-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-language-detection-api-openapi.yml
- filename: bird-named-entity-recognition-api-openapi.yml
  format: yaml
  label: Bird Named Entity Recognition API
  slug: bird-named-entity-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-named-entity-recognition-api-openapi.yml
consequence_counts:
  physical: 5
  read: 21
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bird Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/channels/{channelId}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{workspaceId}/conversations/{conversationId}/messages
operation_count: 37
overview: 'Bird exposes 37 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 11 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bird
provider_slug: bird
slug: bird-agentic-access
source_filename: bird-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/bird-channels-api-openapi.yml, openapi/bird-contacts-api-openapi.yml, openapi/bird-conversations-api-openapi.yml,\n  openapi/bird-faq-api-openapi.yml, openapi/bird-intent-api-openapi.yml, openapi/bird-language-detection-api-openapi.yml,\n  openapi/bird-legacy-messagebird-api-openapi.yml, openapi/bird-messaging-api-openapi.yml, openapi/bird-named-entity-recognition-api-openapi.yml,\n  openapi/bird-numbers-api-openapi.yml, openapi/bird-sms-messaging-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    acting: 16\n    connected: 21\n  by_consequence:\n    write: 11\n    read: 21\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path:\
  \ /workspaces/{workspaceId}/channel-media/presigned-upload\n  method: post\n  operationId: createPresignedUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/channels\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/channels/{channelId}\n  method: get\n  operationId: getChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/contacts/{contactId}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/contacts/{contactId}\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/contacts/{contactId}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/conversations\n  method: post\n  operationId: createConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/conversations/{conversationId}/messages\n  method: post\n  operationId: createConversationMessage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/conversations/{conversationId}/messages/{messageId}\n  method: get\n  operationId: getConversationMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets\n  method: get\n  operationId: FAQ_ListDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{datasetId}\n  method: get\n  operationId: FAQ_GetDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{datasetId}/predict-answer\n  method: post\n  operationId: FAQ_PredictAnswer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/supported-languages\n  method: get\n  operationId: FAQ_ListSupportedLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets\n  method: get\n  operationId: Intent_ListDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{datasetId}\n  method: get\n  operationId: Intent_GetDataset\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/{datasetId}/predict\n  method: post\n  operationId: Intent_PredictIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/supported-languages\n  method: get\n  operationId: Intent_ListSupportedLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/predict-language\n  method: post\n  operationId: LanguageDetection_PredictLanguage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/supported-languages\n  method: get\n  operationId: LanguageDetection_ListSupportedLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages\n  method: post\n  operationId: legacyCreateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  operationId: legacyListMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{id}\n\
  \  method: get\n  operationId: legacyGetMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/{phoneNumber}\n  method: get\n  operationId: legacyLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify\n  method: post\n  operationId: legacyCreateVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voicemessages\n  method: get\n  operationId: legacyListVoiceMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/channels/{channelId}/messages\n  method: post\n  operationId: sendChannelMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/channels/{channelId}/messages\n  method: get\n  operationId: listChannelMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/predict-entities\n  method: post\n  operationId: NamedEntityRecognition_PredictEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/supported-languages\n  method: get\n  operationId: NamedEntityRecognition_ListSupportedLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/numbers\n  method: get\n  operationId: listNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/network-lookup\n  method: post\n  operationId: numberLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /messages\n  method: post\n  operationId: postMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{messageId}\n  method: get\n  operationId: getMessagesByMessageId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{messageId}\n  method: delete\n  operationId: deleteMessagesByMessageId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/agentic-access/bird-agentic-access.yml
summary_line: 37 operations · 16 acting
tags:
- Communications
- SMS
- Email
- WhatsApp
- Voice
- Messaging
- Omnichannel
- Customer Engagement
---
