---
acting_count: 105
action_class_counts:
  acting: 105
  connected: 72
api_specs:
- filename: surfingdog-ai-census-api-openapi.yml
  format: yaml
  label: surfingdog-ai Census API
  slug: surfingdog-ai-census-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-census-api-openapi.yml
- filename: surfingdog-ai-directory-api-openapi.yml
  format: yaml
  label: surfingdog-ai Directory API
  slug: surfingdog-ai-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-directory-api-openapi.yml
- filename: surfingdog-ai-integrations-api-openapi.yml
  format: yaml
  label: surfingdog-ai Integrations API
  slug: surfingdog-ai-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-integrations-api-openapi.yml
- filename: surfingdog-ai-keys-api-openapi.yml
  format: yaml
  label: surfingdog-ai Keys API
  slug: surfingdog-ai-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-keys-api-openapi.yml
- filename: surfingdog-ai-owner-api-openapi.yml
  format: yaml
  label: surfingdog-ai Owner API
  slug: surfingdog-ai-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-owner-api-openapi.yml
- filename: surfingdog-ai-owners-api-openapi.yml
  format: yaml
  label: surfingdog-ai Owners API
  slug: surfingdog-ai-owners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-owners-api-openapi.yml
- filename: surfingdog-ai-products-api-openapi.yml
  format: yaml
  label: surfingdog-ai Products API
  slug: surfingdog-ai-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-products-api-openapi.yml
- filename: surfingdog-ai-public-api-openapi.yml
  format: yaml
  label: surfingdog-ai Public API
  slug: surfingdog-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-public-api-openapi.yml
- filename: surfingdog-ai-reports-api-openapi.yml
  format: yaml
  label: surfingdog-ai Reports API
  slug: surfingdog-ai-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-reports-api-openapi.yml
- filename: surfingdog-ai-rules-api-openapi.yml
  format: yaml
  label: surfingdog-ai Rules API
  slug: surfingdog-ai-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-rules-api-openapi.yml
- filename: surfingdog-ai-score-api-openapi.yml
  format: yaml
  label: surfingdog-ai Score API
  slug: surfingdog-ai-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-score-api-openapi.yml
- filename: surfingdog-ai-setup-api-openapi.yml
  format: yaml
  label: surfingdog-ai Setup API
  slug: surfingdog-ai-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-setup-api-openapi.yml
- filename: surfingdog-ai-stays-api-openapi.yml
  format: yaml
  label: surfingdog-ai Stays API
  slug: surfingdog-ai-stays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/surfingdog-ai/openapi/surfingdog-ai-stays-api-openapi.yml
consequence_counts:
  physical: 23
  read: 72
  safety-critical: 9
  write: 73
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 9
kind: agentic-access
layout: agentic-access
method: generated
name: Surfingdog Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/owner/api-keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/owner/customers/{id}/networks-off
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/owner/email/forwards/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/owner/email/forwards/{id}/confirmed
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/owner/email/sender
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/owner/integrations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/owner/integrations/{id}/link
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/owner/items/{id}/payments/stop-waiting
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/owner/rules/presets/{key}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/items/{id}/accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/items/{id}/details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/items/{id}/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/items/{id}/returns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/items/{id}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/owner/deliveries/{id}/replay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/owner/download/code
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/owner/email/forwards/{id}/check
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/owner/email/sender/check
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/owner/items/{id}/always-put-aside
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/owner/items/{id}/job-tool
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/owner/items/{id}/let-in
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/owner/items/{id}/looks-fine
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/owner/items/{id}/offers
operation_count: 177
overview: 'surfingdog-ai exposes 177 API operations that an AI agent could call, of which 105 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 72 read, 73 write, 23 physical, and 9 safety-critical.


  9 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: surfingdog-ai
provider_slug: surfingdog-ai
slug: surfingdog-ai-agentic-access
source_filename: surfingdog-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/inbox-openapi.json, openapi/network-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 177\n  by_action_class:\n    connected: 72\n    acting: 105\n  by_consequence:\n    read: 72\n    write: 73\n    physical: 23\n    safety-critical: 9\n  human_in_the_loop_required: 9\noperations:\n- path: /v1/owner/items\n  method: get\n  operationId: getV1OwnerItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/items/{id}\n  method: get\n  operationId: getV1OwnerItemsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/spam\n  method: get\n  operationId: getV1OwnerSpam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/spam/filters/{filter}\n  method: put\n  operationId: putV1OwnerSpamFiltersByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/spam/ai\n  method: put\n  operationId: putV1OwnerSpamAi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/owner/spam/filters/{filter}/start\n  method: post\n  operationId: postV1OwnerSpamFiltersByFilterStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/spam/lists/domains\n  method: post\n  operationId: postV1OwnerSpamListsDomains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/spam/lists\n  method: delete\n  operationId: deleteV1OwnerSpamLists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/spam/model\n  method: get\n  operationId: getV1OwnerSpamModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/spam/model\n  method: put\n  operationId: putV1OwnerSpamModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/spam/model\n  method: delete\n  operationId: deleteV1OwnerSpamModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/spam/model/models\n  method: post\n  operationId: postV1OwnerSpamModelModels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/spam/model/test\n  method: post\n  operationId: postV1OwnerSpamModelTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/let-in\n  method: post\n  operationId: postV1OwnerItemsByIdLetIn\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/looks-fine\n  method: post\n  operationId: postV1OwnerItemsByIdLooksFine\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/spam\n  method: post\n  operationId: postV1OwnerItemsByIdSpam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/owner/items/{id}/always-put-aside\n  method: post\n  operationId: postV1OwnerItemsByIdAlwaysPutAside\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/transitions\n  method: post\n  operationId: postV1OwnerItemsByIdTransitions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/returns\n  method: post\n  operationId: postV1OwnerItemsByIdReturns\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/offers\n  method: get\n  operationId: getV1OwnerItemsByIdOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/items/{id}/offers\n  method: post\n  operationId: postV1OwnerItemsByIdOffers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/payments\n  method:\
  \ get\n  operationId: getV1OwnerItemsByIdPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/items/{id}/payments/shop-total\n  method: post\n  operationId: postV1OwnerItemsByIdPaymentsShopTotal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/payments/stop-waiting\n  method: post\n  operationId: postV1OwnerItemsByIdPaymentsStopWaiting\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/owner/items/{id}/offers/draft/send\n  method: post\n  operationId: postV1OwnerItemsByIdOffersDraftSend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/offers/draft\n  method: delete\n  operationId: deleteV1OwnerItemsByIdOffersDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/replies\n  method: post\n  operationId: postV1OwnerItemsByIdReplies\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/customers/{id}\n  method: get\n  operationId: getV1OwnerCustomersById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/customers/{id}/export\n  method: get\n  operationId: getV1OwnerCustomersByIdExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/customers/{id}/networks-off\n  method: post\n  operationId: postV1OwnerCustomersByIdNetworksOff\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/owner/customers/{id}/erase\n  method: post\n  operationId: postV1OwnerCustomersByIdErase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/mail\n  method: get\n  operationId: getV1OwnerMail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/email\n  method: get\n  operationId: getV1OwnerEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/owner/email/provider\n  method: get\n  operationId: getV1OwnerEmailProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/email/forwards\n  method: post\n  operationId: postV1OwnerEmailForwards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/email/forwards/{id}\n  method: delete\n  operationId: deleteV1OwnerEmailForwardsById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/owner/email/forwards/{id}/check\n  method: post\n  operationId: postV1OwnerEmailForwardsByIdCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/email/forwards/{id}/confirmed\n  method: post\n  operationId: postV1OwnerEmailForwardsByIdConfirmed\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/owner/email/sender\n  method: put\n  operationId: putV1OwnerEmailSender\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/owner/email/sender/check\n  method: post\n  operationId: postV1OwnerEmailSenderCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/items/{id}/attachments\n  method: get\n  operationId: getV1OwnerItemsByIdAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/attachments/{id}\n\
  \  method: delete\n  operationId: deleteV1OwnerAttachmentsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/attachments/{id}\n  method: get\n  operationId: getV1OwnerAttachmentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/settings\n  method: get\n  operationId: getV1OwnerSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/settings\n  method: put\n  operationId: putV1OwnerSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/receipts\n  method: get\n  operationId: getV1OwnerReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/receipt-keys/rotate\n  method: post\n  operationId: postV1OwnerReceiptKeysRotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/networks\n  method: get\n  operationId: getV1OwnerNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/discovery\n\
  \  method: get\n  operationId: getV1OwnerDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/discovery/check\n  method: post\n  operationId: postV1OwnerDiscoveryCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/profile\n  method: get\n  operationId: getV1OwnerProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/profile\n  method: put\n  operationId: putV1OwnerProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/services\n  method: get\n  operationId: getV1OwnerServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/services\n  method: post\n  operationId: postV1OwnerServices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/services/{id}\n  method: patch\n  operationId: patchV1OwnerServicesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/services/{id}\n  method: delete\n  operationId: deleteV1OwnerServicesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/products\n  method: get\n  operationId: getV1OwnerProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/products\n  method: post\n  operationId: postV1OwnerProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/owner/products/{id}\n  method: patch\n  operationId: patchV1OwnerProductsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/products/{id}\n  method: delete\n  operationId: deleteV1OwnerProductsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/products/{id}/barcode\n  method: post\n  operationId: postV1OwnerProductsByIdBarcode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/catalogue\n  method: get\n  operationId: getV1OwnerCatalogue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/catalogue/sku-barcodes\n  method: post\n  operationId: postV1OwnerCatalogueSkuBarcodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/catalogue/floors\n  method: get\n  operationId: getV1OwnerCatalogueFloors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/catalogue/floors\n\
  \  method: put\n  operationId: putV1OwnerCatalogueFloors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/availability\n  method: get\n  operationId: getV1OwnerAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/availability\n  method: put\n  operationId: putV1OwnerAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/availability/{serviceId}\n  method: delete\n  operationId:\
  \ deleteV1OwnerAvailabilityByServiceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/availability/closures\n  method: put\n  operationId: putV1OwnerAvailabilityClosures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/rules\n  method: get\n  operationId: getV1OwnerRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/rules\n  method: post\n  operationId: postV1OwnerRules\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/rules/presets\n  method: get\n  operationId: getV1OwnerRulesPresets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/rules/presets/{key}\n  method: post\n  operationId: postV1OwnerRulesPresetsByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/owner/setup/plan\n  method: post\n  operationId: postV1OwnerSetupPlan\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/rules/test\n  method: post\n  operationId: postV1OwnerRulesTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/rules/{id}\n  method: patch\n  operationId: patchV1OwnerRulesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/rules/{id}\n\
  \  method: delete\n  operationId: deleteV1OwnerRulesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/webhooks\n  method: get\n  operationId: getV1OwnerWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/webhooks\n  method: post\n  operationId: postV1OwnerWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/webhooks/{id}\n  method: patch\n  operationId: patchV1OwnerWebhooksById\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/webhooks/{id}\n  method: delete\n  operationId: deleteV1OwnerWebhooksById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/feeds\n  method: get\n  operationId: getV1OwnerFeeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/feeds\n  method: post\n  operationId: postV1OwnerFeeds\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/feeds/{id}\n  method: get\n  operationId: getV1OwnerFeedsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/feeds/{id}\n  method: delete\n  operationId: deleteV1OwnerFeedsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/feeds/{id}/import\n  method: post\n  operationId: postV1OwnerFeedsByIdImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/integrations\n  method: get\n  operationId: getV1OwnerIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/integrations\n  method: post\n  operationId: postV1OwnerIntegrations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/integrations/authorize\n  method: post\n  operationId: postV1OwnerIntegrationsAuthorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/integrations/{id}\n  method: get\n  operationId: getV1OwnerIntegrationsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/integrations/{id}\n  method: patch\n  operationId: patchV1OwnerIntegrationsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/integrations/{id}\n  method: delete\n  operationId: deleteV1OwnerIntegrationsById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/owner/integrations/{id}/sync\n  method: post\n  operationId: postV1OwnerIntegrationsByIdSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/integrations/{id}/link\n  method: post\n  operationId: postV1OwnerIntegrationsByIdLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /v1/owner/webhooks/{id}/rotate-secret\n  method: post\n  operationId: postV1OwnerWebhooksByIdRotateSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/webhooks/{id}/test\n  method: post\n  operationId: postV1OwnerWebhooksByIdTest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/webhooks/{id}/replay\n  method: post\n  operationId: postV1OwnerWebhooksByIdReplay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/owner/webhooks/{id}/deliveries\n  method: get\n  operationId: getV1OwnerWebhooksByIdDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/owner/deliveries\n  method: get\n  operationId: getV1OwnerDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (53 KB total) ---\n# Full source: https://artifacts.apis.io/surfingdog-ai/agentic-access/surfingdog-ai-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/surfingdog-ai/agentic-access/surfingdog-ai-agentic-access.yml
summary_line: 177 operations · 105 acting · 9 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Agent Ready
- Directory
- Inbox
---
