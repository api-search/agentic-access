---
acting_count: 79
action_class_counts:
  acting: 79
  connected: 54
api_specs:
- filename: stax-api-openapi.json
  format: json
  label: Stax API
  slug: stax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stax/refs/heads/main/openapi/stax-api-openapi.json
consequence_counts:
  physical: 29
  read: 54
  safety-critical: 2
  write: 48
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Stax Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /forgot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reset/{token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /credit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice/schedule/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /invoice/schedule/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoice/schedule/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /invoice/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoice/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice/{id}/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice/{id}/pay/{method}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoice/{id}/send/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoice/{id}/send/sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-method
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-method/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payment-method/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payment-method/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment_method/{payment_method_id}/external_vault
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /query/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /query/payment-links/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /query/payment-links/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /query/payment-links/{id}/update-stats
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /self/verify/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /terminal/charge
operation_count: 133
overview: 'Stax exposes 133 API operations that an AI agent could call, of which 79 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 54 read, 48 write, 29 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Stax
provider_slug: stax
slug: stax-agentic-access
source_filename: stax-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: generated\nsource: openapi/stax-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 133\n  by_action_class:\n    connected: 54\n    acting: 79\n  by_consequence:\n    read: 54\n    write: 48\n    physical: 29\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /query/statement/v3/ach-rejects\n  method: get\n  operationId: ach-rejections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file\n  method: post\n  operationId: post_file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file\n  method: get\n  operationId: get_file\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/{id}/registration/file\n  method: post\n  operationId: add-file-to-merchant-registration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/options\n  method: put\n  operationId: addupdate-team-settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/option/advanced_customizations\n  method: put\n  operationId: post_teamoptionadvanced_customizations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{transactionid}/capture\n  method: post\n  operationId: capture-a-pre-auth-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/statement/v3/volumes/card-processing\n  method: get\n  operationId: card-processing\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charge\n  method: post\n  operationId: charge-a-payment-method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terminal/charge/queue\n  method: post\n  operationId: charge-queue\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terminal/charge\n  method: post\n  operationId: charge\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /self/exists\n  method: get\n  operationId: check-if-e-mail-exists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant\n  method: post\n  operationId: create-a-merchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant\n  method: get\n  operationId: get-all-merchants\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/{id}/apikey\n  method: post\n  operationId: create-a-new-api-key-for-merchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{id}/apikey\n  method: get\n  operationId: list-api-keys-for-merchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/user\n  method: post\n  operationId: create-a-new-team-member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /team/user\n  method: get\n  operationId: find-the-merchant-teams-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/payment-links\n  method: post\n  operationId: create-a-payment-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/payment-links\n  method: get\n  operationId: list-and-filter-all-payment-links\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-method\n  method: post\n  operationId: create-a-payment-method-copy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-method\n  method: get\n  operationId: get-all-payment-methods-for-a-merchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-method/\n  method: post\n  operationId: create-a-payment-method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice/schedule/\n\
  \  method: post\n  operationId: createScheduledInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team\n  method: post\n  operationId: create-a-team\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team\n  method: put\n  operationId: edit-your-merchant-teams-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /self\n  method: post\n  operationId: create-a-user-account-self-registration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /self\n  method: get\n  operationId: get-self-and-teams-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /self\n  method: put\n  operationId: update-your-user-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /invoice\n  method: post\n  operationId: create-an-invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice\n  method: get\n  operationId: get-all-invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /item\n  method: post\n  operationId: create-catalog-item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /item\n  method: get\n  operationId:\
  \ retrieve-all-catalog-items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer\n  method: post\n  operationId: create-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer\n  method: get\n  operationId: find-all-customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: post\n  operationId: create-new-webhook-for-all-of-my-users-merchants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook\n  method: get\n  operationId: get-all-webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhookadmin/webhook/brand\n  method: post\n  operationId: create-partner-level-webhook-for-your-brand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhookadmin/webhook/brand\n  method: get\n  operationId: get-all-partner-level-webhooks-for-your-brand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit\n  method:\
  \ post\n  operationId: credit-a-payment-method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terminal/credit\n  method: post\n  operationId: credit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/statement/v3/daily-sales\n  method: get\n  operationId: daily-sales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /item/{id}/decrement\n  method: put\n  operationId:\
  \ decrement-items-stock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /item/{id}\n  method: delete\n  operationId: delete-a-catalog-item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /item/{id}\n  method: get\n  operationId: retrieve-an-item-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /item/{id}\n  method: put\n  operationId: update-an-item\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/{id}\n  method: delete\n  operationId: delete-a-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/{id}\n  method: get\n  operationId: get-a-customers-information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/{id}\n  method: put\n  operationId: update-customer-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file{id}\n  method: delete\n  operationId: delete_file{id}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhookadmin/webhook/brand/{webhook_id}\n  method: delete\n  operationId: delete-a-partner-level-webhook-for-your-brand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhookadmin/webhook/brand/{webhook_id}\n  method: get\n  operationId: get-a-specific-partner-level-webhook-for-your-brand\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/payment-links/{id}\n  method: delete\n  operationId: delete-a-payment-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/payment-links/{id}\n  method: get\n  operationId: get-a-payment-links-information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/payment-links/{id}\n  method: put\n  operationId: update-a-payment-link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-method/{id}\n  method: delete\n  operationId: delete-a-payment-method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-method/{id}\n  method: get\n  operationId: get-a-payment-method-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-method/{id}\n  method: put\n  operationId: update-a-payment-method\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice/{id}\n  method: delete\n  operationId: delete-an-invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice/{id}\n  method: get\n  operationId: get-an-invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice/{id}\n  method: put\n  operationId: update-an-invoice\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file/dispute/{evidenceFileId}\n  method: delete\n  operationId: delete-evidence-for-dispute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{id}/registration/file/{file_id}\n  method: delete\n  operationId: delete-file-from-merchant-registration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice/schedule/{id}\n  method: delete\n  operationId: delete-invoice-schedule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice/schedule/{id}\n  method: put\n  operationId: editInvoiceSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/statement/v3/disputes\n  method:\
  \ get\n  operationId: disputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}/receipt/email\n  method: put\n  operationId: e-mail-transaction-receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file/{id}\n  method: put\n  operationId: put_file{id}\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file/{id}\n  method: get\n  operationId: get_file{id}\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/enroll\n  method: post\n  operationId: enroll-a-merchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ephemeral\n  method: get\n  operationId: ephemeral-authentication-tokens-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file/{tag}\n  method: get\n  operationId: get_file{tag}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/payment-links/{id}/is-active\n  method: get\n  operationId: get-a-payment-links-active-status\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}/related\n  method: get\n  operationId: get-a-related-transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}/funding\n  method: get\n  operationId: get-a-transactions-funding-instructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}\n  method: get\n  operationId: get-a-transactions-information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /terminal/register\n  method: get\n  operationId: get-all-devices\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/{customerId}/payment-method\n  method: get\n  operationId: get-all-payment-methods-for-a-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/depositDetail\n  method: get\n  operationId: get-detail-of-specific-deposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/deposit\n  method: get\n  operationId: get-list-of-deposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/{merchant_id}\n  method: get\n  operationId: get-merchant-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/{id}/registration\n  method: get\n  operationId: get-merchant-registration-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/{id}/registration\n  method: put\n  operationId: update-merchant-registration-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /underwriting/merchant/{id}/registration/documents\n  method: get\n  operationId: get-registration-documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/user/{id}\n  method: put\n  operationId: get-team-members-information-copy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/user/{id}\n  method: get\n  operationId: get-team-members-information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/registration\n  method: get\n  operationId: get-team-registration-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/registration\n  method: put\n  operationId: update-team-registration-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terminal/{registerId}/status/{transactionId}\n  method: get\n  operationId: get-transaction-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/{id}\n  method: delete\n  operationId: delete-a-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /item/{id}/increment\n  method: put\n  operationId: increment-items-stock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /forgot\n  method: post\n  operationId: initiate-password-reset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /merchant/{merchant_id}/user/{user_id}\n  method: post\n  operationId: link-existing-user-to-merchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{merchant_id}/user/{user_id}\n  method: delete\n  operationId: unlink-user-from-merchant\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction\n  method: get\n  operationId: list-and-filter-all-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/apikey\n  method: get\n  operationId: list-api-keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /underwriting/disputes/{merchantId}\n  method: get\n  operationId: list-disputes-copy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /underwriting/disputes\n  method: get\n  operationId: list-disputes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice/{id}/pay/{method}\n  method: post\n  operationId: mark-an-invoice-paid-in-cash-or-check\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice/{id}/pay\n  method: post\n  operationId: pay-an-invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terminal/print\n  method:\
  \ post\n  operationId: print\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terminal/promptChoice\n  method: post\n  operationId: get_terminalpromptChoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terminal/promptInput\n  method: post\n  operationId: prompt-input\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /terminal/prompt/signature\n  method: post\n  operationId: prompt-signature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/statement/v3/adjustments\n  method: get\n  operationId: refund-and-adjustments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}/refund\n  method: post\n  operationId: refund-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /terminal/refund\n  method: post\n  operationId: refund\n  x-agentic-ac\n\n# --- truncated at 32 KB (40 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/stax/refs/heads/main/agentic-access/stax-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stax/refs/heads/main/agentic-access/stax-agentic-access.yml
summary_line: 133 operations · 79 acting · 2 human-in-the-loop
tags:
- Payments
- Payment Processing
- Merchant Services
- Embedded Payments
- ACH
- Invoicing
- Subscription Billing
- Surcharging
- Point-of-Sale
- Tokenization
- Financial-Services
- Fintech
- Card Present
- Merchant Onboarding
---
