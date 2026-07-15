---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 23
api_specs:
- filename: servicenow-table-api-openapi.yml
  format: yaml
  label: ServiceNow Table API
  slug: servicenow-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-table-api-openapi.yml
- filename: servicenow-aggregate-api-openapi.yml
  format: yaml
  label: ServiceNow Aggregate API
  slug: servicenow-aggregate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-aggregate-api-openapi.yml
- filename: servicenow-attachment-api-openapi.yml
  format: yaml
  label: ServiceNow Attachment API
  slug: servicenow-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-attachment-api-openapi.yml
- filename: servicenow-import-set-api-openapi.yml
  format: yaml
  label: ServiceNow Import Set API
  slug: servicenow-import-set-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-import-set-api-openapi.yml
- filename: servicenow-change-management-api-openapi.yml
  format: yaml
  label: ServiceNow Change Management API
  slug: servicenow-change-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-change-management-api-openapi.yml
- filename: servicenow-service-catalog-api-openapi.yml
  format: yaml
  label: ServiceNow Service Catalog API
  slug: servicenow-service-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-service-catalog-api-openapi.yml
- filename: servicenow-cmdb-instance-api-openapi.yml
  format: yaml
  label: ServiceNow CMDB Instance API
  slug: servicenow-cmdb-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-cmdb-instance-api-openapi.yml
- filename: contact-api-openapi.yaml
  format: yaml
  label: ServiceNow Contact API
  slug: servicenow-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/contact-api-openapi.yaml
- filename: trouble-ticket-openapi.yaml
  format: yaml
  label: ServiceNow Trouble Ticket Open API
  slug: servicenow-trouble-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/trouble-ticket-openapi.yaml
- filename: servicenow-events-asyncapi.yml
  format: yaml
  label: ServiceNow Event Management Topic Open API
  slug: servicenow-event-management-topic-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/asyncapi/servicenow-events-asyncapi.yml
consequence_counts:
  physical: 2
  read: 23
  safety-critical: 1
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Servicenow Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /change/emergency
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /servicecatalog/cart/submit_order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /servicecatalog/items/{sys_id}/order_now
operation_count: 44
overview: 'ServiceNow exposes 44 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 18 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ServiceNow
provider_slug: servicenow
slug: servicenow-agentic-access
source_filename: servicenow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/contact-api-openapi.yaml, openapi/servicenow-aggregate-api-openapi.yml, openapi/servicenow-attachment-api-openapi.yml,\n  openapi/servicenow-change-management-api-openapi.yml, openapi/servicenow-cmdb-instance-api-openapi.yml,\n  openapi/servicenow-import-set-api-openapi.yml, openapi/servicenow-service-catalog-api-openapi.yml,\n  openapi/servicenow-table-api-openapi.yml, openapi/trouble-ticket-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 23\n    acting: 21\n  by_consequence:\n    read: 23\n    write: 18\n    safety-critical: 1\n    physical: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /contact\n  method: get\n  operationId:\
  \ getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/{id}\n  method: get\n  operationId: getContactById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/{tableName}\n  method: get\n  operationId: getAggregateStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachment\n  method: get\n  operationId: listAttachments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachment/{sys_id}\n  method: get\n  operationId: getAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachment/{sys_id}\n  method: delete\n  operationId: deleteAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachment/{sys_id}/file\n  method: get\n  operationId: downloadAttachmentFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachment/file\n  method: post\n\
  \  operationId: uploadAttachmentBinary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachment/upload\n  method: post\n  operationId: uploadAttachmentMultipart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /change/normal\n  method: get\n  operationId: listNormalChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change/normal\n  method: post\n  operationId: createNormalChange\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /change/normal/{sys_id}\n  method: get\n  operationId: getNormalChange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change/normal/{sys_id}\n  method: patch\n  operationId: updateNormalChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /change/standard\n  method: get\n  operationId: listStandardChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /change/standard/{standard_change_template_id}\n  method: post\n  operationId: createStandardChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /change/emergency\n  method: get\n  operationId: listEmergencyChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change/emergency\n  method: post\n  operationId: createEmergencyChange\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /change/{sys_id}/task\n  method: get\n  operationId: listChangeTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change/{sys_id}/task\n  method: post\n  operationId: createChangeTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instance/{className}\n  method: get\n  operationId: listCmdbInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance/{className}/{sys_id}\n  method: get\n  operationId: getCmdbInstance\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /import/{stagingTableName}\n  method: post\n  operationId: insertImportSetRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /import/{stagingTableName}/insertMultiple\n  method: post\n  operationId: insertMultipleImportSetRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servicecatalog/catalogs\n  method: get\n  operationId: listCatalogs\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servicecatalog/catalogs/{sys_id}\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servicecatalog/categories/{sys_id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servicecatalog/items\n  method: get\n  operationId: listCatalogItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servicecatalog/items/{sys_id}\n  method: get\n  operationId: getCatalogItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /servicecatalog/items/{sys_id}/add_to_cart\n  method: post\n  operationId: addItemToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servicecatalog/items/{sys_id}/order_now\n  method: post\n  operationId: orderItemNow\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servicecatalog/cart\n  method: get\n  operationId: getCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /servicecatalog/cart\n  method: delete\n  operationId: emptyCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servicecatalog/cart/submit_order\n  method: post\n  operationId: submitCartOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableName}\n  method: get\n  operationId: listRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /table/{tableName}\n  method: post\n  operationId: createRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableName}/{sys_id}\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /table/{tableName}/{sys_id}\n  method: put\n  operationId: updateRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableName}/{sys_id}\n  method: patch\n  operationId:\
  \ patchRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /table/{tableName}/{sys_id}\n  method: delete\n  operationId: deleteRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /troubleTicket\n  method: get\n  operationId: getTroubleTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /troubleTicket\n  method: post\n  operationId: createTroubleTicket\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /troubleTicket/{id}\n  method: get\n  operationId: getTroubleTicketById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /troubleTicket/{id}\n  method: patch\n  operationId: updateTroubleTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/agentic-access/servicenow-agentic-access.yml
summary_line: 44 operations · 21 acting · 1 human-in-the-loop
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
---
