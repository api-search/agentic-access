---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 17
api_specs:
- filename: zayo-maintenance-cases-api-openapi.yml
  format: yaml
  label: Zayo Maintenance Cases API
  slug: zayo-maintenance-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-maintenance-cases-api-openapi.yml
- filename: zayo-network-discovery-api-openapi.yml
  format: yaml
  label: Zayo Network Discovery API
  slug: zayo-network-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-network-discovery-api-openapi.yml
- filename: zayo-order-api-openapi.yml
  format: yaml
  label: Zayo Order API
  slug: zayo-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-order-api-openapi.yml
- filename: zayo-product-catalog-api-openapi.yml
  format: yaml
  label: Zayo Product Catalog API
  slug: zayo-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-product-catalog-api-openapi.yml
- filename: zayo-quote-api-openapi.yml
  format: yaml
  label: Zayo Quote API
  slug: zayo-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-quote-api-openapi.yml
- filename: zayo-service-inventory-api-openapi.yml
  format: yaml
  label: Zayo Service Inventory API
  slug: zayo-service-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-service-inventory-api-openapi.yml
- filename: zayo-ticket-catalog-api-openapi.yml
  format: yaml
  label: Zayo Ticket Catalog API
  slug: zayo-ticket-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-ticket-catalog-api-openapi.yml
- filename: zayo-ticketing-api-openapi.yml
  format: yaml
  label: Zayo Ticketing API
  slug: zayo-ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/openapi/zayo-ticketing-api-openapi.yml
consequence_counts:
  physical: 3
  read: 17
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zayo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /services/notifications/v1/send-test-notification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /services/order-management/v2/orders/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /services/service-management/v1/customer-ticket-action
operation_count: 26
overview: 'Zayo exposes 26 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 6 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zayo
provider_slug: zayo
slug: zayo-agentic-access
source_filename: zayo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/zayo-maintenance-cases-api-openapi.yml, openapi/zayo-network-discovery-api-openapi.yml,\n  openapi/zayo-order-api-openapi.yml, openapi/zayo-product-catalog-api-openapi.yml, openapi/zayo-quote-api-openapi.yml,\n  openapi/zayo-service-inventory-api-openapi.yml, openapi/zayo-ticket-catalog-api-openapi.yml,\n  openapi/zayo-ticketing-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 17\n    acting: 9\n  by_consequence:\n    read: 17\n    write: 6\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /services/service-management/v1/maintenance-cases\n  method: post\n  operationId: getMaintenanceCases\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/service-management/v1/maintenance-impacts\n  method: post\n  operationId: getMaintenanceImpacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/service-management/v1/maintenance-cases/{caseNumber}/notifications\n  method: get\n  operationId: getMaintenanceNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/service-management/v1/maintenance-cases/notifications/{maintenanceNotificationName}\n  method: get\n  operationId: getMaintenanceNotificationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /services/notifications/v1/generate-auth-token\n  method: post\n  operationId: generateAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/notifications/v1/register-callback-url\n  method: post\n  operationId: registerCallbackUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/notifications/v1/send-test-notification\n  method: post\n  operationId: sendTestNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/location-management/v2/buildings/validation\n  method: post\n  operationId: validateBuildings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/location-management/v2/building/{buildingId}/locations\n  method: get\n  operationId: getLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/quote-management/v2/sites/available-cloud-providers\n  method: post\n  operationId: getCloudSites\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/order-management/v2/orders/contacts/{quoteId}\n  method: get\n  operationId: getOrderContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/order-management/v2/orders/order\n  method: post\n  operationId: submitOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/order-management/v2/job/{jobId}\n  method: get\n  operationId: getJobDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/quote-management/v3/catalog/product-code\n  method: get\n  operationId: getProductCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/quote-management/v3/catalog/product-code-details/{productCode}/{version}\n  method: get\n  operationId: getProductCodeDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/quote-management/v3/quotes/quote\n  method: post\n  operationId: requestQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/quote-management/v3/quotes/quote/{quoteId}\n\
  \  method: get\n  operationId: getQuoteDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/quote-management/v2/quotes/nnis\n  method: post\n  operationId: getNNIs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/service-management/v1/existing-services\n  method: post\n  operationId: getservices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/service-management/v1/ticket-catalog\n  method: get\n  operationId: getTicketCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/service-management/v1/ticket-type-details/{ticketType}/{version}\n\
  \  method: get\n  operationId: getTicketTypeDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/service-management/v1/create-ticket\n  method: post\n  operationId: createTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/service-management/v1/ticket-comment\n  method: post\n  operationId: addTicketComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/service-management/v1/ticket-details/{ticketName}\n\
  \  method: get\n  operationId: getTicketDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/service-management/v1/all-tickets\n  method: post\n  operationId: getAllTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/service-management/v1/customer-ticket-action\n  method: post\n  operationId: customerTicketAction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zayo/refs/heads/main/agentic-access/zayo-agentic-access.yml
summary_line: 26 operations · 9 acting
tags:
- Company
- Telecommunications
- Networking
- Connectivity
- Fiber
- Infrastructure
- Bandwidth
- Cloud Connectivity
- Ordering
- Ticketing
---
