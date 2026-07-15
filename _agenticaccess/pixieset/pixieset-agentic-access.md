---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 19
api_specs:
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Clients & CRM API
  slug: pixieset-studio-clients-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Sessions & Booking API
  slug: pixieset-studio-sessions-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Invoices & Payments API
  slug: pixieset-studio-invoices-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Contracts API
  slug: pixieset-studio-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Gallery Collections & Delivery API
  slug: pixieset-gallery-collections-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
consequence_counts:
  read: 19
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pixieset Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Pixieset exposes 22 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pixieset
provider_slug: pixieset
slug: pixieset-agentic-access
source_filename: pixieset-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pixieset-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 19\n    acting: 3\n  by_consequence:\n    read: 19\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /clients/\n  method: get\n  operationId: listClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients/search\n  method: get\n  operationId: searchClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients/{client_id}\n  method: get\n \
  \ operationId: getClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients/{client_id}\n  method: put\n  operationId: updateClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session_types/\n  method: get\n  operationId: listSessionTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /session_types/\n  method: post\n  operationId: createSessionType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session_types/{session_type_id}/check-day-avail/{date_timezone}\n  method: get\n  operationId: checkDayAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoice_id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /invoices/invoice_summary\n  method: get\n  operationId: getInvoiceSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/payments/list/\n  method: get\n  operationId: listInvoicePayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/\n  method: get\n  operationId: listContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/contracts\n  method: get\n  operationId: listContractTemplates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/contracts/{template_id}\n  method: get\n  operationId: getContractTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/contracts/{template_id}\n  method: put\n  operationId: updateContractTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collection_id}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/galleries\n\
  \  method: get\n  operationId: listCollectionGalleries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/clients\n  method: get\n  operationId: listCollectionClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/downloads/\n  method: get\n  operationId: listCollectionDownloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/favorites\n  method: get\n  operationId: listCollectionFavorites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/agentic-access/pixieset-agentic-access.yml
summary_line: 22 operations · 3 acting
tags:
- Photography
- Client Galleries
- Studio Management
- CRM
- Booking
- Invoicing
- Contracts
- No Public API
---
