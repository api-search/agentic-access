---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 18
api_specs:
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Clients API
  slug: repsly-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Representatives API
  slug: repsly-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Visits API
  slug: repsly-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Products API
  slug: repsly-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Forms API
  slug: repsly-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Photos API
  slug: repsly-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Pricelists API
  slug: repsly-pricelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Purchase Orders API
  slug: repsly-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Import and Export API
  slug: repsly-import-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
consequence_counts:
  physical: 1
  read: 18
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Repsly Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /import/sales-document-status
operation_count: 24
overview: 'Repsly exposes 24 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Repsly
provider_slug: repsly
slug: repsly-agentic-access
source_filename: repsly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/repsly-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 18\n    acting: 6\n  by_consequence:\n    read: 18\n    write: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /export/clients/{lastTimestamp}\n  method: get\n  operationId: exportClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/clientnotes/{lastClientNoteID}\n  method: get\n  operationId: exportClientNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /import/client\n  method: post\n  operationId: importClients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /export/representatives\n  method: get\n  operationId: exportRepresentatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/users\n  method: get\n  operationId: exportUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/dailyworkingtime/{lastDailyWorkingTimeID}\n  method: get\n  operationId: exportDailyWorkingTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/visits/{lastTimestamp}\n  method: get\n  operationId: exportVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/visitschedules/{beginDateTime}/{endDateTime}\n  method: get\n  operationId: exportVisitSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/visit-realizations\n  method: get\n  operationId: exportVisitRealizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /import/schedule\n  method: post\n  operationId: importSchedules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /export/products/{lastTimestamp}\n  method: get\n  operationId: exportProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/product-lists\n  method: get\n  operationId: exportProductLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/documentTypes/\n  method: get\n  operationId: exportDocumentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /import/product\n  method: post\n  operationId: importProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /import/package\n  method: post\n  operationId: importPackages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /export/retailaudits/{lastRetailAuditID}\n  method: get\n  operationId: exportRetailAudits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/forms/{lastFormID}\n  method: get\n  operationId: exportForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/photos/{lastPhotoID}\n\
  \  method: get\n  operationId: exportPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/pricelists/\n  method: get\n  operationId: exportPricelists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/pricelists/{pricelistID}\n  method: get\n  operationId: exportPricelistItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /import/pricelist\n  method: post\n  operationId: importPricelists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /export/purchaseorders/{lastDocumentID}\n  method: get\n  operationId: exportPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /import/sales-document-status\n  method: post\n  operationId: updateSalesDocumentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /export/importStatus/{importJobID}\n  method: get\n  operationId: getImportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/agentic-access/repsly-agentic-access.yml
summary_line: 24 operations · 6 acting
tags:
- Retail Execution
- Field Sales
- Merchandising
- CPG
- Retail Audits
- Sales Force Automation
---
