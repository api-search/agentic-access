---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 24
api_specs:
- filename: osis-co-ai-api-openapi.yml
  format: yaml
  label: osis-co AI API
  slug: osis-co-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-ai-api-openapi.yml
- filename: osis-co-calls-api-openapi.yml
  format: yaml
  label: osis-co Calls API
  slug: osis-co-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-calls-api-openapi.yml
- filename: osis-co-capabilities-api-openapi.yml
  format: yaml
  label: osis-co Capabilities API
  slug: osis-co-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-capabilities-api-openapi.yml
- filename: osis-co-conversations-api-openapi.yml
  format: yaml
  label: osis-co Conversations API
  slug: osis-co-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-conversations-api-openapi.yml
- filename: osis-co-events-api-openapi.yml
  format: yaml
  label: osis-co Events API
  slug: osis-co-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-events-api-openapi.yml
- filename: osis-co-groups-api-openapi.yml
  format: yaml
  label: osis-co Groups API
  slug: osis-co-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-groups-api-openapi.yml
- filename: osis-co-lines-api-openapi.yml
  format: yaml
  label: osis-co Lines API
  slug: osis-co-lines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-lines-api-openapi.yml
- filename: osis-co-messages-api-openapi.yml
  format: yaml
  label: osis-co Messages API
  slug: osis-co-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-messages-api-openapi.yml
- filename: osis-co-number-changes-api-openapi.yml
  format: yaml
  label: osis-co Number Changes API
  slug: osis-co-number-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-number-changes-api-openapi.yml
- filename: osis-co-payments-api-openapi.yml
  format: yaml
  label: osis-co Payments API
  slug: osis-co-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-payments-api-openapi.yml
- filename: osis-co-webhooks-api-openapi.yml
  format: yaml
  label: osis-co Webhooks API
  slug: osis-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-webhooks-api-openapi.yml
consequence_counts:
  physical: 12
  read: 24
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Osis Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /calls/{id}/dtmf
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contact-cards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/{message_id}/unsend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payments/branding
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/merchant/terms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payments/shopify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payments/whop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payments/whop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /polls
operation_count: 55
overview: 'osis-co exposes 55 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 19 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: osis-co
provider_slug: osis-co
slug: osis-co-agentic-access
source_filename: osis-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/osis-co-ai-api-openapi.yml, openapi/osis-co-calls-api-openapi.yml, openapi/osis-co-capabilities-api-openapi.yml,\n  openapi/osis-co-conversations-api-openapi.yml, openapi/osis-co-events-api-openapi.yml, openapi/osis-co-groups-api-openapi.yml,\n  openapi/osis-co-lines-api-openapi.yml, openapi/osis-co-messages-api-openapi.yml, openapi/osis-co-number-changes-api-openapi.yml,\n  openapi/osis-co-payments-api-openapi.yml, openapi/osis-co-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    connected: 24\n    acting: 31\n  by_consequence:\n    read: 24\n    write: 19\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /ai/usage\n\
  \  method: get\n  operationId: getAiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/models\n  method: get\n  operationId: listAiModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lines/{e164}/call-forwarding\n  method: get\n  operationId: getCallForwarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lines/{e164}/call-forwarding\n  method: put\n  operationId: putCallForwarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /calls\n  method: get\n  operationId: listCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls\n  method: post\n  operationId: placeCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{id}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{id}/answer\n  method: post\n  operationId: answerCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{id}/decline\n  method: post\n  operationId: declineCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{id}/hangup\n  method: post\n  operationId: hangupCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{id}/say\n  method: post\n  operationId: sayOnCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{id}/dtmf\n  method: post\n  operationId: sendCallDtmf\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{id}/turns\n  method: get\n  operationId: listCallTurns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{id}/media\n  method: get\n  operationId: getCallMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{id}/voicemail\n\
  \  method: get\n  operationId: downloadCallVoicemail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities\n  method: post\n  operationId: checkMessagingCapabilities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations\n  method: get\n  operationId: listConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/typing\n  method: post\n  operationId: setConversationTyping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/read\n  method: post\n  operationId: markConversationRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/backdrop\n  method: post\n  operationId: setConversationBackdrop\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: listDeliveryEvents\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: post\n  operationId: createGroupChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lines\n  method: get\n  operationId: listAvailableDedicatedLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lines/claim\n  method: post\n  operationId: claimDedicatedLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /lines/{e164}/lock\n  method: post\n  operationId: lockDedicatedLine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lines/{e164}/lock\n  method: delete\n  operationId: cancelLinePortSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lines/{e164}/port\n  method: get\n  operationId: getLinePort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lines/{e164}/port\n\
  \  method: post\n  operationId: startLinePort\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lines/{id}/location\n  method: get\n  operationId: getSharedLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lines/{e164}/number-changes\n  method: post\n  operationId: startNumberChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{message_id}/reactions\n  method: post\n  operationId: reactToMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{id}/attachments/{index}\n  method: get\n  operationId: downloadMessageAttachment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /polls\n  method: post\n  operationId: sendPoll\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact-cards\n  method: get\n  operationId: getContactCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact-cards\n  method: post\n  operationId: sendContactCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact-cards\n  method: put\n  operationId: setContactCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{message_id}/unsend\n  method: post\n  operationId: unsendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /number-changes/{id}\n  method: get\n  operationId: getNumberChange\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: post\n  operationId: createPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: get\n  operationId: listPaymentRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/shopify/catalog\n  method: get\n  operationId: getShopifyCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/shopify\n  method: delete\n\
  \  operationId: disconnectShopify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{id}\n  method: get\n  operationId: getPaymentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{id}\n  method: delete\n  operationId: cancelPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /payments/branding\n  method: get\n  operationId: getPaymentsBranding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/branding\n  method: put\n  operationId: putPaymentsBranding\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/merchant\n  method: get\n  operationId: getMerchantStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/merchant/terms\n  method: post\n  operationId: acceptMerchantTerms\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/whop\n  method: get\n  operationId: getPaymentsWhop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/whop\n  method: put\n  operationId: putPaymentsWhop\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/whop\n  method: delete\n  operationId: deletePaymentsWhop\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/osis-co/agentic-access/osis-co-agentic-access.yml
summary_line: 55 operations · 31 acting
tags:
- Messaging
- Communications
- Software-as-a-Service
- Customer Service
---
