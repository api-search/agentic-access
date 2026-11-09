---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 16
api_specs:
- filename: wsystem-dev-billing-api-openapi.yml
  format: yaml
  label: wsystem-dev Billing API
  slug: wsystem-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-billing-api-openapi.yml
- filename: wsystem-dev-company-api-openapi.yml
  format: yaml
  label: wsystem-dev Company API
  slug: wsystem-dev-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-company-api-openapi.yml
- filename: wsystem-dev-e-invoice-api-openapi.yml
  format: yaml
  label: wsystem-dev E Invoice API
  slug: wsystem-dev-e-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-e-invoice-api-openapi.yml
- filename: wsystem-dev-eori-api-openapi.yml
  format: yaml
  label: wsystem-dev EORI API
  slug: wsystem-dev-eori-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-eori-api-openapi.yml
- filename: wsystem-dev-health-api-openapi.yml
  format: yaml
  label: wsystem-dev Health API
  slug: wsystem-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-health-api-openapi.yml
- filename: wsystem-dev-kyb-api-openapi.yml
  format: yaml
  label: wsystem-dev KYB API
  slug: wsystem-dev-kyb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-kyb-api-openapi.yml
- filename: wsystem-dev-sanctions-api-openapi.yml
  format: yaml
  label: wsystem-dev Sanctions API
  slug: wsystem-dev-sanctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-sanctions-api-openapi.yml
- filename: wsystem-dev-vat-api-openapi.yml
  format: yaml
  label: wsystem-dev VAT API
  slug: wsystem-dev-vat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wsystem-dev/openapi/wsystem-dev-vat-api-openapi.yml
consequence_counts:
  physical: 6
  read: 16
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Wsystem Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /einvoice/mandates/{mid}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /einvoice/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /einvoice/mandates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /einvoice/parse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /einvoice/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /einvoice/validate
operation_count: 28
overview: 'wsystem-dev exposes 28 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 5 write, 6 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: wsystem-dev
provider_slug: wsystem-dev
slug: wsystem-dev-agentic-access
source_filename: wsystem-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/wsystem-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 16\n    acting: 12\n  by_consequence:\n    read: 16\n    physical: 6\n    safety-critical: 1\n    write: 5\n  human_in_the_loop_required: 1\noperations:\n- path: /billing/plans\n  method: get\n  operationId: billingPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage\n  method: get\n  operationId: billingUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /billing/checkout\n  method: post\n  operationId: billingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einvoice/mandate-terms\n  method: get\n  operationId: einvoiceMandateTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einvoice/mandates\n  method: post\n  operationId: createPeppolMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /einvoice/mandates/{mid}\n  method: get\n  operationId: getPeppolMandate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einvoice/mandates/{mid}/revoke\n  method: post\n  operationId: revokePeppolMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vies/status\n  method: get\n  operationId: viesStatus\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify\n  method: get\n  operationId: verifyVat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/batch\n  method: post\n  operationId: verifyVatBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company\n  method: get\n  operationId: lookupCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/batch\n  method: post\n  operationId: lookupCompanyBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sanctions/screen\n  method: get\n  operationId: screenSanctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sanctions/screen/batch\n  method: post\n  operationId: screenSanctionsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kyb/check\n  method: post\n  operationId: kybCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eori\n \
  \ method: get\n  operationId: verifyEori\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eori/batch\n  method: post\n  operationId: verifyEoriBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einvoice/validate\n  method: post\n  operationId: validateEinvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einvoice/parse\n  method: post\n  operationId: parseEinvoice\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einvoice/create\n  method: post\n  operationId: createEinvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einvoice/route\n  method: get\n  operationId: einvoiceRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ddreport\n  method: post\n  operationId:\
  \ ddReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fr/pa-registry\n  method: get\n  operationId: frPaRegistry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einvoice/sample\n  method: get\n  operationId: einvoiceSample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einvoice/send\n  method: post\n  operationId: sendEinvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einvoice/evidence-key\n  method: get\n  operationId: einvoiceEvidenceKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einvoice/usage\n  method: get\n  operationId: einvoiceUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/wsystem-dev/agentic-access/wsystem-dev-agentic-access.yml
summary_line: 28 operations · 12 acting · 1 human-in-the-loop
tags:
- Company
- E-Invoicing
- European
- Compliance
---
