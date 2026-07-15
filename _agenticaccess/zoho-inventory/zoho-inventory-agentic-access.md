---
acting_count: 356
action_class_counts:
  acting: 356
  connected: 148
api_specs:
- filename: batches.yml
  format: yaml
  label: Zoho Inventory API
  slug: zoho-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-inventory/refs/heads/main/openapi/batches.yml
consequence_counts:
  physical: 116
  read: 148
  safety-critical: 4
  write: 236
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Zoho Inventory Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /invoices/{invoice_id}/paymentreminder/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /items/disablestoragelocation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /locations/{location_id}/storagelocations/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /settings/warehouses/{warehouse_id}/storagelocations/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /creditnotes/{creditnote_id}/address/shipping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /creditnotes/{creditnote_id}/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /creditnotes/{creditnote_id}/invoices/{creditnote_invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /creditnotes/{creditnote_id}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /creditnotes/{creditnote_id}/refunds/{creditnote_refund_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /creditnotes/{creditnote_id}/refunds/{creditnote_refund_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /customerpayment/{customer_payment_id}/customfields
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /customerpayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /customerpayments/{payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /customerpayments/{payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /deliverychallans/{deliverychallan_id}/address/shipping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoice/{invoice_id}/customfields
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoices/{invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /invoices/{invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoices/{invoice_id}/address/billing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoices/{invoice_id}/address/shipping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{invoice_id}/approve
operation_count: 504
overview: 'Zoho Inventory exposes 504 API operations that an AI agent could call, of which 356 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 148 read, 236 write, 116 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zoho Inventory
provider_slug: zoho-inventory
slug: zoho-inventory-agentic-access
source_filename: zoho-inventory-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/batches.yml, openapi/bills.yml, openapi/compositeitems.yml, openapi/contact-persons.yml,\n  openapi/contacts.yml, openapi/credit-notes.yml, openapi/currency.yml, openapi/customer-payments.yml,\n  openapi/delivery-challans.yml, openapi/inventoryadjustments.yml, openapi/invoices.yml, openapi/itemgroups.yml,\n  openapi/items.yml, openapi/landedcosts.yml, openapi/locations.yml, openapi/moveorders.yml,\n  openapi/organizations.yml, openapi/packages.yml, openapi/picklists.yml, openapi/pricelists.yml,\n  openapi/purchaseorders.yml, openapi/purchasereceives.yml, openapi/putaways.yml, openapi/replenishment.yml,\n  openapi/reporting-tags.yml, openapi/retainer-invoices.yml, openapi/salesorders.yml, openapi/salesreturns.yml,\n  openapi/serialnumbers.yml, openapi/shipmentorders.yml, openapi/storagelocations.yml, openapi/tasks.yml,\n  openapi/taxes.yml, openapi/transferorders.yml, openapi/unit_of_measurement.yml, openapi/users.yml,\n\
  \  openapi/vendor-credits.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 504\n  by_action_class:\n    acting: 356\n    connected: 148\n  by_consequence:\n    write: 236\n    read: 148\n    physical: 116\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /items/batches\n  method: post\n  operationId: create_a_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.items.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/batches\n  method: get\n  operationId: list_batches\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.items.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /items/batches\n  method: delete\n  operationId: bulk_delete_batches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.items.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/batches/{batch_id}\n  method: get\n  operationId: retrieve_a_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.items.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /items/batches/{batch_id}\n  method: put\n  operationId: update_a_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    scope:\n    - ZohoInventory.items.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/batches/{batch_id}\n  method: delete\n  operationId: delete_a_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.items.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/batches/{batch_id}/active\n  method: post\n  operationId: mark_batch_as_active\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.items.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/batches/{batch_id}/inactive\n  method: post\n  operationId: mark_batch_as_inactive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.items.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/batches/active\n  method: post\n  operationId: mark_batches_as_active\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.items.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /items/batches/inactive\n  method: post\n  operationId: mark_batches_as_inactive\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.items.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills\n  method: post\n  operationId: create_bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills\n  method: get\n  operationId: list_bills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.bills.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/{bill_id}\n  method: get\n  operationId:\
  \ get_bill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.bills.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bills/{bill_id}\n  method: put\n  operationId: update_bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{bill_id}\n  method: delete\n  operationId: delete_bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bill/{bill_id}/customfields\n\
  \  method: put\n  operationId: update_custom_field_in_bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{bill_id}/status/open\n  method: post\n  operationId: mark_bill_as_open\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{bill_id}/status/void\n  method: post\n  operationId: mark_bill_as_void\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.CREATE\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{bill_id}/submit\n  method: post\n  operationId: submit_bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{bill_id}/approve\n  method: post\n  operationId: approve_bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{bill_id}/approve/final\n\
  \  method: post\n  operationId: approve_bill_final\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/{bill_id}/reject\n  method: post\n  operationId: reject_bill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/submit\n  method: post\n  operationId: bulk_submit_bills\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.UPDATE\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bills/approve\n  method: post\n  operationId: bulk_approve_bills\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.bills.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compositeitems\n  method: post\n  operationId: create_composite_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compositeitems\n\
  \  method: get\n  operationId: list_composite_items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.compositeitems.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compositeitems/{composite_item_id}\n  method: get\n  operationId: get_composite_item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.compositeitems.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compositeitems/{composite_item_id}\n  method: put\n  operationId: update_composite_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compositeitems/{composite_item_id}\n\
  \  method: delete\n  operationId: delete_composite_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compositeitems/{composite_item_id}/active\n  method: post\n  operationId: mark_composite_item_active\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compositeitems/{composite_item_id}/inactive\n  method: post\n  operationId: mark_composite_item_inactive\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compositeitems/{composite_item_id}/image\n  method: post\n  operationId: upload_composite_item_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compositeitems/{composite_item_id}/image\n  method: delete\n  operationId: delete_composite_item_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.DELETE\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles\n  method: post\n  operationId: create_assemblies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles\n  method: get\n  operationId: list_assemblies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.compositeitems.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundle_id}\n  method: get\n  operationId: get_assembly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n \
  \   - ZohoInventory.compositeitems.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundle_id}\n  method: put\n  operationId: update_assembly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{bundle_id}\n  method: delete\n  operationId: delete_assembly\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{bundle_id}/bundled\n  method: post\n  operationId: mark_assembly_as_built\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{bundle_id}/confirmed\n  method: post\n  operationId: mark_assembly_as_confirmed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.compositeitems.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/contactpersons\n  method: post\n  operationId: create_contact_person\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.CREATE\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/contactpersons/{contact_person_id}\n  method: put\n  operationId: update_contact_person\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/contactpersons/{contact_person_id}\n  method: delete\n  operationId: delete_contact_person\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /contacts/{contact_id}/contactpersons\n  method: get\n  operationId: list_contact_persons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.contacts.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contact_id}/contactpersons/{contact_person_id}\n  method: get\n  operationId: get_contact_person\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.contacts.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/contactpersons/{contact_person_id}/primary\n  method: post\n  operationId: mark_contact_person_as_primary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: post\n  operationId: create_contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: get\n  operationId: list_contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.contacts.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contact_id}\n  method: put\n  operationId: update_contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.UPDATE\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contact_id}\n  method: get\n  operationId: get_contact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.contacts.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contact_id}\n  method: delete\n  operationId: delete_contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contact_id}/address\n  method: get\n  operationId: get_contact_address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - ZohoInventory.contacts.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contact_id}/active\n  method: post\n  operationId: mark_contact_as_active\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contact_id}/inactive\n  method: post\n  operationId: mark_contact_as_inactive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contact_id}/statements/email\n  method:\
  \ post\n  operationId: email_statement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contact_id}/statements/email\n  method: get\n  operationId: get_statement_mail_content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.contacts.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contact_id}/email\n  method: post\n  operationId: email_contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.contacts.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contact_id}/comments\n  method: get\n  operationId: list_contact_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.contacts.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes\n  method: post\n  operationId: create_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes\n  method: get\n  operationId: list_credit_notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}\n  method: put\n  operationId: update_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}\n  method: get\n  operationId: get_credit_note\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}\n  method: delete\n  operationId: delete_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.DELETE\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/email\n  method: post\n  operationId: email_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/email\n  method: get\n  operationId: get_credit_note_email_content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}/void\n  method: post\n  operationId: mark_credit_note_as_void\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/draft\n  method: post\n  operationId: mark_credit_note_as_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/converttoopen\n  method: post\n  operationId: mark_credit_note_as_open\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/submit\n  method: post\n  operationId: submit_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/approve\n  method: post\n  operationId: approve_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /creditnotes/{creditnote_id}/emailhistory\n  method: get\n  operationId: get_credit_note_email_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}/address/billing\n  method: put\n  operationId: update_credit_note_billing_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/address/shipping\n  method: put\n  operationId: update_credit_note_shipping_address\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n \
  \   scope:\n    - ZohoInventory.creditnotes.UPDATE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/templates\n  method: get\n  operationId: list_credit_note_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}/templates/{template_id}\n  method: put\n  operationId: update_credit_note_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.UPDATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /creditnotes/{creditnote_id}/invoices\n  method: get\n  operationId: list_invoices_credited\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}/invoices\n  method: post\n  operationId: apply_credits_to_invoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/invoices/{creditnote_invoice_id}\n  method: delete\n  operationId: delete_credits_applied_to_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.DELETE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/comments\n  method: get\n  operationId: list_credit_note_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}/comments\n  method: post\n  operationId: create_credit_note_comment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/comments/{comment_id}\n  method: delete\n  operationId: delete_credit_note_comment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.DELETE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/refunds\n  method: get\n  operationId: list_credit_note_refunds_of_all_credit_notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}/refunds\n  method: get\n  operationId: list_credit_note_refunds_of_a_credit_notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}/refunds\n  method: post\n  operationId: create_credit_note_refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - ZohoInventory.creditnotes.CREATE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creditnotes/{creditnote_id}/refunds/{creditnote_refund_id}\n  method: get\n  operationId: get_credit_note_refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoInventory.creditnotes.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creditnotes/{creditnote_id}/refunds/{creditnote_refund_id}\n\
  \  method: put\n  operationId: update_credit_note_refun\n\n# --- truncated at 32 KB (188 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/zoho-inventory/refs/heads/main/agentic-access/zoho-inventory-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-inventory/refs/heads/main/agentic-access/zoho-inventory-agentic-access.yml
summary_line: 504 operations · 356 acting · 4 human-in-the-loop
tags:
- Inventory Management
- Warehousing
- Sales Orders
- Purchase Orders
- Stock Adjustment
- Shipments
- Items
- E-commerce
---
