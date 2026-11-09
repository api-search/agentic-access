---
acting_count: 42
action_class_counts:
  acting: 42
  connected: 34
api_specs:
- filename: noerrands-com-booking-api-openapi.yml
  format: yaml
  label: noerrands-com Booking API
  slug: noerrands-com-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noerrands-com/openapi/noerrands-com-booking-api-openapi.yml
- filename: noerrands-com-cards-api-openapi.yml
  format: yaml
  label: noerrands-com Cards API
  slug: noerrands-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noerrands-com/openapi/noerrands-com-cards-api-openapi.yml
- filename: noerrands-com-fax-api-openapi.yml
  format: yaml
  label: noerrands-com Fax API
  slug: noerrands-com-fax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noerrands-com/openapi/noerrands-com-fax-api-openapi.yml
- filename: noerrands-com-mail-api-openapi.yml
  format: yaml
  label: noerrands-com Mail API
  slug: noerrands-com-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noerrands-com/openapi/noerrands-com-mail-api-openapi.yml
- filename: noerrands-com-prints-api-openapi.yml
  format: yaml
  label: noerrands-com Prints API
  slug: noerrands-com-prints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noerrands-com/openapi/noerrands-com-prints-api-openapi.yml
- filename: noerrands-com-ship-api-openapi.yml
  format: yaml
  label: noerrands-com Ship API
  slug: noerrands-com-ship-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noerrands-com/openapi/noerrands-com-ship-api-openapi.yml
- filename: noerrands-com-sign-api-openapi.yml
  format: yaml
  label: noerrands-com Sign API
  slug: noerrands-com-sign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noerrands-com/openapi/noerrands-com-sign-api-openapi.yml
- filename: noerrands-com-tables-api-openapi.yml
  format: yaml
  label: noerrands-com Tables API
  slug: noerrands-com-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/noerrands-com/openapi/noerrands-com-tables-api-openapi.yml
consequence_counts:
  physical: 14
  read: 34
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Noerrands Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/cards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/envelopes/{envelope_id}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/faxes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/labels
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/letters
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/me
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pickups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pickups/{pickup_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/postcards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/returns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipments/{shipment_id}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/topups
operation_count: 76
overview: 'noerrands-com exposes 76 API operations that an AI agent could call, of which 42 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 28 write, and 14 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: noerrands-com
provider_slug: noerrands-com
slug: noerrands-com-agentic-access
source_filename: noerrands-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/booking-openapi.json, openapi/cards-openapi.json, openapi/fax-openapi.json,\n  openapi/mail-openapi.json, openapi/prints-openapi.json, openapi/ship-openapi.json, openapi/sign-openapi.json,\n  openapi/tables-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 76\n  by_action_class:\n    connected: 34\n    acting: 42\n  by_consequence:\n    read: 34\n    write: 28\n    physical: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/providers/search\n  method: post\n  operationId: search_providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/providers/{provider_id}/services\n\
  \  method: get\n  operationId: list_services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/providers/{provider_id}/availability\n  method: post\n  operationId: get_availability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings\n  method: post\n  operationId: create_booking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings\n  method: get\n  operationId: list_my_bookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/bookings/{booking_id}\n  method: get\n  operationId: get_booking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{booking_id}/cancel\n  method: post\n  operationId: cancel_booking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: delete\n  operationId: delete_my_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/designs\n  method: get\n  operationId: list_card_designs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/styles\n  method: get\n  operationId: list_handwriting_styles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quotes\n  method: post\n  operationId: preview_card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards\n  method: post\n  operationId: send_card\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards\n  method: get\n  operationId: list_cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{card_id}\n  method: get\n  operationId: get_card\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{card_id}/cancel\n  method: post\n  operationId: cancel_card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/balance\n  method: get\n  operationId: get_balance\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topups\n  method: post\n  operationId: create_topup_link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: delete\n  operationId: delete_my_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/estimate\n  method: post\n  operationId: estimate_fax_cost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/faxes\n  method: post\n  operationId: send_fax\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/faxes\n  method: get\n  operationId: list_faxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/faxes/{fax_id}\n  method: get\n  operationId: get_fax_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/balance\n  method: get\n  operationId: get_balance\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topups\n  method: post\n  operationId: create_topup_link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: delete\n  operationId: delete_my_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/addresses/verify\n  method: post\n  operationId: verify_address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/estimate\n  method: post\n  operationId: estimate_cost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/letters\n  method: post\n  operationId: send_letter\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/postcards\n  method: post\n  operationId: send_postcard\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mail/{mail_id}\n  method: get\n  operationId: get_mail_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mail\n  method: get\n  operationId: list_sent_mail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/balance\n  method: get\n  operationId: get_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topups\n  method: post\n  operationId:\
  \ create_topup_link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: delete\n  operationId: delete_my_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: get\n  operationId: get_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products\n  method: get\n  operationId: list_print_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images\n  method: post\n  operationId: upload_print_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quotes\n  method: post\n  operationId: quote_prints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders\n  method: post\n  operationId: order_prints\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders\n  method: get\n  operationId: list_print_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{order_id}\n  method: get\n  operationId: get_print_order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{order_id}/cancel\n  method: post\n  operationId: cancel_print_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/balance\n  method: get\n  operationId: get_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topups\n  method: post\n  operationId: create_topup_link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: delete\n  operationId: delete_my_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rates\n  method: post\n  operationId: get_shipping_rates\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/labels\n  method: post\n  operationId: buy_label\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/returns\n  method: post\n  operationId: create_return_label\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipments/{shipment_id}\n  method: get\n  operationId: get_shipment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments\n  method: get\n  operationId: list_shipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/track\n  method: get\n  operationId: track_package\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments/{shipment_id}/void\n  method: post\n  operationId: void_label\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pickups/options\n  method:\
  \ post\n  operationId: get_pickup_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pickups\n  method: post\n  operationId: schedule_pickup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pickups/{pickup_id}/cancel\n  method: post\n  operationId: cancel_pickup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/balance\n  method: get\n  operationId: get_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topups\n  method: post\n  operationId: create_topup_link\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: delete\n  operationId: delete_my_data\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/envelopes\n  method: post\n  operationId: create_envelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/envelopes\n  method: get\n  operationId: list_envelopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/envelopes/{envelope_id}/send\n  method: post\n  operationId: send_envelope\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/envelopes/{envelope_id}\n\
  \  method: get\n  operationId: get_envelope\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/envelopes/{envelope_id}\n  method: delete\n  operationId: delete_envelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/envelopes/{envelope_id}/signers/{signer_id}/link\n  method: post\n  operationId: remind_signer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/envelopes/{envelope_id}/void\n  method: post\n \
  \ operationId: void_envelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/envelopes/{envelope_id}/document\n  method: get\n  operationId: get_signed_document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/balance\n  method: get\n  operationId: get_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topups\n  method: post\n  operationId: create_topup_link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: delete\n  operationId: delete_my_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/requests\n  method: post\n  operationId: request_table\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/requests\n  method: get\n  operationId: list_table_requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/requests/{request_id}\n  method: get\n  operationId: get_table_request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/requests/{request_id}/cancel\n  method: post\n  operationId: cancel_table_request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/balance\n  method: get\n  operationId: get_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topups\n  method: post\n  operationId: create_topup_link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: delete\n  operationId: delete_my_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/noerrands-com/agentic-access/noerrands-com-agentic-access.yml
summary_line: 76 operations · 42 acting
tags:
- Company
- Artificial Intelligence
- Automation
- Productivity
- Messaging
---
