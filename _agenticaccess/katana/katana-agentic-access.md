---
acting_count: 139
action_class_counts:
  acting: 139
  connected: 87
api_specs:
- filename: katana-openapi-original.json
  format: json
  label: Katana API
  slug: katana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/katana/refs/heads/main/openapi/katana-openapi-original.json
consequence_counts:
  read: 87
  safety-critical: 139
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 139
kind: agentic-access
layout: agentic-access
method: generated
name: Katana Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /batch_stocks/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /batches
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bin_locations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /bin_locations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /bin_locations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bin_transfer_rows
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /bin_transfer_rows/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /bin_transfer_rows/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bin_transfers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /bin_transfers/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /bin_transfers/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /bin_transfers/{id}/status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bom_rows
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bom_rows/batch/create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /bom_rows/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /bom_rows/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /custom_field_definitions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /custom_field_definitions/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /custom_field_definitions/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /customer_addresses
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /customer_addresses/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /customer_addresses/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /customers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /customers/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /customers/{id}
operation_count: 226
overview: 'Katana exposes 226 API operations that an AI agent could call, of which 139 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 87 read and 139 safety-critical.


  139 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Katana
provider_slug: katana
slug: katana-agentic-access
source_filename: katana-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/katana-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 226\n  by_action_class:\n    connected: 87\n    acting: 139\n  by_consequence:\n    read: 87\n    safety-critical: 139\n  human_in_the_loop_required: 139\noperations:\n- path: /additional_costs\n  method: get\n  operationId: AdditionalCostController.getAdditionalCosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch_stocks/{id}\n  method: patch\n  operationId: BatchStockController.updateBatchStock\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /batch_stocks\n  method: get\n  operationId: BatchStockController.getBatchStock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches\n  method: post\n  operationId: BatchController.createBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_inventory\n  method: get\n  operationId: BinInventoryController.findAndPaginate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bin_locations/{id}\n  method: patch\n  operationId: BinLocationController.updateBinLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_locations/{id}\n  method: delete\n  operationId: BinLocationController.deleteBinLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_locations\n  method: post\n  operationId: BinLocationController.createBinLocation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_locations\n  method: get\n  operationId: BinLocationController.findBinLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bin_transfer_rows/{id}\n  method: patch\n  operationId: BinTransferRowController.updateById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_transfer_rows/{id}\n\
  \  method: get\n  operationId: BinTransferRowController.findById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bin_transfer_rows/{id}\n  method: delete\n  operationId: BinTransferRowController.deleteById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_transfer_rows\n  method: post\n  operationId: BinTransferRowController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /bin_transfer_rows\n  method: get\n  operationId: BinTransferRowController.findAndPaginate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bin_transfers/{id}/status\n  method: patch\n  operationId: BinTransferController.updateStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_transfers/{id}\n  method: patch\n  operationId: BinTransferController.updateById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_transfers/{id}\n  method: get\n  operationId: BinTransferController.findById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bin_transfers/{id}\n  method: delete\n  operationId: BinTransferController.deleteById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_transfers\n  method: post\n  operationId: BinTransferController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n    \
  \  exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bin_transfers\n  method: get\n  operationId: BinTransferController.findAndPaginate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bom_rows/batch/create\n  method: post\n  operationId: BomRowController.createBomRowsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bom_rows/{id}\n  method: patch\n  operationId: BomRowController.updateBomRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bom_rows/{id}\n  method: delete\n  operationId: BomRowController.deleteBomRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bom_rows\n  method: post\n  operationId: BomRowController.createBomRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /bom_rows\n  method: get\n  operationId: BomRowController.getBomRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_field_definitions/{id}\n  method: patch\n  operationId: CustomFieldDefinitionController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom_field_definitions/{id}\n  method: get\n  operationId: CustomFieldDefinitionController.getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_field_definitions/{id}\n  method: delete\n  operationId: CustomFieldDefinitionController.deleteById\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom_field_definitions\n  method: post\n  operationId: CustomFieldDefinitionController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom_field_definitions\n  method: get\n  operationId: CustomFieldDefinitionController.getAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_fields_collections\n\
  \  method: get\n  operationId: ItemsCustomFieldsCollectionController.getAllCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer_addresses/{id}\n  method: patch\n  operationId: CustomerAddressController.updateCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /customer_addresses/{id}\n  method: delete\n  operationId: CustomerAddressController.deleteCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /customer_addresses\n  method: post\n  operationId: CustomerAddressController.createCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /customer_addresses\n  method: get\n  operationId: CustomerAddressController.getAllCustomerAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: patch\n  operationId: CustomerController.updateVariant\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /customers/{id}\n  method: delete\n  operationId: CustomerController.deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /customers\n  method: post\n  operationId: CustomerController.createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /customers\n  method:\
  \ get\n  operationId: CustomerController.getAllCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand_forecasts\n  method: post\n  operationId: DemandForecastController.updateDemandForecast\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /demand_forecasts\n  method: get\n  operationId: DemandForecastController.findDemandForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand_forecasts\n  method: delete\n  operationId: DemandForecastController.clearDemandForecast\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /factory\n  method: get\n  operationId: FactoryController.getFactory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory\n  method: get\n  operationId: InventoryController.getInventories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory_movements\n  method: get\n  operationId: InventoryController.getInventoryMovements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /inventory_reorder_points\n  method: post\n  operationId: InventorySafetyStockLevelController.createInventoryReorderPoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /inventory_safety_stock_levels\n  method: post\n  operationId: InventorySafetyStockLevelController.createInventorySafetyStockLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /locations/{id}\n  method: get\n  operationId: LocationController.getLocation\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: LocationController.getAllLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturing_order_make_to_order\n  method: post\n  operationId: MakeToOrderMOController.createMTO\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_operation_rows/{id}\n  method: patch\n  operationId: ManufacturingOrderOperationRowController.updateManufacturingOrderOperationRow\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_operation_rows/{id}\n  method: get\n  operationId: ManufacturingOrderOperationRowController.retrieveManufacturingOrderOperationRow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturing_order_operation_rows/{id}\n  method: delete\n  operationId: ManufacturingOrderOperationRowController.deleteManufacturingOrderOperationRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /manufacturing_order_operation_rows\n  method: post\n  operationId: ManufacturingOrderOperationRowController.createManufacturingOrderOperationRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_operation_rows\n  method: get\n  operationId: ManufacturingOrderOperationRowController.getManufacturingOrderOperationRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturing_order_production_ingredients/{id}\n  method: patch\n  operationId: ManufacturingOrderProductionIngredientController.updateManufacturingOrderProductionIngredient\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_production_ingredients\n  method: get\n  operationId: ManufacturingOrderProductionIngredientController.find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturing_order_productions/{id}\n  method: patch\n  operationId: ManufacturingOrderProductionController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n  \
  \  audit: required\n- path: /manufacturing_order_productions/{id}\n  method: get\n  operationId: ManufacturingOrderProductionController.findById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturing_order_productions/{id}\n  method: delete\n  operationId: ManufacturingOrderProductionController.deleteManufacturingOrderProduction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_productions\n  method: post\n  operationId: ManufacturingOrderProductionController.completePartially\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_productions\n  method: get\n  operationId: ManufacturingOrderProductionController.find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturing_order_recipe_rows/{id}\n  method: patch\n  operationId: ManufacturingOrderRecipeRowController.updateManufacturingRecipeRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_recipe_rows/{id}\n  method: get\n  operationId:\
  \ ManufacturingOrderRecipeRowController.findManufacturingOrderRecipeRowById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturing_order_recipe_rows/{id}\n  method: delete\n  operationId: ManufacturingOrderRecipeRowController.deleteManufacturingOrderRecipeRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_recipe_rows\n  method: post\n  operationId: ManufacturingOrderRecipeRowController.createManufacturingOrderRecipeRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_recipe_rows\n  method: get\n  operationId: ManufacturingOrderRecipeRowController.findManufacturingOrderRecipeRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturing_order_rerank\n  method: post\n  operationId: MakeToOrderMOController.rerank\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_order_unlink\n  method: post\n  operationId: MakeToOrderMOController.unlink\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_orders/{id}\n  method: patch\n  operationId: ManufacturingOrderController.updateManufacturingOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_orders/{id}\n  method: get\n  operationId: ManufacturingOrderController.getManufacturingOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manufacturing_orders/{id}\n  method: delete\n\
  \  operationId: ManufacturingOrderController.deleteManufacturingOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_orders\n  method: post\n  operationId: ManufacturingOrderController.createManufacturingOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /manufacturing_orders\n  method: get\n  operationId: ManufacturingOrderController.getManufacturingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /materials/{id}\n  method: patch\n  operationId: MaterialController.updateMaterial\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /materials/{id}\n  method: get\n  operationId: MaterialController.getMaterial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /materials/{id}\n  method: delete\n  operationId: MaterialController.deleteManufacturingOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n     \
  \ purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /materials\n  method: post\n  operationId: MaterialController.createMaterial\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /materials\n  method: get\n  operationId: MaterialController.getAllMaterials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /negative_stock\n  method: get\n  operationId: NegativeStockLatestMovementController.getAllNegativeStockLatestMovements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /operators\n  method: get\n  operationId: OperatorsController.find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outsourced_purchase_order_recipe_rows/{id}\n  method: patch\n  operationId: PurchaseOrderRecipeRowController.updatePurchaseOrderRecipeRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /outsourced_purchase_order_recipe_rows/{id}\n  method: get\n  operationId: PurchaseOrderRecipeRowController.getPurchaseOrderRecipeRow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /outsourced_purchase_order_recipe_rows/{id}\n  method: delete\n  operationId: PurchaseOrderRecipeRowController.deletePurchaseOrderRecipeRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /outsourced_purchase_order_recipe_rows\n  method: post\n  operationId: PurchaseOrderRecipeRowController.createPurchaseOrderRecipeRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /outsourced_purchase_order_recipe_rows\n  method: get\n  operationId:\
  \ PurchaseOrderRecipeRowController.getPurchaseOrderRecipeRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /po_additional_cost_rows/{id}\n  method: patch\n  operationId: PoAdditionalCostRowController.updatePoAdditionalCostRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /po_additional_cost_rows/{id}\n  method: get\n  operationId: PoAdditionalCostRowController.getPoAdditionalCostRow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /po_additional_cost_rows/{id}\n  method: delete\n  operationId: PoAdditionalCostRowController.deletePoAdditionalCostRow\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /po_additional_cost_rows\n  method: post\n  operationId: PoAdditionalCostRowController.createPoAdditionalCostRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /po_additional_cost_rows\n  method: get\n  operationId: PoAdditionalCostRowController.getPoAdditionalCostRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /price_list_customers/{id}\n  method: patch\n  operationId: PriceListCustomerController.updateById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /price_list_customers/{id}\n  method: get\n  operationId: PriceListCustomerController.findById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price_list_customers/{id}\n  method: delete\n  operationId: PriceListCustomerController.deleteById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: r\n\n# --- truncated at 32 KB (75 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/katana/refs/heads/main/agentic-access/katana-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/katana/refs/heads/main/agentic-access/katana-agentic-access.yml
summary_line: 226 operations · 139 acting · 139 human-in-the-loop
tags:
- Company
- Enterprise
- Inventory
- Manufacturing
- ERP
- Supply Chain
- Warehouse Management
- Order Management
---
