---
acting_count: 134
action_class_counts:
  acting: 134
  connected: 85
api_specs:
- filename: dishdirectory-com-academy-api-openapi.yml
  format: yaml
  label: Dish Directory Academy API
  slug: dishdirectory-com-academy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-academy-api-openapi.yml
- filename: dishdirectory-com-admin-api-openapi.yml
  format: yaml
  label: Dish Directory Admin API
  slug: dishdirectory-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-admin-api-openapi.yml
- filename: dishdirectory-com-categories-api-openapi.yml
  format: yaml
  label: Dish Directory Categories API
  slug: dishdirectory-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-categories-api-openapi.yml
- filename: dishdirectory-com-certificates-api-openapi.yml
  format: yaml
  label: Dish Directory Certificates API
  slug: dishdirectory-com-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-certificates-api-openapi.yml
- filename: dishdirectory-com-listings-api-openapi.yml
  format: yaml
  label: Dish Directory Listings API
  slug: dishdirectory-com-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-listings-api-openapi.yml
- filename: dishdirectory-com-places-api-openapi.yml
  format: yaml
  label: Dish Directory Places API
  slug: dishdirectory-com-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-places-api-openapi.yml
- filename: dishdirectory-com-product-categories-api-openapi.yml
  format: yaml
  label: Dish Directory Product Categories API
  slug: dishdirectory-com-product-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-product-categories-api-openapi.yml
- filename: dishdirectory-com-products-api-openapi.yml
  format: yaml
  label: Dish Directory Products API
  slug: dishdirectory-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-products-api-openapi.yml
- filename: dishdirectory-com-sources-api-openapi.yml
  format: yaml
  label: Dish Directory Sources API
  slug: dishdirectory-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-sources-api-openapi.yml
- filename: dishdirectory-com-stats-api-openapi.yml
  format: yaml
  label: Dish Directory Stats API
  slug: dishdirectory-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dishdirectory-com/openapi/dishdirectory-com-stats-api-openapi.yml
consequence_counts:
  physical: 26
  read: 85
  safety-critical: 17
  write: 91
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 17
kind: agentic-access
layout: agentic-access
method: generated
name: Dishdirectory Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/academy/certificates
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/academy/certificates/{code}/extend
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/academy/certificates/{code}/reinstate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/academy/certificates/{code}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/academy/memberships/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/billing/invoices/{id}/refund
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/claims/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/leads/dispatch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/leads/drips
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/listings/{id}/owner
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /admin/listings/{slug}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/newsletter/api-keys
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /admin/outreach/sender
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/tokens/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/users/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/users/{id}/sessions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /admin/video/jobs/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/academy/courses/{slug}/images
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/academy/courses/{slug}/publish
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/academy/courses/{slug}/questions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/academy/memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/billing/retry
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/leads/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /admin/listings/{slug}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /admin/listings/{slug}/photos
operation_count: 219
overview: 'Dish Directory exposes 219 API operations that an AI agent could call, of which 134 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 85 read, 91 write, 26 physical, and 17 safety-critical.


  17 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dish Directory
provider_slug: dishdirectory-com
slug: dishdirectory-com-agentic-access
source_filename: dishdirectory-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dishdirectory-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 219\n  by_action_class:\n    connected: 85\n    acting: 134\n  by_consequence:\n    read: 85\n    physical: 26\n    write: 91\n    safety-critical: 17\n  human_in_the_loop_required: 17\noperations:\n- path: /listings\n  method: get\n  operationId: getListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{slug}\n  method: get\n  operationId: getListingsBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /places\n  method: get\n  operationId: getPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources\n  method: get\n  operationId: getSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{slug}\n  method: get\n  operationId: getProductsBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product-categories\n  method: get\n  operationId: getProductCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /academy/courses\n  method: get\n  operationId: getAcademyCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /academy/courses/{slug}\n  method: get\n  operationId: getAcademyCoursesBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /certificates/{code}\n  method: get\n\
  \  operationId: getCertificatesByCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/backlinks/export\n  method: get\n  operationId: getAdminBacklinksExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/test-sends\n  method: post\n  operationId: postAdminTestSends\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/voice/preview\n  method: post\n  operationId: postAdminVoicePreview\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/agent-runs\n  method: get\n  operationId: getAdminAgentRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/agent-runs\n  method: post\n  operationId: postAdminAgentRuns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/agent-runs/{id}\n  method: patch\n  operationId: patchAdminAgentRunsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/apps/{slug}\n  method: put\n  operationId: putAdminAppsBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/apps/{slug}\n  method: delete\n  operationId: deleteAdminAppsBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/audit-log\n  method: get\n  operationId: getAdminAuditLog\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/backup/export\n  method: post\n  operationId: postAdminBackupExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/backup/status\n  method: get\n  operationId: getAdminBackupStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/categories/{slug}\n  method: put\n  operationId: putAdminCategoriesBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /admin/categories/{slug}\n  method: delete\n  operationId: deleteAdminCategoriesBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/billing/subscriptions\n  method: get\n  operationId: getAdminBillingSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/billing/subscriptions/{id}\n  method: patch\n  operationId: patchAdminBillingSubscriptionsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /admin/billing/invoices\n  method: get\n  operationId: getAdminBillingInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/billing/invoices/{id}/refund\n  method: post\n  operationId: postAdminBillingInvoicesByIdRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/billing/retry\n  method: post\n  operationId: postAdminBillingRetry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/claims/{id}\n  method: post\n  operationId: postAdminClaimsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/claims/{id}\n  method: delete\n  operationId: deleteAdminClaimsById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/listings/{id}/owner\n  method: post\n  operationId: postAdminListingsByIdOwner\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{id}/owner\n  method: delete\n  operationId: deleteAdminListingsByIdOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/claims\n  method: get\n  operationId: getAdminClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/guides\n  method: get\n  operationId: getAdminGuides\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/guides\n  method: post\n  operationId: postAdminGuides\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/guides/{slug}\n  method: get\n  operationId: getAdminGuidesBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/guides/{slug}\n  method: put\n  operationId: putAdminGuidesBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /admin/guides/{slug}\n  method: patch\n  operationId: patchAdminGuidesBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/guides/{slug}\n  method: delete\n  operationId: deleteAdminGuidesBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/crm/export\n  method: get\n  operationId: getAdminCrmExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/crm/{id}\n  method:\
  \ patch\n  operationId: patchAdminCrmById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/crm/{id}\n  method: post\n  operationId: postAdminCrmById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/crm/{id}\n  method: delete\n  operationId: deleteAdminCrmById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /admin/edits/{id}\n  method: post\n  operationId: postAdminEditsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/enrichment/requests\n  method: get\n  operationId: getAdminEnrichmentRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/enrichment/requests/{id}\n  method: patch\n  operationId: patchAdminEnrichmentRequestsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /admin/ads/campaigns\n  method: post\n  operationId: postAdminAdsCampaigns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/ads/campaigns/{id}/status\n  method: post\n  operationId: postAdminAdsCampaignsByIdStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/enrichment/run\n  method: post\n  operationId: postAdminEnrichmentRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/enrichment/runs\n  method: get\n  operationId: getAdminEnrichmentRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/forms/export.csv\n  method: get\n  operationId: getAdminFormsExportCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/mail\n  method: post\n  operationId: postAdminMail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/mail/recent\n  method: get\n \
  \ operationId: getAdminMailRecent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/support/tickets\n  method: get\n  operationId: getAdminSupportTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/support/canned\n  method: get\n  operationId: getAdminSupportCanned\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/support/refund\n  method: post\n  operationId: postAdminSupportRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /admin/support/takedown\n  method: post\n  operationId: postAdminSupportTakedown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/support/legal\n  method: post\n  operationId: postAdminSupportLegal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/support/requests\n  method: get\n  operationId: getAdminSupportRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /admin/support/tickets/{id}\n  method: patch\n  operationId: patchAdminSupportTicketsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/support/tickets/{id}/escalate\n  method: post\n  operationId: postAdminSupportTicketsByIdEscalate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/support/tickets/{id}/reply\n  method: post\n  operationId: postAdminSupportTicketsByIdReply\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/mail/{messageId}/attachments/{attachmentId}\n  method: get\n  operationId: getAdminMailByMessageIdAttachmentsByAttachmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/monitoring/alerts\n  method: get\n  operationId: getAdminMonitoringAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/monitoring/sites\n  method: get\n  operationId: getAdminMonitoringSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /admin/domains/{domain}/status\n  method: get\n  operationId: getAdminDomainsByDomainStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/domains/{domain}/verify\n  method: post\n  operationId: postAdminDomainsByDomainVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/leads/dispatch\n  method: post\n  operationId: postAdminLeadsDispatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n   \
  \   human-in-the-loop: required\n    audit: required\n- path: /admin/leads/drips\n  method: post\n  operationId: postAdminLeadsDrips\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/leads/{id}\n  method: post\n  operationId: postAdminLeadsById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/leads/kb\n  method: post\n  operationId: postAdminLeadsKb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/leads/reconcile\n  method: get\n  operationId: getAdminLeadsReconcile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/leads/scripts\n  method: post\n  operationId: postAdminLeadsScripts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/leads/templates\n  method: post\n  operationId: postAdminLeadsTemplates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/link-exchanges\n  method: get\n  operationId: getAdminLinkExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/link-exchanges/{id}\n  method: get\n  operationId: getAdminLinkExchangesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/link-exchanges/{id}\n  method: post\n  operationId: postAdminLinkExchangesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /admin/listings\n  method: get\n  operationId: getAdminListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{slug}\n  method: get\n  operationId: getAdminListingsBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{slug}\n  method: delete\n  operationId: deleteAdminListingsBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}\n  method: patch\n  operationId: patchAdminListingsBySlug\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}\n  method: put\n  operationId: putAdminListingsBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/listings/{slug}\n  method: post\n  operationId: postAdminListingsBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /admin/listings/bulk\n  method: post\n  operationId: postAdminListingsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/photos\n  method: get\n  operationId: getAdminListingsBySlugPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{slug}/photos\n  method: post\n  operationId: postAdminListingsBySlugPhotos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/photos\n\
  \  method: patch\n  operationId: patchAdminListingsBySlugPhotos\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/photos/{photoId}\n  method: patch\n  operationId: patchAdminListingsBySlugPhotosByPhotoId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/photos/{photoId}\n  method: delete\n  operationId: deleteAdminListingsBySlugPhotosByPhotoId\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/reviews\n  method: get\n  operationId: getAdminListingsBySlugReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{slug}/reviews\n  method: post\n  operationId: postAdminListingsBySlugReviews\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/reviews/{rowId}\n  method: get\n\
  \  operationId: getAdminListingsBySlugReviewsByRowId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{slug}/reviews/{rowId}\n  method: patch\n  operationId: patchAdminListingsBySlugReviewsByRowId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/reviews/{rowId}\n  method: delete\n  operationId: deleteAdminListingsBySlugReviewsByRowId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /admin/listings/{slug}/reviews/{rowId}/publish\n  method: post\n  operationId: postAdminListingsBySlugReviewsByRowIdPublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/reviews/{rowId}/reject\n  method: post\n  operationId: postAdminListingsBySlugReviewsByRowIdReject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/source-photos\n  method: get\n  operationId: getAdminListingsBySlugSourcePhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{slug}/source-photos\n  method: patch\n  operationId: patchAdminListingsBySlugSourcePhotos\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/source-photos/{rowId}\n  method: get\n  operationId: getAdminListingsBySlugSourcePhotosByRowId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{slug}/source-photos/{rowId}\n  method: patch\n  operationId: patchAdminListingsBySlugSourcePhotosByRowId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/source-photos/{rowId}\n  method: delete\n  operationId: deleteAdminListingsBySlugSourcePhotosByRowId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{slug}/source-reviews\n  method: get\n  operationId: getAdminListingsBySlugSourceReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (67 KB total) ---\n# Full source: https://artifacts.apis.io/dishdirectory-com/agentic-access/dishdirectory-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/dishdirectory-com/agentic-access/dishdirectory-com-agentic-access.yml
summary_line: 219 operations · 134 acting · 17 human-in-the-loop
tags:
- Restaurant
- Food
- Data
- Listings
- Discovery
---
