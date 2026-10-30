---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 19
api_specs:
- filename: thanks-io-creatives-library-api-openapi.yml
  format: yaml
  label: Thanks.io Creatives Library API
  slug: thanks-io-creatives-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-creatives-library-api-openapi.yml
- filename: thanks-io-dynamic-images-api-openapi.yml
  format: yaml
  label: Thanks.io Dynamic Images API
  slug: thanks-io-dynamic-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-dynamic-images-api-openapi.yml
- filename: thanks-io-giftcards-api-openapi.yml
  format: yaml
  label: Thanks.io Giftcards API
  slug: thanks-io-giftcards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-giftcards-api-openapi.yml
- filename: thanks-io-handwriting-styles-api-openapi.yml
  format: yaml
  label: Thanks.io Handwriting Styles API
  slug: thanks-io-handwriting-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-handwriting-styles-api-openapi.yml
- filename: thanks-io-image-templates-api-openapi.yml
  format: yaml
  label: Thanks.io Image Templates API
  slug: thanks-io-image-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-image-templates-api-openapi.yml
- filename: thanks-io-mailing-lists-api-openapi.yml
  format: yaml
  label: Thanks.io Mailing Lists API
  slug: thanks-io-mailing-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-mailing-lists-api-openapi.yml
- filename: thanks-io-message-templates-api-openapi.yml
  format: yaml
  label: Thanks.io Message Templates API
  slug: thanks-io-message-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-message-templates-api-openapi.yml
- filename: thanks-io-order-estimates-api-openapi.yml
  format: yaml
  label: Thanks.io Order Estimates API
  slug: thanks-io-order-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-order-estimates-api-openapi.yml
- filename: thanks-io-orders-api-openapi.yml
  format: yaml
  label: Thanks.io Orders API
  slug: thanks-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-orders-api-openapi.yml
- filename: thanks-io-recipients-api-openapi.yml
  format: yaml
  label: Thanks.io Recipients API
  slug: thanks-io-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-recipients-api-openapi.yml
- filename: thanks-io-send-mailer-api-openapi.yml
  format: yaml
  label: Thanks.io Send Mailer API
  slug: thanks-io-send-mailer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-send-mailer-api-openapi.yml
- filename: thanks-io-webhook-events-api-openapi.yml
  format: yaml
  label: Thanks.io Webhook Events API
  slug: thanks-io-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-webhook-events-api-openapi.yml
- filename: thanks-io-webhooks-api-openapi.yml
  format: yaml
  label: Thanks.io Webhooks API
  slug: thanks-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-webhooks-api-openapi.yml
- filename: thanks-io-subaccounts-api-openapi.yml
  format: yaml
  label: Thanks.io Subaccounts API
  slug: thanks-io-subaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-subaccounts-api-openapi.yml
consequence_counts:
  physical: 16
  read: 19
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thanks Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimate/giftcard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimate/magnacard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimate/notecard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimate/postcard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimate/windowedletter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimate/windowlessletter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /order-items/{orderItemId}/invalidate-giftcard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/{orderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderId}/replay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/giftcard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/magnacard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/notecard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/postcard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/windowedletter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/windowlessletter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /sub-accounts/{subAccountId}
operation_count: 52
overview: 'Thanks.io exposes 52 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 17 write, and 16 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Thanks.io
provider_slug: thanks-io
slug: thanks-io-agentic-access
source_filename: thanks-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/thanks-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 19\n    acting: 33\n  by_consequence:\n    read: 19\n    write: 17\n    physical: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /recipients/{recipientId}\n  method: get\n  operationId: getRecipientsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipients/{recipientId}\n  method: put\n  operationId: updateRecipientDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients/{recipientId}\n  method: delete\n  operationId: deleteRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients\n  method: post\n  operationId: createRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients-utils/create-multiple\n  method: post\n  operationId: createMultipleRecipients\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients-utils/delete-by-address\n  method: post\n  operationId: deleteRecipientByAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailing-lists/\n  method: get\n  operationId: getMailingLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailing-lists/\n  method: post\n  operationId: createMailingList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailing-lists/{mailingListId}\n  method: get\n  operationId: getMailingListDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailing-lists/{mailingListId}\n  method: delete\n  operationId: deleteMailingList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailing-lists-utils/recipients/{mailingListId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /mailing-lists-utils/buy-radius-search\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailing-lists-utils/count-radius-search\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send/postcard\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /send/magnacard\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send/windowedletter\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send/windowlessletter\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send/notecard\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send/giftcard\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimate/postcard\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimate/windowedletter\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimate/windowlessletter\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimate/notecard\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimate/magnacard\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimate/giftcard\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /build/image-template\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /handwriting-styles\n  method: get\n  operationId: listHandwritingStyles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /giftcard-brands\n  method: get\n  operationId: listGiftcardBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /giftcard-brands-list\n  method: get\n  operationId: listGiftcardBrandsAsList\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sub-accounts/\n  method: get\n  operationId: getSubAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sub-accounts/\n  method: post\n  operationId: createSubAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sub-accounts/{subAccountId}\n  method: get\n  operationId: getSubAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sub-accounts/{subAccountId}\n  method: put\n  operationId: updateSubAccount\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sub-accounts/{subAccountId}\n  method: delete\n  operationId: deleteSubAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image-templates/\n  method: get\n  operationId: getImageTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creatives/\n  method: get\n  operationId: getCreatives\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creatives/{creativeId}\n  method: get\n  operationId: getCreative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /message-templates/\n  method: get\n  operationId: getMessageTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /message-templates/\n  method: post\n  operationId: createMessageTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /message-templates/{messageTemplateId}\n  method: get\n  operationId: getMessageTemplate\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /message-templates/{messageTemplateId}\n  method: patch\n  operationId: updateMessageTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /message-templates/{messageTemplateId}\n  method: delete\n  operationId: deleteMessageTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/list\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/track\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/items\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderId}/cancel\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}/replay\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order-items/{orderItemId}/invalidate-giftcard\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/thanks-io/agentic-access/thanks-io-agentic-access.yml
summary_line: 52 operations · 33 acting
tags:
- Company
- AI
- DirectMail
- Automation
- API
---
