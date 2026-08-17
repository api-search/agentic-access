---
acting_count: 233
action_class_counts:
  acting: 233
  connected: 289
api_specs:
- filename: dotdigital-v2-api-full-openapi.yml
  format: yaml
  label: Dotdigital v2 API
  slug: dotdigital-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/openapi/dotdigital-v2-api-full-openapi.yml
- filename: dotdigital-contacts-openapi.yml
  format: yaml
  label: Dotdigital v3 API
  slug: dotdigital-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/openapi/dotdigital-contacts-openapi.yml
- filename: dotdigital-omnichannel-openapi.yml
  format: yaml
  label: Dotdigital CPaaS API
  slug: dotdigital-cpaas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/openapi/dotdigital-omnichannel-openapi.yml
consequence_counts:
  physical: 25
  read: 289
  safety-critical: 2
  write: 206
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Dotdigital Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cpaas/chats/{chatId}/typing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cpaas/conversations/{conversationId}/typing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cpaas/chats/{chatId}/form
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cpaas/chats/{chatId}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cpaas/conversations/{conversationId}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cpaas/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cpaas/messages/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /cpaas/profiles/{id}/rels/link/{linkedId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /cpaas/profiles/{id}/rels/link/{linkedId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /cpaas/profiles/{id}/rels/primary/{linkedId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /cpaas/profiles/{id}/rels/primary/{linkedId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /marketing-email/v3/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /marketing-email/v3/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/campaigns/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/campaigns/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/campaigns/send-time-optimised
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/campaigns/send-time-optimised
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/email/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/email/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/email/triggered-campaign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/email/triggered-campaign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/email/triggered-campaign/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/email/triggered-campaign/batch
operation_count: 522
overview: 'Dotdigital exposes 522 API operations that an AI agent could call, of which 233 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 289 read, 206 write, 25 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dotdigital
provider_slug: dotdigital
slug: dotdigital-agentic-access
source_filename: dotdigital-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/dotdigital-accounts-and-utilities-openapi.yml, openapi/dotdigital-analytics-openapi.yml,\n  openapi/dotdigital-campaign-templates-openapi.yml, openapi/dotdigital-chat-config-openapi.yml,\n  openapi/dotdigital-chat-message-openapi.yml, openapi/dotdigital-chat-openapi.yml, openapi/dotdigital-chat-presence-openapi.yml,\n  openapi/dotdigital-configuration-service-openapi.yml, openapi/dotdigital-contact-data-fields-openapi.yml,\n  openapi/dotdigital-contacts-openapi.yml, openapi/dotdigital-content-openapi.yml, openapi/dotdigital-conversation-message-openapi.yml,\n  openapi/dotdigital-conversation-openapi.yml, openapi/dotdigital-cpaas-openapi.yml, openapi/dotdigital-data-firehose-openapi.yml,\n  openapi/dotdigital-documents-openapi.yml, openapi/dotdigital-ecommerce-openapi.yml, openapi/dotdigital-email-campaigns-openapi.yml,\n  openapi/dotdigital-email-contacts-openapi.yml, openapi/dotdigital-events-openapi.yml, openapi/dotdigital-images-openapi.yml,\n\
  \  openapi/dotdigital-insight-and-transactional-data-openapi.yml, openapi/dotdigital-insight-data-service-openapi.yml,\n  openapi/dotdigital-lists-address-books-openapi.yml, openapi/dotdigital-marketing-email-openapi.yml,\n  openapi/dotdigital-message-history-openapi.yml, openapi/dotdigital-message-rules-openapi.yml,\n  openapi/dotdigital-omnichannel-openapi.yml, openapi/dotdigital-pages-and-forms-openapi.yml,\n  openapi/dotdigital-phone-number-validation-openapi.yml, openapi/dotdigital-preferences-and-subscriptions-openapi.yml,\n  openapi/dotdigital-product-recommendations-openapi.yml, openapi/dotdigital-profile-openapi.yml,\n  openapi/dotdigital-programs-openapi.yml, openapi/dotdigital-scoring-openapi.yml, openapi/dotdigital-segments-openapi.yml,\n  openapi/dotdigital-session-openapi.yml, openapi/dotdigital-sms-campaigns-openapi.yml, openapi/dotdigital-templates-openapi.yml,\n  openapi/dotdigital-transactional-email-openapi.yml, openapi/dotdigital-v2-api-full-openapi.yml,\n  openapi/dotdigital-webhook-openapi.yml,\
  \ openapi/dotdigital-whatsapp-channel-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 522\n  by_action_class:\n    connected: 289\n    acting: 233\n  by_consequence:\n    read: 289\n    write: 206\n    physical: 25\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v2/account-info\n  method: get\n  operationId: get-account-information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/server-time\n  method: get\n  operationId: get-server-time\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/empty-recycle-bin/\n\
  \  method: post\n  operationId: empty-recycle-bin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/analytics/conversationmessages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/chats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/chats/live\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/messages\n  method: get\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/messages/metrics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/sessions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/sms/tracking\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/sms/verify\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/sms/inbound\n  method: get\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/sms/outbound\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/whatsapp/conversations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/analytics/whatsapp/dailymessagingusage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/templates\n  method: post\n  operationId: create-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/templates\n  method: get\n  operationId: get-templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/templates/{id}\n  method: get\n  operationId: get-template-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/templates/{id}\n  method: put\n  operationId: update-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chat/config\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/chat/config/teams/{teamId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/chat/config/teams/{teamId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chat/config/teams/{teamId}/appMessaging\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chat/config/teams/{teamId}/appMessaging\n\
  \  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chat/config/teams/{teamId}/settings\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chat/config/teams/{teamId}/settings\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}/events\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/chats/{chatId}/messages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/chats/{chatId}/messages\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}/messages/statusupdates\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/chats/{chatId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}/assign\n  method: put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}/close\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}/channel\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}/form\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/chats\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}/typing\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/chats/{chatId}/typing\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cpaas/chats/{chatId}/participants\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/presence\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/presence/appmessaging\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v3/customIdentifiers\n  method: get\n  operationId: getCustomIdentifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/v3/customIdentifiers\n  method: post\n  operationId: createCustomIdentifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /configuration/v3/customIdentifiers/{name}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/data-fields\n  method: post\n  operationId: create-contact-data-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/data-fields\n  method: get\n  operationId: get-contact-data-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/data-fields/{name}\n  method: delete\n  operationId: delete-contact-data-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /contacts/v3\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/v3\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/v3/delete\n  method: post\n  operationId: deleteContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/v3/delete/{deleteId}\n  method: get\n  operationId: getDeleteStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/v3/import\n  method: put\n  operationId: importContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/v3/import/{importId}\n  method: get\n  operationId: getImportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/v3/{identifier}/{value}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/v3/{identifier}/{value}\n  method: put\n\
  \  operationId: replaceContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/v3/{identifier}/{value}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/v3/{identifier}/{value}\n  method: patch\n  operationId: importContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /cpaas/content\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/content/{fileId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/content/{fileId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/conversations/{conversationId}/events\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/conversations/{conversationId}/messages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/conversations/{conversationId}/messages\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/conversations/{conversationId}/messages/statusupdates\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/conversations/{conversationId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/conversations/{conversationId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/conversations/{conversationId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/conversations\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/conversations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/conversations/{conversationId}/typing\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/conversations/{conversationId}/typing\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cpaas/conversations/{conversationId}/participants\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cpaas/conversations/{conversationId}/participants\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cpaas/conversations/{conversationId}/participants\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/dedicatedNumbers\n  method: get\n  operationId: get-sms-phone-number\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/shortcodes\n  method: get\n  operationId: get-sms-shortcodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/keywords\n  method: get\n  operationId: get-sms-keywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/facebook/state\n  method: post\n  operationId: facebook-meta-data-service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-firehose/v3/configurations/{id}\n  method: get\n  operationId: getConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-firehose/v3/configurations/{id}\n  method: put\n  operationId: updateConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-firehose/v3/configurations/{id}\n  method: delete\n  operationId: deleteConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-firehose/v3/configurations/{id}/status/{newStatus}\n  method: put\n  operationId: updateStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-firehose/v3/configurations\n  method: post\n  operationId: addConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/document-folders/{id}\n  method: post\n  operationId: create-document-folder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/document-folders\n  method: get\n  operationId: get-document-folders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/document-folders/{id}/documents\n  method: get\n  operationId: get-documents-in-folder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/document-folders/{id}/documents\n  method: post\n  operationId: upload-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ecommerce/orders\n  method: get\n  operationId: get-orders-since-date\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns\n  method: post\n  operationId: create-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns\n  method: get\n  operationId: get-all-campaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/split-test\n  method: post\n  operationId: create-split-test-campaign\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns/{id}\n  method: put\n  operationId: update-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns/{id}\n  method: delete\n  operationId: delete-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns/{id}\n\
  \  method: get\n  operationId: get-campaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{id}/copy\n  method: post\n  operationId: copy-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns/send\n  method: post\n  operationId: send-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns/send-time-optimised\n  method:\
  \ post\n  operationId: send-time-optimised-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns/send/{id}\n  method: get\n  operationId: get-campaign-send-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{campaignID}/attachments\n  method: post\n  operationId: add-campaign-attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/campaigns/{campaignID}/attachments\n  method: get\n  operationId: get-campaign-attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{campaignID}/attachments/{documentID}\n  method: delete\n  operationId: remove-campaign-attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns/filtered\n  method: get\n  operationId: get-all-campaigns-with-filters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{id}/with-details\n  method: get\n  operationId: get-campaign-with-details\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{id}/summary\n  method: get\n  operationId: get-campaign-summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{id}/opens\n  method: get\n  operationId: get-campaign-opens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{campaignID}/activities/{contactID}/opens\n  method: get\n  operationId: get-campaign-opens-for-a-contact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{campaignID}/activities/{contactID}\n  method: get\n  operationId: get-campaign-activity-for\n\n# --- truncated at\
  \ 32 KB (151 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/agentic-access/dotdigital-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotdigital/refs/heads/main/agentic-access/dotdigital-agentic-access.yml
summary_line: 522 operations · 233 acting · 2 human-in-the-loop
tags:
- Marketing Automation
- Email Marketing
- SMS
- MMS
- WhatsApp
- Contacts
- Campaigns
- Push Notifications
- Transactional Email
- Engagement
- Automation
- CPaaS
- Omnichannel
- Customer Data
- Consent Management
- Personalization
- Loyalty
- Ecommerce
- Events
- Webhooks
---
