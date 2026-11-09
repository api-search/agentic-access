---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 9
api_specs:
- filename: attestwire-com-billing-api-openapi.yml
  format: yaml
  label: Attestwire Billing API
  slug: attestwire-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-billing-api-openapi.yml
- filename: attestwire-com-diagnose-api-openapi.yml
  format: yaml
  label: Attestwire Diagnose API
  slug: attestwire-com-diagnose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-diagnose-api-openapi.yml
- filename: attestwire-com-invoices-api-openapi.yml
  format: yaml
  label: Attestwire Invoices API
  slug: attestwire-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-invoices-api-openapi.yml
- filename: attestwire-com-keys-api-openapi.yml
  format: yaml
  label: Attestwire Keys API
  slug: attestwire-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-keys-api-openapi.yml
- filename: attestwire-com-meta-api-openapi.yml
  format: yaml
  label: Attestwire Meta API
  slug: attestwire-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-meta-api-openapi.yml
- filename: attestwire-com-peppol-api-openapi.yml
  format: yaml
  label: Attestwire Peppol API
  slug: attestwire-com-peppol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-peppol-api-openapi.yml
- filename: attestwire-com-recipient-api-openapi.yml
  format: yaml
  label: Attestwire Recipient API
  slug: attestwire-com-recipient-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-recipient-api-openapi.yml
- filename: attestwire-com-records-api-openapi.yml
  format: yaml
  label: Attestwire Records API
  slug: attestwire-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-records-api-openapi.yml
- filename: attestwire-com-vat-api-openapi.yml
  format: yaml
  label: Attestwire Vat API
  slug: attestwire-com-vat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestwire-com/openapi/attestwire-com-vat-api-openapi.yml
consequence_counts:
  physical: 8
  read: 9
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Attestwire Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/bundle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/diagnose
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/fix/claim
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/generate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/parse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/validate
operation_count: 21
overview: 'Attestwire exposes 21 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 4 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Attestwire
provider_slug: attestwire-com
slug: attestwire-com-agentic-access
source_filename: attestwire-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/attestwire-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 12\n    connected: 9\n  by_consequence:\n    physical: 8\n    read: 9\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/diagnose\n  method: post\n  operationId: diagnose_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/peppol/lookup\n  method: post\n \
  \ operationId: lookup_peppol_participant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vat/verify\n  method: post\n  operationId: verify_vat_vies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipient\n  method: post\n  operationId: get_recipient_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validate\n  method: post\n  operationId: validateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generate\n  method: post\n  operationId: generateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bundle\n  method: post\n  operationId: bundleInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/send\n  method: post\n  operationId:\
  \ sendInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/rotate\n  method: post\n  operationId: rotateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/checkout\n  method: get\n  operationId: checkoutStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/portal\n  method: get\n  operationId: getBillingPortal\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/portal\n  method: post\n  operationId: createBillingPortalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parse\n  method: post\n  operationId: parseInvoiceDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fix/claim\n  method: post\n  operationId: claimFixReport\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/records/{id}\n  method: get\n  operationId: getValidationRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/versions\n  method: get\n  operationId: versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/attestwire-signing-keys.json\n  method: get\n  operationId: signingKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/attestwire-com/agentic-access/attestwire-com-agentic-access.yml
summary_line: 21 operations · 12 acting
tags:
- Attestwire
- E-invoice
- Validation
- XRechnung
- PEPPOL
- MCP
---
