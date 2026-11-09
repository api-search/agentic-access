---
acting_count: 82
action_class_counts:
  acting: 82
  connected: 47
api_specs:
- filename: adhdevaluations-fyi-admin-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Admin API
  slug: adhdevaluations-fyi-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-admin-api-openapi.yml
- filename: adhdevaluations-fyi-categories-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Categories API
  slug: adhdevaluations-fyi-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-categories-api-openapi.yml
- filename: adhdevaluations-fyi-listings-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Listings API
  slug: adhdevaluations-fyi-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-listings-api-openapi.yml
- filename: adhdevaluations-fyi-places-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Places API
  slug: adhdevaluations-fyi-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-places-api-openapi.yml
- filename: adhdevaluations-fyi-sources-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Sources API
  slug: adhdevaluations-fyi-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-sources-api-openapi.yml
- filename: adhdevaluations-fyi-stats-api-openapi.yml
  format: yaml
  label: ADHDEvaluations Stats API
  slug: adhdevaluations-fyi-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adhdevaluations-fyi/openapi/adhdevaluations-fyi-stats-api-openapi.yml
consequence_counts:
  physical: 18
  read: 47
  safety-critical: 10
  write: 54
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Adhdevaluations Fyi Agentic Access
name_suffix: Agentic Access
notable_actions:
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
  path: /admin/billing/retry
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/leads/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /admin/listings/{id}/photos
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /admin/listings/{id}/photos/{photoId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/mail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/moderation/ban
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/newsletter/campaigns/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/outreach/campaigns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/outreach/messages/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/outreach/reconcile
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/outreach/targets/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/support/tickets/{id}/escalate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/support/tickets/{id}/reply
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/test-sends
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/users
operation_count: 129
overview: 'ADHDEvaluations exposes 129 API operations that an AI agent could call, of which 82 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 47 read, 54 write, 18 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ADHDEvaluations
provider_slug: adhdevaluations-fyi
slug: adhdevaluations-fyi-agentic-access
source_filename: adhdevaluations-fyi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/adhdevaluations-fyi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 129\n  by_action_class:\n    connected: 47\n    acting: 82\n  by_consequence:\n    read: 47\n    physical: 18\n    write: 54\n    safety-critical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /listings\n  method: get\n  operationId: getListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{slug}\n  method: get\n  operationId: getListingsBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /places\n  method: get\n  operationId: getPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources\n  method: get\n  operationId: getSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/backlinks/export\n  method: get\n  operationId: getAdminBacklinksExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/test-sends\n  method: post\n  operationId: postAdminTestSends\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/voice/preview\n  method: post\n  operationId: postAdminVoicePreview\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/agent-runs\n  method: get\n  operationId: getAdminAgentRuns\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/agent-runs\n  method: post\n  operationId: postAdminAgentRuns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/agent-runs/{id}\n  method: patch\n  operationId: patchAdminAgentRunsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/apps/{slug}\n  method: put\n  operationId: putAdminAppsBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/apps/{slug}\n  method: delete\n  operationId: deleteAdminAppsBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/audit-log\n  method: get\n  operationId: getAdminAuditLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/backup/export\n  method: post\n  operationId: postAdminBackupExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/backup/status\n  method: get\n  operationId: getAdminBackupStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/categories/{slug}\n  method: put\n  operationId: putAdminCategoriesBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/categories/{slug}\n  method: delete\n  operationId: deleteAdminCategoriesBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/billing/subscriptions\n  method: get\n  operationId: getAdminBillingSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/billing/subscriptions/{id}\n  method: patch\n  operationId: patchAdminBillingSubscriptionsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/billing/invoices\n  method: get\n  operationId: getAdminBillingInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/billing/invoices/{id}/refund\n\
  \  method: post\n  operationId: postAdminBillingInvoicesByIdRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/billing/retry\n  method: post\n  operationId: postAdminBillingRetry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/claims/{id}\n  method: post\n  operationId: postAdminClaimsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/claims/{id}\n  method: delete\n  operationId: deleteAdminClaimsById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/claims\n  method: get\n  operationId: getAdminClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/content/publish\n  method: post\n  operationId: postAdminContentPublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/guides\n  method: get\n  operationId: getAdminGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/guides\n  method: post\n  operationId: postAdminGuides\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/guides/{slug}\n  method: get\n  operationId: getAdminGuidesBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/guides/{slug}\n  method: put\n  operationId: putAdminGuidesBySlug\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/guides/{slug}\n  method: patch\n  operationId: patchAdminGuidesBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/guides/{slug}\n  method: delete\n  operationId: deleteAdminGuidesBySlug\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /admin/crm/export\n  method: get\n  operationId: getAdminCrmExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/crm/{id}\n  method: patch\n  operationId: patchAdminCrmById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/crm/{id}\n  method: post\n  operationId: postAdminCrmById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/crm/{id}\n  method: delete\n  operationId: deleteAdminCrmById\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/edits/{id}\n  method: post\n  operationId: postAdminEditsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/enrichment/requests\n  method: get\n  operationId: getAdminEnrichmentRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/enrichment/requests/{id}\n  method: patch\n  operationId: patchAdminEnrichmentRequestsById\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/ads/campaigns\n  method: post\n  operationId: postAdminAdsCampaigns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/ads/campaigns/{id}/status\n  method: post\n  operationId: postAdminAdsCampaignsByIdStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /admin/enrichment/run\n  method: post\n  operationId: postAdminEnrichmentRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/enrichment/runs\n  method: get\n  operationId: getAdminEnrichmentRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/forms/export.csv\n  method: get\n  operationId: getAdminFormsExportCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/mail\n  method: post\n  operationId: postAdminMail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/mail/recent\n  method: get\n  operationId: getAdminMailRecent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/support/tickets\n  method: get\n  operationId: getAdminSupportTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/support/tickets/{id}\n  method: patch\n  operationId: patchAdminSupportTicketsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /admin/support/tickets/{id}/escalate\n  method: post\n  operationId: postAdminSupportTicketsByIdEscalate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/support/tickets/{id}/reply\n  method: post\n  operationId: postAdminSupportTicketsByIdReply\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/mail/{messageId}/attachments/{attachmentId}\n\
  \  method: get\n  operationId: getAdminMailByMessageIdAttachmentsByAttachmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/monitoring/alerts\n  method: get\n  operationId: getAdminMonitoringAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/monitoring/sites\n  method: get\n  operationId: getAdminMonitoringSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/domains/{domain}/status\n  method: get\n  operationId: getAdminDomainsByDomainStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/domains/{domain}/verify\n  method: post\n\
  \  operationId: postAdminDomainsByDomainVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/leads/dispatch\n  method: post\n  operationId: postAdminLeadsDispatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/leads/drips\n  method: post\n  operationId: postAdminLeadsDrips\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/leads/{id}\n  method: post\n  operationId: postAdminLeadsById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/leads/kb\n  method: post\n  operationId: postAdminLeadsKb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/leads/reconcile\n  method: get\n  operationId: getAdminLeadsReconcile\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/leads/scripts\n  method: post\n  operationId: postAdminLeadsScripts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/leads/templates\n  method: post\n  operationId: postAdminLeadsTemplates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/link-exchanges/{id}\n  method: post\n  operationId: postAdminLinkExchangesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/bulk\n  method: post\n  operationId: postAdminListingsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{id}\n  method: post\n  operationId: postAdminListingsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{id}/photos\n  method: get\n  operationId: getAdminListingsByIdPhotos\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{id}/photos\n  method: post\n  operationId: postAdminListingsByIdPhotos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{id}/photos\n  method: patch\n  operationId: patchAdminListingsByIdPhotos\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{id}/photos/{photoId}\n\
  \  method: patch\n  operationId: patchAdminListingsByIdPhotosByPhotoId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{id}/photos/{photoId}\n  method: delete\n  operationId: deleteAdminListingsByIdPhotosByPhotoId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/moderation/queue\n  method: get\n  operationId: getAdminModerationQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /admin/moderation/{id}\n  method: patch\n  operationId: patchAdminModerationById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/moderation/ban\n  method: get\n  operationId: getAdminModerationBan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/moderation/ban\n  method: post\n  operationId: postAdminModerationBan\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /admin/moderation/ban\n  method: delete\n  operationId: deleteAdminModerationBan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/newsletter/api-keys\n  method: get\n  operationId: getAdminNewsletterApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/newsletter/api-keys\n  method: post\n  operationId: postAdminNewsletterApiKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /admin/newsletter/contacts\n  method: get\n  operationId: getAdminNewsletterContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/newsletter/contacts\n  method: post\n  operationId: postAdminNewsletterContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/newsletter/campaigns\n  method: get\n  operationId: getAdminNewsletterCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/newsletter/campaigns\n  method: post\n  operationId: postAdminNewsletterCampaigns\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/newsletter/campaigns/{id}\n  method: get\n  operationId: getAdminNewsletterCampaignsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/newsletter/campaigns/{id}\n  method: patch\n  operationId: patchAdminNewsletterCampaignsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/newsletter/campaigns/{id}\n  method: delete\n  operationId: deleteAdminNewsletterCampaignsById\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/newsletter/campaigns/{id}\n  method: post\n  operationId: postAdminNewsletterCampaignsById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/reports/leads\n  method: get\n  operationId: getAdminReportsLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/reports/revenue\n  method: get\n  operationId:\
  \ getAdminReportsRevenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/reports/traffic\n  method: get\n  operationId: getAdminReportsTraffic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/seo/audit\n  method: get\n  operationId: getAdminSeoAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/seo/indexnow\n  method: post\n  operationId: postAdminSeoIndexnow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/seo/resubmit-sitemap\n\
  \  method: post\n  operationId: postAdminSeoResubmitSitemap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/settings\n  method: get\n  operationId: getAdminSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/settings\n  method: put\n  operationId: putAdminSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/settings\n  method: delete\n  operationId: deleteAdminSettings\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/sources/{key}\n  method: put\n  operationId: putAdminSourcesByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/sources/{key}\n  method: delete\n  operationId: deleteAdminSourcesByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/submissions\n\
  \  method: get\n  operationId: getAdminSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/submissions/{id}\n  method: post\n  operationId: postAdminSubmissionsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/tokens\n  method: get\n  operationId: getAdminTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/tokens\n  method: post\n  operationId: postAdminTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/tokens/{id}\n  method: delete\n  operationId: deleteAdminTokensById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/outreach/messages/{id}\n  method: post\n  operationId: postAdminOutreachMessagesById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (39 KB total)\
  \ ---\n# Full source: https://artifacts.apis.io/adhdevaluations-fyi/agentic-access/adhdevaluations-fyi-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/adhdevaluations-fyi/agentic-access/adhdevaluations-fyi-agentic-access.yml
summary_line: 129 operations · 82 acting · 10 human-in-the-loop
tags:
- ADHD
- Healthcare
- Directory
- Evaluation
- Providers
---
