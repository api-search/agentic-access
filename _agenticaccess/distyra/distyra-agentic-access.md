---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 24
api_specs:
- filename: distyra-authentication-api-openapi.yml
  format: yaml
  label: Brightfield Software Authentication API
  slug: distyra-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-authentication-api-openapi.yml
- filename: distyra-billing-api-openapi.yml
  format: yaml
  label: Brightfield Software Billing API
  slug: distyra-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-billing-api-openapi.yml
- filename: distyra-catalog-api-openapi.yml
  format: yaml
  label: Brightfield Software Catalog API
  slug: distyra-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-catalog-api-openapi.yml
- filename: distyra-connect-api-openapi.yml
  format: yaml
  label: Brightfield Software Connect API
  slug: distyra-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-connect-api-openapi.yml
- filename: distyra-enrichment-api-openapi.yml
  format: yaml
  label: Brightfield Software Enrichment API
  slug: distyra-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-enrichment-api-openapi.yml
- filename: distyra-feedback-api-openapi.yml
  format: yaml
  label: Brightfield Software Feedback API
  slug: distyra-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-feedback-api-openapi.yml
- filename: distyra-system-api-openapi.yml
  format: yaml
  label: Brightfield Software System API
  slug: distyra-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-system-api-openapi.yml
- filename: distyra-underwriting-api-openapi.yml
  format: yaml
  label: Brightfield Software Underwriting API
  slug: distyra-underwriting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-underwriting-api-openapi.yml
- filename: distyra-webhooks-api-openapi.yml
  format: yaml
  label: Brightfield Software Webhooks API
  slug: distyra-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-webhooks-api-openapi.yml
consequence_counts:
  read: 24
  safety-critical: 3
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Distyra Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/connect/connections/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/connect/connections/{id}/revoke-link
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/underwrite/collection-links/{id}
operation_count: 50
overview: 'Brightfield Software exposes 50 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 23 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Brightfield Software
provider_slug: distyra
slug: distyra-agentic-access
source_filename: distyra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: generated\nsource: openapi/distyra-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    connected: 24\n    acting: 26\n  by_consequence:\n    read: 24\n    write: 23\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/coverage\n  method: get\n  operationId: connectCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrich\n\
  \  method: post\n  operationId: enrichSingle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrich/batch\n  method: post\n  operationId: enrichBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/analyze\n  method: post\n  operationId: analyzeApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/underwrite/analyze/statement\n  method: post\n  operationId: analyzeApplicantFromStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/analyze/statement/async\n  method: post\n  operationId: analyzeApplicantFromStatementAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/analyze/statement/async/{id}\n  method: get\n  operationId: analyzeApplicantFromStatementAsyncStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/underwrite/analyze/statement/parsed\n  method: post\n  operationId: analyzeApplicantFromParsedStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/analyze/statement/parsed/async\n  method: post\n  operationId: analyzeApplicantFromParsedStatementAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/feedback\n  method: post\n  operationId: submitUnderwritingFeedback\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/analyses/{id}\n  method: get\n  operationId: getUnderwritingAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/underwrite/analyses/{id}/report\n  method: get\n  operationId: getUnderwritingAnalysisReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/underwrite/analyses\n  method: get\n  operationId: listUnderwritingAnalyses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/underwrite/ingest\n  method: post\n\
  \  operationId: ingestStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/ingest/batch\n  method: post\n  operationId: ingestStatementBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/ingestions/{id}\n  method: get\n  operationId: getIngestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/underwrite/ingestions\n  method: get\n  operationId: listIngestions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/underwrite/collection-links\n  method: post\n  operationId: createCollectionLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/collection-links\n  method: get\n  operationId: listCollectionLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/underwrite/collection-links/{id}\n  method: get\n  operationId: getCollectionLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/underwrite/collection-links/{id}\n\
  \  method: delete\n  operationId: revokeCollectionLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/underwrite/collection-links/{id}/files\n  method: post\n  operationId: stageCollectionFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/underwrite/collection-links/{id}/finish-analyze\n  method: post\n  operationId: finishCollectionAnalyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/invoices/{id}/pdf\n  method: get\n  operationId: getBillingInvoicePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/payments/{paymentId}\n  method: get\n  operationId: getBillingPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enrich/batch/async\n  method: post\n  operationId: enrichBatchAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrich/batch/async/{id}\n\
  \  method: get\n  operationId: enrichBatchAsyncStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchants/{id}\n  method: get\n  operationId: getMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback/correction\n  method: post\n  operationId: submitCorrection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/feedback/confirmation\n  method: post\n  operationId: submitConfirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_endpoints\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook_endpoints/{id}\n  method: get\n\
  \  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook_endpoints/{id}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_endpoints/{id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_endpoints/{id}/rotate_secret\n  method: post\n  operationId:\
  \ rotateWebhookEndpointSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook_deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/aspsps\n  method: get\n  operationId: listAspsps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect/connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/connections/{id}\n  method: get\n  operationId: getConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/connections/{id}\n  method: delete\n  operationId: revokeConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/connect/connections/{id}/accounts\n\
  \  method: get\n  operationId: getConnectionAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/connections/{id}/identity\n  method: get\n  operationId: getConnectionIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/connections/{id}/transactions\n  method: get\n  operationId: getConnectionTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect/connections/{id}/revoke-link\n  method: post\n  operationId: createConnectionRevokeLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/connect/hosted-link\n  method: post\n  operationId: createHostedConnectLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/rotate\n  method: post\n  operationId: rotateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/agentic-access/distyra-agentic-access.yml
summary_line: 50 operations · 26 acting · 3 human-in-the-loop
tags:
- Company
- Banking
- API
- Fintech
- European
---
