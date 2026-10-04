---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 26
api_specs:
- filename: kudosity-account-api-openapi.yml
  format: yaml
  label: Kudosity Account API
  slug: kudosity-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-account-api-openapi.yml
- filename: kudosity-contacts-lists-api-openapi.yml
  format: yaml
  label: Kudosity Contacts & Lists API
  slug: kudosity-contacts-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-contacts-lists-api-openapi.yml
- filename: kudosity-email-sms-api-openapi.yml
  format: yaml
  label: Kudosity Email SMS API
  slug: kudosity-email-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-email-sms-api-openapi.yml
- filename: kudosity-keywords-api-openapi.yml
  format: yaml
  label: Kudosity Keywords API
  slug: kudosity-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-keywords-api-openapi.yml
- filename: kudosity-mms-api-openapi.yml
  format: yaml
  label: Kudosity MMS API
  slug: kudosity-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-mms-api-openapi.yml
- filename: kudosity-numbers-api-openapi.yml
  format: yaml
  label: Kudosity Numbers API
  slug: kudosity-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-numbers-api-openapi.yml
- filename: kudosity-rcs-api-openapi.yml
  format: yaml
  label: Kudosity RCS API
  slug: kudosity-rcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-rcs-api-openapi.yml
- filename: kudosity-reporting-api-openapi.yml
  format: yaml
  label: Kudosity Reporting API
  slug: kudosity-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-reporting-api-openapi.yml
- filename: kudosity-senders-api-openapi.yml
  format: yaml
  label: Kudosity Senders API
  slug: kudosity-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-senders-api-openapi.yml
- filename: kudosity-sms-api-openapi.yml
  format: yaml
  label: Kudosity SMS API
  slug: kudosity-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-sms-api-openapi.yml
- filename: kudosity-webhook-api-openapi.yml
  format: yaml
  label: Kudosity Webhook API
  slug: kudosity-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-webhook-api-openapi.yml
- filename: kudosity-whats-app-api-openapi.yml
  format: yaml
  label: Kudosity Whats App API
  slug: kudosity-whats-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-whats-app-api-openapi.yml
consequence_counts:
  physical: 9
  read: 26
  safety-critical: 1
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Kudosity Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /optout-list-member.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send-sms.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/mms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/rcs/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/senders/phone-numbers/{phone_number}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/senders/registrations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/senders/registrations/{registration_id}/verifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/senders/registrations/{registration_id}/verifications/confirmation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/whatsapp/messages
operation_count: 57
overview: 'Kudosity exposes 57 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 21 write, 9 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kudosity
provider_slug: kudosity
slug: kudosity-agentic-access
source_filename: kudosity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/kudosity-account-api-openapi.yml, openapi/kudosity-contacts-lists-api-openapi.yml,\n  openapi/kudosity-email-sms-api-openapi.yml, openapi/kudosity-keywords-api-openapi.yml, openapi/kudosity-mms-api-openapi.yml,\n  openapi/kudosity-numbers-api-openapi.yml, openapi/kudosity-rcs-api-openapi.yml, openapi/kudosity-reporting-api-openapi.yml,\n  openapi/kudosity-senders-api-openapi.yml, openapi/kudosity-sms-api-openapi.yml, openapi/kudosity-webhook-api-openapi.yml,\n  openapi/kudosity-whats-app-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 26\n    acting: 31\n  by_consequence:\n    read: 26\n    write: 21\n    safety-critical: 1\n  \
  \  physical: 9\n  human_in_the_loop_required: 1\noperations:\n- path: /get-balance.json\n  method: get\n  operationId: getGetBalanceJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add-contacts-bulk.json\n  method: post\n  operationId: postAddContactsBulkJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /add-list.json\n  method: post\n  operationId: postAddListJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /add-field-to-list.json\n  method: post\n  operationId: postAddFieldToListJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /remove-list.json\n  method: post\n  operationId: postRemoveListJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /add-to-list.json\n  method: post\n  operationId: postAddToListJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit-list-member.json\n  method: post\n  operationId: postEditListMemberJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-from-list.json\n  method: post\n  operationId: postDeleteFromListJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /optout-list-member.json\n  method: post\n  operationId: postOptoutListMemberJson\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /add-contacts-bulk-progress.json\n  method: post\n  operationId: postAddContactsBulkProgressJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /add-email.json\n  method: post\n  operationId: postAddEmailJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-email.json\n  method: post\n  operationId:\
  \ postDeleteEmailJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /add-keyword.json\n  method: post\n  operationId: postAddKeywordJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit-keyword.json\n  method: post\n  operationId: postEditKeywordJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /get-keywords.json\n  method: post\n  operationId: postGetKeywordsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/mms\n  method: post\n  operationId: postV2Mms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/mms/{id}\n  method: get\n  operationId: getV2MmsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lease-number.json\n  method: post\n  operationId: postLeaseNumberJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-numbers.json\n  method: get\n  operationId: getGetNumbersJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-number.json\n  method: post\n  operationId: postGetNumberJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit-number-options.json\n  method: post\n  operationId: postEditNumberOptionsJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/rcs/messages\n  method: get\n  operationId: getV2RcsMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/rcs/messages\n  method: post\n  operationId: postV2RcsMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/rcs/capabilities\n  method: post\n  operationId: postV2RcsCapabilities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/rcs/messages/{id}\n\
  \  method: get\n  operationId: getV2RcsMessagesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-sms.json\n  method: post\n  operationId: postGetSmsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-sms-delivery-status.json\n  method: post\n  operationId: postGetSmsDeliveryStatusJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-sms-sent-count.json\n  method: post\n  operationId: postGetSmsSentCountJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-user-sms-sent.json\n  method: post\n  operationId: postGetUserSmsSentJson\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-contact-sms-stats.json\n  method: get\n  operationId: getGetContactSmsStatsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-sms-stats.json\n  method: post\n  operationId: postGetSmsStatsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-sms-sent.json\n  method: post\n  operationId: postGetSmsSentJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-message-report.json\n  method: post\n  operationId: postGetMessageReportJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-list.json\n  method: post\n  operationId: postGetListJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-lists.json\n  method: get\n  operationId: getGetListsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-contact.json\n  method: post\n  operationId: postGetContactJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/senders/registrations\n  method: get\n  operationId: getV2SendersRegistrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/senders/registrations\n  method: post\n\
  \  operationId: postV2SendersRegistrations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/senders/phone-numbers/{phone_number}\n  method: delete\n  operationId: deleteV2SendersPhoneNumbersByPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/senders/registrations/{registration_id}/verifications\n  method: post\n  operationId: postV2SendersRegistrationsByRegistrationIdVerifications\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/senders/registrations/{registration_id}/verifications/confirmation\n  method: post\n  operationId: postV2SendersRegistrationsByRegistrationIdVerificationsConfirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sms/{id}\n  method: get\n  operationId: getV2SmsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v2/sms\n  method: get\n  operationId: getV2Sms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sms\n  method: post\n  operationId: postV2Sms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send-sms.json\n  method: post\n  operationId: postSendSmsJson\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /cancel-sms.json\n  method: post\n  operationId: postCancelSmsJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /format-number.json\n  method: post\n  operationId: postFormatNumberJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-sms-responses.json\n  method: post\n  operationId: postGetSmsResponsesJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-user-sms-responses.json\n  method: get\n  operationId: getGetUserSmsResponsesJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook\n  method: post\n  operationId: postV2Webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook\n  method: get\n  operationId: getV2Webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook/{id}\n  method: get\n  operationId: getV2WebhookById\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook/{id}\n  method: put\n  operationId: putV2WebhookById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook/{id}\n  method: delete\n  operationId: deleteV2WebhookById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/whatsapp/messages\n  method: get\n  operationId: getV2WhatsappMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/whatsapp/messages\n  method: post\n  operationId: postV2WhatsappMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/whatsapp/messages/{id}\n  method: get\n  operationId: getV2WhatsappMessagesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/agentic-access/kudosity-agentic-access.yml
summary_line: 57 operations · 31 acting · 1 human-in-the-loop
tags:
- Messaging
- SMS
- MMS
- RCS
- WhatsApp
- Communications
- CPaaS
- Webhook
- MCP
- Agent-Native
- Australia
- Notification
- Two-Way Messaging
- Contact Management
---
