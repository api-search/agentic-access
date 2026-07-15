---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 24
api_specs:
- filename: wm-openapi.yml
  format: yaml
  label: WM Services API
  slug: wm-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Service Operations & Materials API
  slug: wm-service-operations-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Service Pricing API
  slug: wm-service-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Invoices & Balance API
  slug: wm-invoices-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Profiles & Preferences API
  slug: wm-profiles-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Contacts API
  slug: wm-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Cases & Tickets API
  slug: wm-cases-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Activities API
  slug: wm-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
consequence_counts:
  read: 24
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wm Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'WM exposes 27 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WM
provider_slug: wm
slug: wm-agentic-access
source_filename: wm-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wm-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 24\n    acting: 3\n  by_consequence:\n    read: 24\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /customers/{customerId}/services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/services/plan\n  method: get\n  operationId: getServicePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /customers/{customerId}/services/stats\n  method: get\n  operationId: getServiceStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/services/next-pickup\n  method: get\n  operationId: getNextPickup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/services/{serviceId}/eta\n  method: get\n  operationId: getServiceEta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/services/operations\n  method: get\n  operationId: listServiceOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/services/materials\n\
  \  method: get\n  operationId: listServiceMaterials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/services/prices\n  method: get\n  operationId: listServicePrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/services/prices/invoice-fees\n  method: get\n  operationId: listInvoiceFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/invoices/{invoiceId}\n  method: get\n\
  \  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/profiles\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/communication-preferences\n  method: get\n  operationId: getCommunicationPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/communication-preferences\n  method: put\n  operationId: updateCommunicationPreferences\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /preferences/categories\n  method: get\n  operationId: listPreferenceCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/contacts/billing\n  method: get\n  operationId: getBillingContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/contacts/billing\n\
  \  method: put\n  operationId: updateBillingContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/contacts/service\n  method: put\n  operationId: updateServiceContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/cases\n  method: get\n  operationId: listCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/cases/{caseId}\n  method: get\n \
  \ operationId: getCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/tickets\n  method: get\n  operationId: listTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/tickets/{ticketId}\n  method: get\n  operationId: getTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/activities/notes\n  method: get\n  operationId: listNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/activities/email\n  method: get\n  operationId: listEmailActivity\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/activities/issues\n  method: get\n  operationId: listIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/agentic-access/wm-agentic-access.yml
summary_line: 27 operations · 3 acting
tags:
- Waste Management
- Recycling
- Environmental Services
- Field Services
- Logistics
- Account Management
- Enterprise
- B2B
---
