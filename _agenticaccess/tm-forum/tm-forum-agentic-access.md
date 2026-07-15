---
acting_count: 255
action_class_counts:
  acting: 255
  connected: 80
api_specs:
- filename: tm-forum-tmf620-product-catalog-openapi.yaml
  format: yaml
  label: TMF620 Product Catalog Management
  slug: tmf620-product-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf620-product-catalog-openapi.yaml
- filename: tm-forum-tmf621-trouble-ticket-openapi.yaml
  format: yaml
  label: TMF621 Trouble Ticket Management
  slug: tmf621-trouble-ticket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf621-trouble-ticket-openapi.yaml
- filename: tm-forum-tmf622-product-ordering-openapi.yaml
  format: yaml
  label: TMF622 Product Order Management
  slug: tmf622-product-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf622-product-ordering-openapi.yaml
- filename: tm-forum-tmf629-customer-management-openapi.yaml
  format: yaml
  label: TMF629 Customer Management
  slug: tmf629-customer-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf629-customer-management-openapi.yaml
- filename: tm-forum-tmf632-party-management-openapi.yaml
  format: yaml
  label: TMF632 Party Management
  slug: tmf632-party-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf632-party-management-openapi.yaml
- filename: tm-forum-tmf633-service-catalog-openapi.json
  format: json
  label: TMF633 Service Catalog Management
  slug: tmf633-service-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf633-service-catalog-openapi.json
- filename: tm-forum-tmf634-resource-catalog-openapi.json
  format: json
  label: TMF634 Resource Catalog Management
  slug: tmf634-resource-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf634-resource-catalog-openapi.json
- filename: tm-forum-tmf637-product-inventory-openapi.yaml
  format: yaml
  label: TMF637 Product Inventory Management
  slug: tmf637-product-inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf637-product-inventory-openapi.yaml
- filename: tm-forum-tmf641-service-ordering-openapi.json
  format: json
  label: TMF641 Service Order Management
  slug: tmf641-service-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf641-service-ordering-openapi.json
- filename: tm-forum-tmf648-quote-management-openapi.json
  format: json
  label: TMF648 Quote Management
  slug: tmf648-quote-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf648-quote-management-openapi.json
- filename: tm-forum-tmf651-agreement-management-openapi.json
  format: json
  label: TMF651 Agreement Management
  slug: tmf651-agreement-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf651-agreement-management-openapi.json
- filename: tm-forum-tmf666-account-management-openapi.json
  format: json
  label: TMF666 Account Management
  slug: tmf666-account-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/openapi/tm-forum-tmf666-account-management-openapi.json
consequence_counts:
  physical: 29
  read: 80
  write: 226
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tm Forum Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cancelProductOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cancelServiceOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/cancelProductOrderCreateEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/cancelProductOrderInformationRequiredEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/cancelProductOrderStateChangeEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/cancelServiceOrderCreateEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/cancelServiceOrderInformationRequiredEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/cancelServiceOrderStateChangeEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/productOrderAttributeValueChangeEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/productOrderCreateEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/productOrderDeleteEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/productOrderErrorMessageEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/productOrderInformationRequiredEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/productOrderJeopardyAlertEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/productOrderMilestoneEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/productOrderStateChangeEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderAttributeValueChangeEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderCreateEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderDeleteEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderInformationRequiredEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderJeopardyEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderMilestoneEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /listener/serviceOrderStateChangeEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /productOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /productOrder/{id}
operation_count: 335
overview: 'TM Forum exposes 335 API operations that an AI agent could call, of which 255 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 80 read, 226 write, and 29 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TM Forum
provider_slug: tm-forum
slug: tm-forum-agentic-access
source_filename: tm-forum-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tm-forum-tmf620-product-catalog-openapi.yaml, openapi/tm-forum-tmf621-trouble-ticket-openapi.yaml,\n  openapi/tm-forum-tmf622-product-ordering-openapi.yaml, openapi/tm-forum-tmf629-customer-management-openapi.yaml,\n  openapi/tm-forum-tmf632-party-management-openapi.yaml, openapi/tm-forum-tmf633-service-catalog-openapi.json,\n  openapi/tm-forum-tmf634-resource-catalog-openapi.json, openapi/tm-forum-tmf637-product-inventory-openapi.yaml,\n  openapi/tm-forum-tmf641-service-ordering-openapi.json, openapi/tm-forum-tmf648-quote-management-openapi.json,\n  openapi/tm-forum-tmf651-agreement-management-openapi.json, openapi/tm-forum-tmf666-account-management-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 335\n  by_action_class:\n    connected: 80\n    acting: 255\n  by_consequence:\n    read: 80\n    write: 226\n    physical: 29\n  human_in_the_loop_required: 0\noperations:\n- path: /category\n  method: get\n  operationId: listCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /category\n  method: post\n  operationId: createCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /category/{id}\n  method: get\n  operationId: retrieveCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /category/{id}\n  method:\
  \ patch\n  operationId: patchCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /category/{id}\n  method: delete\n  operationId: deleteCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exportJob\n  method: get\n  operationId: listExportJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exportJob\n  method: post\n  operationId: createExportJob\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exportJob/{id}\n  method: get\n  operationId: retrieveExportJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exportJob/{id}\n  method: delete\n  operationId: deleteExportJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub\n  method: post\n  operationId: createHub\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/{id}\n  method: delete\n  operationId: hubDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /importJob\n  method: get\n  operationId: listImportJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /importJob\n  method: post\n  operationId: createImportJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /importJob/{id}\n  method: get\n  operationId: retrieveImportJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /importJob/{id}\n  method: delete\n  operationId: deleteImportJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/categoryAttributeValueChangeEvent\n  method: post\n  operationId: categoryAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/categoryCreateEvent\n\
  \  method: post\n  operationId: categoryCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/categoryDeleteEvent\n  method: post\n  operationId: categoryDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/categoryStateChangeEvent\n  method: post\n  operationId: categoryStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/exportJobCreateEvent\n  method: post\n  operationId: exportJobCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/exportJobStateChangeEvent\n  method: post\n  operationId: exportJobStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/importJobCreateEvent\n  method: post\n  operationId: importJobCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/importJobStateChangeEvent\n  method: post\n  operationId: importJobStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productCatalogAttributeValueChangeEvent\n  method: post\n  operationId: productCatalogAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productCatalogCreateEvent\n\
  \  method: post\n  operationId: productCatalogCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productCatalogDeleteEvent\n  method: post\n  operationId: productCatalogDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productCatalogStateChangeEvent\n  method: post\n  operationId: productCatalogStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOfferingAttributeValueChangeEvent\n  method: post\n  operationId: productOfferingAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOfferingCreateEvent\n  method: post\n  operationId: productOfferingCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOfferingDeleteEvent\n  method: post\n  operationId: productOfferingDeleteEvent\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOfferingPriceAttributeValueChangeEvent\n  method: post\n  operationId: productOfferingPriceAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOfferingPriceCreateEvent\n  method: post\n  operationId: productOfferingPriceCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOfferingPriceDeleteEvent\n  method: post\n  operationId: productOfferingPriceDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOfferingPriceStateChangeEvent\n  method: post\n  operationId: productOfferingPriceStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOfferingStateChangeEvent\n  method: post\n  operationId: productOfferingStateChangeEvent\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productSpecificationAttributeValueChangeEvent\n  method: post\n  operationId: productSpecificationAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productSpecificationCreateEvent\n  method: post\n  operationId: productSpecificationCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /listener/productSpecificationDeleteEvent\n  method: post\n  operationId: productSpecificationDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productSpecificationStateChangeEvent\n  method: post\n  operationId: productSpecificationStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productCatalog\n  method: get\n  operationId: listProductCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productCatalog\n  method: post\n  operationId: createProductCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productCatalog/{id}\n  method: get\n  operationId: retrieveProductCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productCatalog/{id}\n  method: patch\n  operationId: patchProductCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /productCatalog/{id}\n  method: delete\n  operationId: deleteProductCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productOffering\n  method: get\n  operationId: listProductOffering\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productOffering\n  method: post\n  operationId: createProductOffering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productOffering/{id}\n  method: get\n  operationId:\
  \ retrieveProductOffering\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productOffering/{id}\n  method: patch\n  operationId: patchProductOffering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productOffering/{id}\n  method: delete\n  operationId: deleteProductOffering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productOfferingPrice\n  method: get\n  operationId: listProductOfferingPrice\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productOfferingPrice\n  method: post\n  operationId: createProductOfferingPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productOfferingPrice/{id}\n  method: get\n  operationId: retrieveProductOfferingPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productOfferingPrice/{id}\n  method: patch\n  operationId: patchProductOfferingPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productOfferingPrice/{id}\n  method: delete\n  operationId: deleteProductOfferingPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productSpecification\n  method: get\n  operationId: listProductSpecification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productSpecification\n  method: post\n  operationId: createProductSpecification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /productSpecification/{id}\n  method: get\n  operationId: retrieveProductSpecification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productSpecification/{id}\n  method: patch\n  operationId: patchProductSpecification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /productSpecification/{id}\n  method: delete\n  operationId: deleteProductSpecification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /hub\n  method: post\n  operationId: createHub\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/{id}\n  method: get\n  operationId: hubGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hub/{id}\n  method: delete\n  operationId: hubDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketAttributeValueChangeEvent\n  method: post\n  operationId:\
  \ troubleTicketAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketCreateEvent\n  method: post\n  operationId: troubleTicketCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketDeleteEvent\n  method: post\n  operationId: troubleTicketDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketInformationRequiredEvent\n  method: post\n  operationId: troubleTicketInformationRequiredEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketResolvedEvent\n  method: post\n  operationId: troubleTicketResolvedEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketSpecificationAttributeValueChangeEvent\n  method: post\n  operationId: troubleTicketSpecificationAttributeValueChangeEvent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketSpecificationCreateEvent\n  method: post\n  operationId: troubleTicketSpecificationCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketSpecificationDeleteEvent\n  method: post\n  operationId: troubleTicketSpecificationDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketSpecificationStatusChangeEvent\n  method: post\n  operationId: troubleTicketSpecificationStatusChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/troubleTicketStatusChangeEvent\n  method: post\n  operationId: troubleTicketStatusChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /troubleTicket\n  method: get\n  operationId: listTroubleTicket\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /troubleTicket\n  method: post\n  operationId: createTroubleTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /troubleTicket/{id}\n  method: get\n  operationId: retrieveTroubleTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /troubleTicket/{id}\n  method: patch\n  operationId: patchTroubleTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /troubleTicket/{id}\n  method: delete\n  operationId: deleteTroubleTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /troubleTicketSpecification\n  method: get\n  operationId: listTroubleTicketSpecification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /troubleTicketSpecification\n  method: post\n  operationId: createTroubleTicketSpecification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /troubleTicketSpecification/{id}\n  method: get\n  operationId: retrieveTroubleTicketSpecification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /troubleTicketSpecification/{id}\n  method: patch\n  operationId: patchTroubleTicketSpecification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /troubleTicketSpecification/{id}\n  method: delete\n  operationId: deleteTroubleTicketSpecification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /cancelProductOrder\n  method: get\n  operationId: listCancelProductOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cancelProductOrder\n  method: post\n  operationId: createCancelProductOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancelProductOrder/{id}\n  method: get\n  operationId: retrieveCancelProductOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hub\n  method: post\n  operationId: createHub\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hub/{id}\n  method: delete\n  operationId: hubDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/cancelProductOrderCreateEvent\n  method: post\n  operationId: cancelProductOrderCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /listener/cancelProductOrderInformationRequiredEvent\n  method: post\n  operationId: cancelProductOrderInformationRequiredEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/cancelProductOrderStateChangeEvent\n  method: post\n  operationId: cancelProductOrderStateChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOrderAttributeValueChangeEvent\n\
  \  method: post\n  operationId: productOrderAttributeValueChangeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOrderCreateEvent\n  method: post\n  operationId: productOrderCreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOrderDeleteEvent\n  method: post\n  operationId: productOrderDeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOrderErrorMessageEvent\n  method: post\n  operationId: productOrderErrorMessageEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listener/productOrderInformationRequiredEvent\n  method: post\n  operationId: productOrderInformationRequiredEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: tru\n\n\
  # --- truncated at 32 KB (108 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/agentic-access/tm-forum-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tm-forum/refs/heads/main/agentic-access/tm-forum-agentic-access.yml
summary_line: 335 operations · 255 acting
tags:
- Telco
- Telecommunications
- BSS
- OSS
- Open APIs
- Standards
---
