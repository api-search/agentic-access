---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: jithox-com-iban-api-openapi.yml
  format: yaml
  label: jithox-com Iban API
  slug: jithox-com-iban-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-iban-api-openapi.yml
- filename: jithox-com-invoice-api-openapi.yml
  format: yaml
  label: jithox-com Invoice API
  slug: jithox-com-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-invoice-api-openapi.yml
- filename: jithox-com-payment-api-openapi.yml
  format: yaml
  label: jithox-com Payment API
  slug: jithox-com-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-payment-api-openapi.yml
- filename: jithox-com-peppol-api-openapi.yml
  format: yaml
  label: jithox-com Peppol API
  slug: jithox-com-peppol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-peppol-api-openapi.yml
- filename: jithox-com-vat-api-openapi.yml
  format: yaml
  label: jithox-com Vat API
  slug: jithox-com-vat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-vat-api-openapi.yml
consequence_counts:
  physical: 2
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jithox Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/invoice/review
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payment/preflight
operation_count: 5
overview: 'jithox-com exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: jithox-com
provider_slug: jithox-com
slug: jithox-com-agentic-access
source_filename: jithox-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/jithox-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 2\n    read: 1\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/vat/verify\n  method: post\n  operationId: verifyVat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/peppol/participant\n  method: post\n  operationId: lookupPeppolParticipant\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/iban/verify\n  method: post\n  operationId: verifyIban\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payment/preflight\n  method: post\n  operationId: preflightPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/invoice/review\n  method: post\n  operationId: reviewInvoice\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/jithox-com/agentic-access/jithox-com-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- Company
- Artificial Intelligence
- Automation
- Back Office
- Tools
---
