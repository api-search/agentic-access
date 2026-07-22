---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 23
api_specs:
- filename: sibill-openapi-original.json
  format: json
  label: Sibill Integration API
  slug: sibill-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-openapi-original.json
consequence_counts:
  read: 23
  safety-critical: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 25
kind: agentic-access
layout: agentic-access
method: generated
name: Sibill Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/categories
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/companies/{company_id}/categories/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/companies/{company_id}/categories/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/counterparts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/companies/{company_id}/counterparts/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/document-sectionals
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/companies/{company_id}/document-sectionals/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/documents/invoice
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/documents/{document_id}/flows
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/companies/{company_id}/documents/{document_id}/flows/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/companies/{company_id}/documents/{document_id}/flows/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/documents/{document_id}/share-invoice
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/companies/{company_id}/documents/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/companies/{company_id}/documents/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/products
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/companies/{company_id}/products/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/companies/{company_id}/products/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/reconciliations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/companies/{company_id}/reconciliations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/requests/bulk-payment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/requests/f24/ocr
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/companies/{company_id}/subcategories
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/companies/{company_id}/subcategories/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/companies/{company_id}/subcategories/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/companies/{company_id}/transactions/{id}
operation_count: 48
overview: 'Sibill exposes 48 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 25 safety-critical.


  25 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sibill
provider_slug: sibill
slug: sibill-agentic-access
source_filename: sibill-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/sibill-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 23\n    acting: 25\n  by_consequence:\n    read: 23\n    safety-critical: 25\n  human_in_the_loop_required: 25\noperations:\n- path: /api/v1/companies\n  method: get\n  operationId: SibillWeb.Integration.V1.CompaniesController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/accounts\n  method: get\n  operationId: SibillWeb.Integration.V1.AccountsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/accounts/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.AccountsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/categories\n  method: get\n  operationId: SibillWeb.Integration.V1.CategoriesController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/categories\n  method: post\n  operationId: SibillWeb.Integration.V1.CategoriesController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/categories/{id}\n  method: delete\n  operationId: SibillWeb.Integration.V1.CategoriesController.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/categories/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.CategoriesController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/categories/{id}\n  method: patch\n  operationId: SibillWeb.Integration.V1.CategoriesController.update\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/counterparts\n  method: get\n  operationId: SibillWeb.Integration.V1.CounterpartsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/counterparts\n  method: post\n  operationId: SibillWeb.Integration.V1.CounterpartsController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /api/v1/companies/{company_id}/counterparts/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.CounterpartsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/counterparts/{id}\n  method: patch\n  operationId: SibillWeb.Integration.V1.CounterpartsController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/document-sectionals\n  method: get\n  operationId: SibillWeb.Integration.V1.DocumentSectionalsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/document-sectionals\n  method: post\n  operationId: SibillWeb.Integration.V1.DocumentSectionalsController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/document-sectionals/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.DocumentSectionalsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/document-sectionals/{id}\n  method: patch\n  operationId: SibillWeb.Integration.V1.DocumentSectionalsController.update\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/documents\n  method: get\n  operationId: SibillWeb.Integration.V1.DocumentsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/documents/invoice\n  method: post\n  operationId: SibillWeb.Integration.V1.DocumentsActionsController.create_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/v1/companies/{company_id}/documents/{document_id}/flows\n  method: get\n  operationId: SibillWeb.Integration.V1.FlowsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/documents/{document_id}/flows\n  method: post\n  operationId: SibillWeb.Integration.V1.FlowsController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/documents/{document_id}/flows/{id}\n  method: delete\n  operationId: SibillWeb.Integration.V1.FlowsController.delete\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/documents/{document_id}/flows/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.FlowsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/documents/{document_id}/flows/{id}\n  method: patch\n  operationId: SibillWeb.Integration.V1.FlowsController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/v1/companies/{company_id}/documents/{document_id}/invoice\n  method: get\n  operationId: SibillWeb.Integration.V1.DocumentsActionsController.get_invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/documents/{document_id}/share-invoice\n  method: post\n  operationId: SibillWeb.Integration.V1.DocumentsActionsController.share_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/documents/{id}\n  method: delete\n  operationId: SibillWeb.Integration.V1.DocumentsController.delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/documents/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.DocumentsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/documents/{id}\n  method: patch\n  operationId: SibillWeb.Integration.V1.DocumentsController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /api/v1/companies/{company_id}/products\n  method: get\n  operationId: SibillWeb.Integration.V1.ProductsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/products\n  method: post\n  operationId: SibillWeb.Integration.V1.ProductsController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/products/{id}\n  method: delete\n  operationId: SibillWeb.Integration.V1.ProductsController.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/products/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.ProductsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/products/{id}\n  method: patch\n  operationId: SibillWeb.Integration.V1.ProductsController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/reconciliations\n  method: get\n  operationId:\
  \ SibillWeb.Integration.V1.ReconciliationsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/reconciliations\n  method: post\n  operationId: SibillWeb.Integration.V1.ReconciliationsController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/reconciliations/{id}\n  method: delete\n  operationId: SibillWeb.Integration.V1.ReconciliationsController.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n  \
  \    purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/reconciliations/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.ReconciliationsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/requests/bulk-payment\n  method: post\n  operationId: SibillWeb.Integration.V1.RequestsController.bulk_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/requests/f24/ocr\n  method: post\n  operationId: SibillWeb.Integration.V1.RequestsController.f24_ocr\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/subcategories\n  method: get\n  operationId: SibillWeb.Integration.V1.SubcategoriesController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/subcategories\n  method: post\n  operationId: SibillWeb.Integration.V1.SubcategoriesController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/subcategories/{id}\n  method: delete\n  operationId: SibillWeb.Integration.V1.SubcategoriesController.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/subcategories/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.SubcategoriesController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/subcategories/{id}\n  method: patch\n  operationId: SibillWeb.Integration.V1.SubcategoriesController.update\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/companies/{company_id}/transactions\n  method: get\n  operationId: SibillWeb.Integration.V1.TransactionsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/transactions/{id}\n  method: get\n  operationId: SibillWeb.Integration.V1.TransactionsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{company_id}/transactions/{id}\n  method: patch\n  operationId: SibillWeb.Integration.V1.TransactionsController.update\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/counterparts/search\n  method: get\n  operationId: SibillWeb.Integration.V1.CounterpartsActionsController.search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/agentic-access/sibill-agentic-access.yml
summary_line: 48 operations · 25 acting · 25 human-in-the-loop
tags:
- Company
- Fintech
- Invoicing
- Payments
- Reconciliation
- Accounting
- Banking
- SME
- Open Banking
- Electronic Invoicing
- Italy
---
