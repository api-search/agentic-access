---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 13
api_specs:
- filename: storecove-additionaltaxidentifiers-api-openapi.yml
  format: yaml
  label: Storecove Additional Tax Identifiers API
  slug: storecove-additionaltaxidentifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-additionaltaxidentifiers-api-openapi.yml
- filename: storecove-administrations-api-openapi.yml
  format: yaml
  label: Storecove Administrations API
  slug: storecove-administrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-administrations-api-openapi.yml
- filename: storecove-c5activation-api-openapi.yml
  format: yaml
  label: Storecove C5Activation API
  slug: storecove-c5activation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-c5activation-api-openapi.yml
- filename: storecove-discovery-api-openapi.yml
  format: yaml
  label: Storecove Discovery API
  slug: storecove-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-discovery-api-openapi.yml
- filename: storecove-invoicesubmissions-api-openapi.yml
  format: yaml
  label: Storecove Invoice Submissions API
  slug: storecove-invoicesubmissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-invoicesubmissions-api-openapi.yml
- filename: storecove-legalentities-api-openapi.yml
  format: yaml
  label: Storecove Legal Entities API
  slug: storecove-legalentities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-legalentities-api-openapi.yml
- filename: storecove-peppolidentifiers-api-openapi.yml
  format: yaml
  label: Storecove Peppol Identifiers API
  slug: storecove-peppolidentifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-peppolidentifiers-api-openapi.yml
- filename: storecove-purchaseinvoices-api-openapi.yml
  format: yaml
  label: Storecove Purchase Invoices API
  slug: storecove-purchaseinvoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-purchaseinvoices-api-openapi.yml
- filename: storecove-receiveddocuments-api-openapi.yml
  format: yaml
  label: Storecove Received Documents API
  slug: storecove-receiveddocuments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-receiveddocuments-api-openapi.yml
- filename: storecove-webhookinstances-api-openapi.yml
  format: yaml
  label: Storecove Webhook Instances API
  slug: storecove-webhookinstances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-webhookinstances-api-openapi.yml
- filename: storecove-document-submissions-api-openapi.yml
  format: yaml
  label: Storecove document submissions API
  slug: storecove-document-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/storecove/openapi/storecove-document-submissions-api-openapi.yml
consequence_counts:
  physical: 2
  read: 13
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Storecove Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice_submissions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice_submissions/preflight
operation_count: 40
overview: 'Storecove exposes 40 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 25 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Storecove
provider_slug: storecove
slug: storecove-agentic-access
source_filename: storecove-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/storecove-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    acting: 27\n    connected: 13\n  by_consequence:\n    write: 25\n    read: 13\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /legal_entities/{legal_entity_id}/additional_tax_identifiers\n  method: post\n  operationId: create_additional_tax_identifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities/{legal_entity_id}/additional_tax_identifiers/{id}\n\
  \  method: get\n  operationId: get_additional_tax_identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /legal_entities/{legal_entity_id}/additional_tax_identifiers/{id}\n  method: delete\n  operationId: delete_additional_tax_identifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities/{legal_entity_id}/additional_tax_identifiers/{id}\n  method: patch\n  operationId: update_additional_tax_identifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /legal_entities/{legal_entity_id}/administrations\n  method: post\n  operationId: create_administration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities/{legal_entity_id}/administrations/{id}\n  method: get\n  operationId: get_administration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /legal_entities/{legal_entity_id}/administrations/{id}\n  method: delete\n  operationId: delete_administration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities/{legal_entity_id}/administrations/{id}\n  method: patch\n  operationId: update_administration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/legal_entities/{legal_entity_id}/c5_activation/activate\n  method: post\n  operationId: create_c5_activation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/legal_entities/{legal_entity_id}/c5_deactivation/deactivate\n  method: post\n  operationId: create_c5_deactivation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/legal_entities/{legal_entity_id}/c5/iras/email/activate\n  method: post\n  operationId: create_c5_email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/legal_entities/{legal_entity_id}/c5/iras/email/deactivate\n  method: post\n  operationId: deactivate_c5_email\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/legal_entities/{legal_entity_id}/c5/iras/email/cancel\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/legal_entities/{legal_entity_id}/c5/iras/redirect/activate\n  method: post\n  operationId: activate_c5_redirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/legal_entities/{legal_entity_id}/c5/iras/redirect/deactivate\n  method: post\n  operationId: deactivate_c5_redirect\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/legal_entities/{legal_entity_id}/c5/iras/redirect/cancel\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery/receives\n  method: post\n  operationId: discovery_receives\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery/exists\n\
  \  method: post\n  operationId: discovery_exists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery/identifiers\n  method: get\n  operationId: discovery_identifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice_submissions/{guid}/evidence\n  method: get\n  operationId: show_invoice_submission_evidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice_submissions\n  method: post\n  operationId: create_invoice_submission\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_submissions\n  method: post\n  operationId: create_document_submission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document_submissions/{guid}/evidence\n  method: get\n  operationId: show_document_submission_evidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document_submissions/{guid}/evidence/{evidence_type}\n  method: get\n  operationId: show_document_submission_evidence_by_type\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice_submissions/preflight\n  method: post\n  operationId: preflight_invoice_recipient\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities\n  method: post\n  operationId: create_legal_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities/{id}\n  method: get\n  operationId: get_legal_entity\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /legal_entities/{id}\n  method: delete\n  operationId: delete_legal_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities/{id}\n  method: patch\n  operationId: update_legal_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purchase_invoices/{guid}\n  method: get\n  operationId: get_invoice_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchase_invoices/{guid}/{packaging}\n  method: get\n  operationId: get_invoice_ubl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchase_invoices/{guid}/{packaging}/{package_version}\n  method: get\n  operationId: get_invoice_ubl_versioned\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /legal_entities/{legal_entity_id}/peppol_identifiers\n  method: post\n  operationId: create_peppol_identifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities/{legal_entity_id}/peppol_identifiers/{superscheme}/{scheme}/{identifier}\n\
  \  method: patch\n  operationId: update_peppol_identifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities/{legal_entity_id}/peppol_identifiers/{superscheme}/{scheme}/{identifier}\n  method: delete\n  operationId: delete_peppol_identifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /legal_entities/{legal_entity_id}/received_documents\n  method: post\n  operationId: receive_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /received_documents/{guid}\n  method: get\n  operationId: get_received_document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /received_documents/{guid}/{format}\n  method: get\n  operationId: get_received_document_in_format\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook_instances/\n  method: get\n  operationId: get_webhook_instances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook_instances/{guid}\n  method: delete\n  operationId: delete_webhook_instance\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/storecove/agentic-access/storecove-agentic-access.yml
summary_line: 40 operations · 27 acting
tags:
- Company
- E-Invoicing
- PEPPOL
- Tax Compliance
- Invoicing
- Accounting
- ERP Integration
- Fintech
---
