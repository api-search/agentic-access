---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: dassault-accreditations-api-openapi.yml
  format: yaml
  label: Dassault Systèmes Accreditations API
  slug: dassault-accreditations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-accreditations-api-openapi.yml
- filename: dassault-leads-opportunities-api-openapi.yml
  format: yaml
  label: Dassault Systèmes Leads Opportunities API
  slug: dassault-leads-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-leads-opportunities-api-openapi.yml
- filename: dassault-orders-api-openapi.yml
  format: yaml
  label: Dassault Systèmes Orders API
  slug: dassault-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-orders-api-openapi.yml
- filename: dassault-portfolio-items-api-openapi.yml
  format: yaml
  label: Dassault Systèmes Portfolio Items API
  slug: dassault-portfolio-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-portfolio-items-api-openapi.yml
- filename: dassault-price-lists-api-openapi.yml
  format: yaml
  label: Dassault Systèmes Price Lists API
  slug: dassault-price-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-price-lists-api-openapi.yml
- filename: dassault-api-keys-api-openapi.yml
  format: yaml
  label: Dassault Systèmes API Keys API
  slug: dassault-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/openapi/dassault-api-keys-api-openapi.yml
consequence_counts:
  physical: 1
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dassault Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/api4partners/v0/apikeys
operation_count: 10
overview: 'Dassault Systèmes exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dassault Systèmes
provider_slug: dassault
slug: dassault-agentic-access
source_filename: dassault-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/dassault-accreditations-api-openapi.yml, openapi/dassault-api-keys-api-openapi.yml,\n  openapi/dassault-leads-opportunities-api-openapi.yml, openapi/dassault-orders-api-openapi.yml,\n  openapi/dassault-portfolio-items-api-openapi.yml, openapi/dassault-price-lists-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 7\n    acting: 3\n  by_consequence:\n    read: 7\n    physical: 1\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /order/api4partners/v0/accreditations/search\n  method: get\n  operationId: searchAccreditations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/api4partners/v0/apikeys\n  method: post\n  operationId: generateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sales/api4partners/v0/leads-opportunities\n  method: post\n  operationId: createLeadsOpportunities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sales/api4partners/v0/leads-opportunities/{id}\n  method: patch\n  operationId: updateLeadOpportunitiesDetails\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sales/api4partners/v0/leads-opportunities/{id}\n  method: get\n  operationId: getLeadsOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sales/api4partners/v0/leads-opportunities/search\n  method: post\n  operationId: searchLeadsOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/api4partners/v0/orders/search\n  method: post\n  operationId: searchOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /order/api4partners/v0/orders/{id}\n  method: get\n  operationId: getOrderDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sales/api4partners/v0/portfolio-items/search\n  method: get\n  operationId: searchPortfolioItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/api4partners/v0/price-lists/search\n  method: get\n  operationId: searchPriceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dassault/refs/heads/main/agentic-access/dassault-agentic-access.yml
summary_line: 10 operations · 3 acting
tags:
- 3DEXPERIENCE
- PLM
- CAD
- Manufacturing
- SolidWorks
- CATIA
- ENOVIA
- Engineering
- 3D Collaboration
---
