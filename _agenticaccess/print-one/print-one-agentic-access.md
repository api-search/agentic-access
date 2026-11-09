---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 24
api_specs:
- filename: print-one-address-api-openapi.yml
  format: yaml
  label: print-one Address API
  slug: print-one-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-address-api-openapi.yml
- filename: print-one-campaigns-api-openapi.yml
  format: yaml
  label: print-one Campaigns API
  slug: print-one-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-campaigns-api-openapi.yml
- filename: print-one-coupons-api-openapi.yml
  format: yaml
  label: print-one Coupons API
  slug: print-one-coupons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-coupons-api-openapi.yml
- filename: print-one-design-previews-api-openapi.yml
  format: yaml
  label: print-one Design Previews API
  slug: print-one-design-previews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-design-previews-api-openapi.yml
- filename: print-one-designs-api-openapi.yml
  format: yaml
  label: print-one Designs API
  slug: print-one-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-designs-api-openapi.yml
- filename: print-one-imports-api-openapi.yml
  format: yaml
  label: print-one Imports API
  slug: print-one-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-imports-api-openapi.yml
- filename: print-one-items-api-openapi.yml
  format: yaml
  label: print-one Items API
  slug: print-one-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-items-api-openapi.yml
- filename: print-one-mailings-api-openapi.yml
  format: yaml
  label: print-one Mailings API
  slug: print-one-mailings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-mailings-api-openapi.yml
- filename: print-one-webhooks-api-openapi.yml
  format: yaml
  label: print-one Webhooks API
  slug: print-one-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-webhooks-api-openapi.yml
- filename: print-one-webhook-events-api-openapi.yml
  format: yaml
  label: print-one Webhook Events API
  slug: print-one-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-webhook-events-api-openapi.yml
consequence_counts:
  physical: 2
  read: 24
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Print One Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/campaigns/{campaignId}/imports/{importId}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/campaigns/{campaignId}/items/{itemId}/send
operation_count: 49
overview: 'print-one exposes 49 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 23 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: print-one
provider_slug: print-one
slug: print-one-agentic-access
source_filename: print-one-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/print-one-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    acting: 25\n    connected: 24\n  by_consequence:\n    write: 23\n    read: 24\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/address/validate\n  method: post\n  operationId: Address/validateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - live.orders.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/address/auto-complete\n\
  \  method: post\n  operationId: Address/autoCompleteAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - live.orders.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns\n  method: get\n  operationId: Campaign/getCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - campaign.read\n    - live.api.key\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}\n  method: get\n  operationId: Campaign/getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - campaign.read\n    - live.api.key\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v3/campaigns/{campaignId}\n  method: patch\n  operationId: Campaign/updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaign.write\n    - live.api.key\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/pause\n  method: post\n  operationId: Campaign/pauseCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaign.write\n    - live.api.key\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/resume\n  method: post\n  operationId: Campaign/resumeCampaign\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaign.write\n    - live.api.key\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/designs/preview\n  method: post\n  operationId: CampaignDesignPreviews/createDesignPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - template.read\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/designs/{destination}/{designId}/{version}/preview\n  method: post\n  operationId: CampaignDesignPreviews/createDesignDestinationPreview\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - template.read\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/designs/{destination}/{designId}/{version}/preview/{previewId}\n  method: get\n  operationId: CampaignDesignPreviews/getDesignPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - live.api.key\n    - template.read\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/designs/{destination}/{designId}/{version}/preview/{previewId}/details\n  method: get\n  operationId: CampaignDesignPreviews/getDesignPreviewDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - live.api.key\n    - template.read\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/designs/{destination}\n  method: post\n  operationId: CampaignDesigns/createDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - template.write\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/designs/{destination}/{designId}\n  method: get\n  operationId: CampaignDesigns/getDesign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - live.api.key\n    - template.read\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/designs/{destination}/{designId}\n\
  \  method: patch\n  operationId: CampaignDesigns/updateDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - template.write\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/designs/{destination}/{designId}\n  method: delete\n  operationId: CampaignDesigns/deleteDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - template.write\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/designs\n  method: get\n  operationId: CampaignDesigns/getDesigns\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - live.api.key\n    - template.read\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/items\n  method: post\n  operationId: CampaignItems/addItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - draft.orders.write\n    - live.api.key\n    - live.orders.write\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/items\n  method: get\n  operationId: CampaignItems/getItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n    - live.api.key\n    - live.orders.read\n    - tenant.admin\n    - test.api.key\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/items/{itemId}\n  method: get\n  operationId: CampaignItems/getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n    - live.api.key\n    - live.orders.read\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/items/{itemId}\n  method: patch\n  operationId: CampaignItems/updateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - draft.orders.write\n    - live.api.key\n    - live.orders.write\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/items/{itemId}/cancel\n  method: post\n  operationId: CampaignItems/cancelItem\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - draft.orders.write\n    - live.api.key\n    - live.orders.write\n    - tenant.admin\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/items/{itemId}/send\n  method: post\n  operationId: CampaignItems/markItemDeliverable\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - live.api.key\n    - live.orders.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/items/{itemId}/preview\n  method: get\n  operationId:\
  \ CampaignItems/getItemPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n    - live.api.key\n    - live.orders.read\n    - tenant.admin\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/mailings\n  method: get\n  operationId: CampaignMailings/getMailings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - live.api.key\n    - live.orders.read\n    - tenant.admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/mailings/{mailingId}\n  method: get\n  operationId: CampaignMailings/getMailing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - live.api.key\n    - live.orders.read\n    - tenant.admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/mailings/{mailingId}/items\n\
  \  method: get\n  operationId: CampaignMailings/getMailingItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n    - live.api.key\n    - live.orders.read\n    - tenant.admin\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/mailings/{mailingId}/items/{itemId}\n  method: get\n  operationId: CampaignMailings/getMailingItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n    - live.api.key\n    - live.orders.read\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/mailings/{mailingId}/items/{itemId}/preview\n  method: get\n  operationId: CampaignMailings/getMailingItemPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n  \
  \  - live.api.key\n    - live.orders.read\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/imports\n  method: post\n  operationId: CampaignImports/createImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - draft.orders.write\n    - live.api.key\n    - live.orders.write\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/imports\n  method: get\n  operationId: CampaignImports/getImports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n    - live.api.key\n    - live.orders.read\n    - tenant.admin\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/imports/{importId}\n\
  \  method: get\n  operationId: CampaignImports/getImportDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n    - live.api.key\n    - live.orders.read\n    - tenant.admin\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/imports/{importId}/csv\n  method: get\n  operationId: CampaignImports/downloadImportCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n    - live.api.key\n    - live.orders.read\n    - tenant.admin\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/imports/{importId}/items\n  method: get\n  operationId: CampaignImports/getImportItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - draft.orders.read\n    - live.api.key\n\
  \    - live.orders.read\n    - tenant.admin\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/campaigns/{campaignId}/imports/{importId}/cancel\n  method: post\n  operationId: CampaignImports/cancelImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - draft.orders.write\n    - live.api.key\n    - live.orders.write\n    - tenant.admin\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/imports/{importId}/preview/{rowId}\n  method: post\n  operationId: CampaignImports/previewImportItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - draft.orders.write\n    - live.api.key\n    - live.orders.write\n    - test.api.key\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/imports/{importId}/process\n  method: post\n  operationId: CampaignImports/processImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - draft.orders.write\n    - live.api.key\n    - live.orders.write\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/campaigns/{campaignId}/imports/{importId}/send\n  method: post\n  operationId: CampaignImports/sendImport\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - draft.orders.write\n    - live.api.key\n    - live.orders.write\n    - test.api.key\n    audience: null\n   \
  \ token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/coupons\n  method: post\n  operationId: Coupons/addCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - coupons.write\n    - live.api.key\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/coupons\n  method: get\n  operationId: Coupons/getCouponsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - coupons.read\n    - live.api.key\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/coupons/{id}\n  method: get\n  operationId: Coupons/getCoupon\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - coupons.read\n    - live.api.key\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/coupons/{id}\n  method: delete\n  operationId: Coupons/deleteCoupon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - coupons.write\n    - live.api.key\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/coupons/{id}\n  method: post\n  operationId: Coupons/importCouponCodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - coupons.write\n    - live.api.key\n    - test.api.key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/coupons/{id}/codes\n  method: get\n  operationId: Coupons/getCouponCodesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - coupons.read\n    - live.api.key\n    - test.api.key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/webhooks\n  method: post\n  operationId: Webhook/createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - tenant.admin\n    - webhooks.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/webhooks\n  method: get\n  operationId: Webhook/getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - live.api.key\n\
  \    - webhooks.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/webhooks/{id}\n  method: get\n  operationId: Webhook/getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - live.api.key\n    - webhooks.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/webhooks/{id}\n  method: patch\n  operationId: Webhook/updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - webhooks.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/webhooks/{id}\n  method: delete\n  operationId: Webhook/deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - live.api.key\n    - tenant.admin\n    - webhooks.write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/webhooks/{id}/logs\n  method: get\n  operationId: Webhook/getWebhookLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - live.api.key\n    - webhooks.read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/print-one/agentic-access/print-one-agentic-access.yml
summary_line: 49 operations · 25 acting
tags:
- Postcards
- Direct Mail
- Marketing
- Automation
---
