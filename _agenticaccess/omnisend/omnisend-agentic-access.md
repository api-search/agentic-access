---
acting_count: 54
action_class_counts:
  acting: 54
  connected: 28
api_specs:
- filename: omnisend-brands-api-openapi.yml
  format: yaml
  label: Omnisend Brands API
  slug: omnisend-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-brands-api-openapi.yml
- filename: omnisend-campaigns-api-openapi.yml
  format: yaml
  label: Omnisend Campaigns API
  slug: omnisend-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-campaigns-api-openapi.yml
- filename: omnisend-contacts-api-openapi.yml
  format: yaml
  label: Omnisend Contacts API
  slug: omnisend-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-contacts-api-openapi.yml
- filename: omnisend-events-api-openapi.yml
  format: yaml
  label: Omnisend Events API
  slug: omnisend-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-events-api-openapi.yml
- filename: omnisend-images-api-openapi.yml
  format: yaml
  label: Omnisend Images API
  slug: omnisend-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-images-api-openapi.yml
- filename: omnisend-products-api-openapi.yml
  format: yaml
  label: Omnisend Products API
  slug: omnisend-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-products-api-openapi.yml
- filename: omnisend-segments-api-openapi.yml
  format: yaml
  label: Omnisend Segments API
  slug: omnisend-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-segments-api-openapi.yml
- filename: omnisend-automations-api-openapi.yml
  format: yaml
  label: Omnisend Automations API
  slug: omnisend-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-automations-api-openapi.yml
- filename: omnisend-event-metadata-api-openapi.yml
  format: yaml
  label: Omnisend Event Metadata API
  slug: omnisend-event-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-event-metadata-api-openapi.yml
- filename: omnisend-batch-api-openapi.yml
  format: yaml
  label: Omnisend Batch API
  slug: omnisend-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-batch-api-openapi.yml
- filename: omnisend-email-content-api-openapi.yml
  format: yaml
  label: Omnisend Email Content API
  slug: omnisend-email-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-email-content-api-openapi.yml
- filename: omnisend-email-templates-api-openapi.yml
  format: yaml
  label: Omnisend Email Templates API
  slug: omnisend-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-email-templates-api-openapi.yml
- filename: omnisend-email-universal-layouts-api-openapi.yml
  format: yaml
  label: Omnisend Email Universal Layouts API
  slug: omnisend-email-universal-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-email-universal-layouts-api-openapi.yml
- filename: omnisend-product-categories-api-openapi.yml
  format: yaml
  label: Omnisend Product Categories API
  slug: omnisend-product-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-product-categories-api-openapi.yml
- filename: omnisend-reports-api-openapi.yml
  format: yaml
  label: Omnisend Reports API
  slug: omnisend-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-reports-api-openapi.yml
- filename: omnisend-statistics-api-openapi.yml
  format: yaml
  label: Omnisend Statistics API
  slug: omnisend-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-statistics-api-openapi.yml
consequence_counts:
  physical: 4
  read: 28
  safety-critical: 2
  write: 48
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Omnisend Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /automations/{id}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /campaigns/{id}/ab-test/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /automations/{id}/blocks/{blockID}/test-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /campaigns/{id}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /campaigns/{id}/test-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /events
operation_count: 82
overview: 'Omnisend exposes 82 API operations that an AI agent could call, of which 54 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 48 write, 4 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Omnisend
provider_slug: omnisend
slug: omnisend-agentic-access
source_filename: omnisend-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/omnisend-automations-api-openapi.yml, openapi/omnisend-batch-api-openapi.yml,\n  openapi/omnisend-brands-api-openapi.yml, openapi/omnisend-campaigns-api-openapi.yml, openapi/omnisend-contacts-api-openapi.yml,\n  openapi/omnisend-email-content-api-openapi.yml, openapi/omnisend-email-templates-api-openapi.yml,\n  openapi/omnisend-email-universal-layouts-api-openapi.yml, openapi/omnisend-event-metadata-api-openapi.yml,\n  openapi/omnisend-events-api-openapi.yml, openapi/omnisend-images-api-openapi.yml, openapi/omnisend-product-categories-api-openapi.yml,\n  openapi/omnisend-products-api-openapi.yml, openapi/omnisend-reports-api-openapi.yml, openapi/omnisend-segments-api-openapi.yml,\n  openapi/omnisend-statistics-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n\
  \  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 82\n  by_action_class:\n    connected: 28\n    acting: 54\n  by_consequence:\n    read: 28\n    write: 48\n    physical: 4\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /automations\n  method: get\n  operationId: getAutomations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - automations.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /automations\n  method: post\n  operationId: postAutomations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - automations.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /automations/{id}\n  method: delete\n  operationId: deleteAutomationsById\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - automations.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /automations/{id}\n  method: get\n  operationId: getAutomationsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - automations.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /automations/{id}\n  method: patch\n  operationId: patchAutomationsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - automations.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /automations/{id}/blocks\n\
  \  method: put\n  operationId: putAutomationsByIdBlocks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - automations.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /automations/{id}/blocks/{blockID}/test-email\n  method: post\n  operationId: postAutomationsByIdBlocksByBlockIDTestEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - automations.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /automations/{id}/blocks/{blockID}/utm\n  method: get\n  operationId: getAutomationsByIdBlocksByBlockIDUtm\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - automations.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /automations/{id}/blocks/{blockID}/utm\n  method: put\n  operationId: putAutomationsByIdBlocksByBlockIDUtm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - automations.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /automations/{id}/copy\n  method: post\n  operationId: postAutomationsByIdCopy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - automations.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /automations/{id}/disable\n  method: post\n  operationId: postAutomationsByIdDisable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - automations.write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /automations/{id}/enable\n  method: post\n  operationId: postAutomationsByIdEnable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - automations.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /automations/{id}/utm\n  method: get\n  operationId: getAutomationsByIdUtm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - automations.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches\n  method: get\n  operationId: getBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - contacts.read\n    - events.read\n    - products.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches\n  method: post\n  operationId: postBatches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - contacts.write\n    - events.write\n    - products.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batches/{batchID}\n  method: get\n  operationId: getBatchesByBatchID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - contacts.read\n\
  \    - events.read\n    - products.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches/{batchID}/items\n  method: get\n  operationId: getBatchesByBatchIDItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - contacts.read\n    - events.read\n    - products.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/current\n  method: get\n  operationId: getBrandsCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - brands.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/current\n  method: post\n  operationId: postBrandsCurrent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - brands.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /campaigns\n  method: get\n  operationId: getCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - campaigns.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: post\n  operationId: postCampaigns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}\n  method: delete\n  operationId: deleteCampaignsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /campaigns/{id}\n  method: get\n  operationId: getCampaignsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - campaigns.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}\n  method: patch\n  operationId: patchCampaignsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/ab-test/resume\n  method: post\n  operationId: postCampaignsByIdAbTestResume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/ab-test/stop\n  method: post\n  operationId: postCampaignsByIdAbTestStop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /campaigns/{id}/ab-test/winner\n  method: post\n  operationId: postCampaignsByIdAbTestWinner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/cancel\n  method: post\n\
  \  operationId: postCampaignsByIdCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/copy\n  method: post\n  operationId: postCampaignsByIdCopy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/send\n  method: post\n  operationId: postCampaignsByIdSend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n  \
  \    max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/test-email\n  method: post\n  operationId: postCampaignsByIdTestEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/utm\n  method: get\n  operationId: getCampaignsByIdUtm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - campaigns.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/utm\n  method: put\n  operationId: putCampaignsByIdUtm\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - campaigns.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - contacts.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: patch\n  operationId: patchContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - contacts.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: post\n  operationId: postContacts\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - contacts.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: get\n  operationId: getContactsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - contacts.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}\n  method: patch\n  operationId: patchContactsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - contacts.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/tags\n  method: delete\n  operationId: deleteContactsTags\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - contacts.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/tags\n  method: post\n  operationId: postContactsTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - contacts.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-content/{id}\n  method: get\n  operationId: getEmailContentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email-templates.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-content/{id}\n  method:\
  \ put\n  operationId: putEmailContentById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-content/{id}/render\n  method: post\n  operationId: postEmailContentByIdRender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-templates\n  method: get\n  operationId: getEmailTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email-templates.read\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /email-templates\n  method: post\n  operationId: postEmailTemplates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-templates/{id}\n  method: delete\n  operationId: deleteEmailTemplatesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-templates/{id}\n  method: get\n  operationId: getEmailTemplatesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    scope:\n    - email-templates.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-templates/{id}\n  method: put\n  operationId: putEmailTemplatesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-templates/{id}/render\n  method: post\n  operationId: postEmailTemplatesByIdRender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-templates/import\n  method: post\n  operationId: postEmailTemplatesImport\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-universal-layouts\n  method: get\n  operationId: getEmailUniversalLayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email-templates.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-universal-layouts\n  method: post\n  operationId: postEmailUniversalLayouts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /email-universal-layouts/{id}\n  method: delete\n  operationId: deleteEmailUniversalLayoutsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email-universal-layouts/{id}\n  method: get\n  operationId: getEmailUniversalLayoutsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email-templates.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-universal-layouts/{id}\n  method: put\n  operationId: putEmailUniversalLayoutsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - email-templates.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event-metadata\n  method: post\n  operationId: post_event_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event-metadata\n  method: put\n  operationId: put_event_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event-metadata/query\n  method: post\n  operationId: post_event_metadata_query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: post\n  operationId: postEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - events.write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images\n  method: get\n  operationId: getImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - images.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images\n  method: post\n  operationId: postImages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - images.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/{id}\n  method: delete\n  operationId: deleteImagesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - images.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/{id}\n  method: get\n  operationId: getImagesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - images.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/upload\n  method: post\n  operationId: postImagesUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - images.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product-categories\n  method: get\n  operationId: getProductCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product-categories\n  method: post\n  operationId: postProductCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product-categories/{categoryID}\n  method: delete\n  operationId: deleteProductCategoriesByCategoryID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products.write\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product-categories/{categoryID}\n  method: get\n  operationId: getProductCategoriesByCategoryID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - products.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product-categories/{categoryID}\n  method: patch\n  operationId: patchProductCategoriesByCategoryID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products\n  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - products.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: post\n  operationId: postProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{productID}\n  method: delete\n  operationId: deleteProductsByProductID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/{productID}\n  method: get\n  operationId: getProductsByProductID\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - products.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productID}\n  method: put\n  operationId: putProductsByProductID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - products.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/reports\n  method: post\n  operationId: postAnalyticsReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - analytics.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /segments\n  method: get\n  operationId: getSegments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - segments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /segments\n  method: post\n  operationId: postSegments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - segments.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /segments/{segmentID}\n  method: delete\n  operationId: deleteSegmentsBySegmentID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - segments.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /segments/{segmentID}\n  method: get\n  operationId: getSegmentsBySegmentID\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - segments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /segments/{segmentID}\n  method: put\n  operationId: putSegmentsBySegmentID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - segments.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /segments/{segmentID}/statistics\n  method: get\n  operationId: getSegmentsBySegmentIDStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - segments.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/statistics\n  method: post\n  operationId: postAnalyticsStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - analytics.read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/agentic-access/omnisend-agentic-access.yml
summary_line: 82 operations · 54 acting · 2 human-in-the-loop
tags:
- Email Marketing
- Marketing Automation
- E-Commerce
- SMS Marketing
- Customer Engagement
- Segmentation
- Campaigns
- Forms
- Popups
- Web Push
- Automation Workflows
- Analytics
- MCP
- Agent Ready
- Transactional Messaging
---
