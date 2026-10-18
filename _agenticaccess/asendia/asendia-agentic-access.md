---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 17
api_specs:
- filename: asendia-closeshipment-api-openapi.yml
  format: yaml
  label: Asendia Close Shipment API
  slug: asendia-closeshipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-closeshipment-api-openapi.yml
- filename: asendia-consolidation-api-openapi.yml
  format: yaml
  label: Asendia Consolidation API
  slug: asendia-consolidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-consolidation-api-openapi.yml
- filename: asendia-dpdtracking-api-openapi.yml
  format: yaml
  label: Asendia DPD Tracking API
  slug: asendia-dpdtracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-dpdtracking-api-openapi.yml
- filename: asendia-dws-api-openapi.yml
  format: yaml
  label: Asendia DWS API
  slug: asendia-dws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-dws-api-openapi.yml
- filename: asendia-externalinvoiceimport-api-openapi.yml
  format: yaml
  label: Asendia External Invoice Import API
  slug: asendia-externalinvoiceimport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-externalinvoiceimport-api-openapi.yml
- filename: asendia-fulfillment-api-openapi.yml
  format: yaml
  label: Asendia Fulfillment API
  slug: asendia-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-fulfillment-api-openapi.yml
- filename: asendia-idmailinterface-api-openapi.yml
  format: yaml
  label: Asendia ID Mail Interface API
  slug: asendia-idmailinterface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-idmailinterface-api-openapi.yml
- filename: asendia-npi-api-openapi.yml
  format: yaml
  label: Asendia NPI API
  slug: asendia-npi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-npi-api-openapi.yml
- filename: asendia-parcel-api-openapi.yml
  format: yaml
  label: Asendia Parcel API
  slug: asendia-parcel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-parcel-api-openapi.yml
- filename: asendia-pudolocator-api-openapi.yml
  format: yaml
  label: Asendia Pudo Locator API
  slug: asendia-pudolocator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-pudolocator-api-openapi.yml
- filename: asendia-puttolight-api-openapi.yml
  format: yaml
  label: Asendia Put To Light API
  slug: asendia-puttolight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-puttolight-api-openapi.yml
- filename: asendia-receptaclesorting-api-openapi.yml
  format: yaml
  label: Asendia Receptacle Sorting API
  slug: asendia-receptaclesorting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-receptaclesorting-api-openapi.yml
- filename: asendia-servicenow-api-openapi.yml
  format: yaml
  label: Asendia Service Now API
  slug: asendia-servicenow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-servicenow-api-openapi.yml
- filename: asendia-shippingplatform-api-openapi.yml
  format: yaml
  label: Asendia Shipping Platform API
  slug: asendia-shippingplatform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-shippingplatform-api-openapi.yml
- filename: asendia-shippingplatformbulk-api-openapi.yml
  format: yaml
  label: Asendia Shipping Platform Bulk API
  slug: asendia-shippingplatformbulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-shippingplatformbulk-api-openapi.yml
- filename: asendia-tracking-api-openapi.yml
  format: yaml
  label: Asendia Tracking API
  slug: asendia-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/openapi/asendia-tracking-api-openapi.yml
consequence_counts:
  physical: 10
  read: 17
  safety-critical: 4
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Asendia Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/A1/v1.0/ShippingPlatform/CloseDirectShipmentDispatch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/A1/v1.0/ShippingPlatform/CloseDispatch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/A1/v1.0/ShippingPlatform/PreAlertDispatch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/A1/v1.0/ShippingPlatform/PreAlertDispatchWithReceptacle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/A1/CloseShipment/CloseDAShipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/A1/CloseShipment/CloseShipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/A1/Fulfillment/PurchaseOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/A1/Fulfillment/SalesOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/A1/Fulfillment/VoidSalesOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/A1/v1.0/Consolidation/Orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/A1/v1.0/ExternalInvoiceImport/Invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/A1/v1.0/ShippingPlatform/Package
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/A1/v1.0/ShippingPlatform/Package
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/A1/v1.0/ShippingPlatformBulk/Package
operation_count: 50
overview: 'Asendia exposes 50 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 19 write, 10 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Asendia
provider_slug: asendia
slug: asendia-agentic-access
source_filename: asendia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/asendia-a1-consolidation-openapi.yml, openapi/asendia-a1-dpd-tracking-openapi.yml,\n  openapi/asendia-a1-dws-openapi.yml, openapi/asendia-a1-externalinvoiceimport-openapi.yml,\n  openapi/asendia-a1-fulfillment-openapi.yml, openapi/asendia-a1-idmailinterface-openapi.yml,\n  openapi/asendia-a1-npi-openapi.yml, openapi/asendia-a1-parcel-openapi.yml, openapi/asendia-a1-pudo-locator-openapi.yml,\n  openapi/asendia-a1-put-to-light-openapi.yml, openapi/asendia-a1-receptacle-openapi.yml, openapi/asendia-a1-servicenow-openapi.yml,\n  openapi/asendia-a1-shippingplatform-openapi.yml, openapi/asendia-a1-shippingplatformbulk-openapi.yml,\n  openapi/asendia-a1-tracking-openapi.yml, openapi/asendia-a1-tracking-v2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment.\
  \ See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    acting: 33\n    connected: 17\n  by_consequence:\n    physical: 10\n    write: 19\n    read: 17\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /api/A1/v1.0/Consolidation/Orders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/DPDTracking/TTEvents\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Operation/DWS/PreProcessParcel2\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Operation/DWS/PreProcessParcel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Operation/DWS/GenericPreProcessParcel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Operation/DWS/PreProcessParcelSimulator\n\
  \  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Operation/DWS/PackageLabel\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/Operation/DWS/PackageLabelManagerOverride\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/Operation/DWS/VolumizerPreProcessParcel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Operation/DWS/VitronicDashboardItems\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/v1.0/ExternalInvoiceImport/Invoice\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Fulfillment/SalesOrder\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/Fulfillment/SalesOrder\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Fulfillment/VoidSalesOrder\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Fulfillment/InventoryAdjustments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/Fulfillment/PurchaseOrder\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/Fulfillment/PurchaseOrder\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/External/IDMailInterface/InsertProcessingEntry\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/External/IDMailInterface/CloseBag\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/External/IDMailInterface/FinishRun\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Operation/NPI/Bin\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/Operation/NPI/Bin\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api/A1/Operation/NPI/BinClose\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/CloseShipment/CloseShipment\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/CloseShipment/CloseDAShipment\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/Parcel/CreateParcel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/Parcel/CustomerCreateParcel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/Parcel/UKCreateParcel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/Parcel/UKCreateParcel\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/Parcel/DeleteParcel\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v2.6/PudoLocator/PudoLocation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/A1/Operation/PutToLight/Barcode\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/Operation/PutToLight/Barcode2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/ReceptacleSorting/CreateReceptacle\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/ReceptacleSorting/GetReceptacle\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/v1.0/ServiceNow/Account\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/v1.0/ServiceNow/Contact\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/v1.0/ShippingPlatform/Package\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/ShippingPlatform/Package\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/v1.0/ShippingPlatform/Package\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/ShippingPlatform/CloseDispatch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/A1/v1.0/ShippingPlatform/ShippingRate\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/v1.0/ShippingPlatform/PreAlertDispatch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/A1/v1.0/ShippingPlatform/PreAlertDispatchWithReceptacle\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/A1/v1.0/ShippingPlatform/CloseDirectShipmentDispatch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/A1/v1.0/ShippingPlatformBulk/Package\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/A1/v1.0/Tracking/Detail\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/v1.0/Tracking/Milestone\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/v2.0/Tracking/Detail\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/A1/v2.0/Tracking/Milestone\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asendia/refs/heads/main/agentic-access/asendia-agentic-access.yml
summary_line: 50 operations · 33 acting · 4 human-in-the-loop
tags:
- Company
- Shipping
- Logistics
- Parcel
- Cross-border eCommerce
- Tracking
- Postal
---
