---
acting_count: 60
action_class_counts:
  acting: 60
  connected: 35
api_specs:
- filename: karrio-addresses-api-openapi.yml
  format: yaml
  label: Karrio Addresses API
  slug: karrio-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-addresses-api-openapi.yml
- filename: karrio-api-api-openapi.yml
  format: yaml
  label: Karrio API
  slug: karrio-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-api-api-openapi.yml
- filename: karrio-auth-api-openapi.yml
  format: yaml
  label: Karrio Auth API
  slug: karrio-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-auth-api-openapi.yml
- filename: karrio-batches-api-openapi.yml
  format: yaml
  label: Karrio Batches API
  slug: karrio-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-batches-api-openapi.yml
- filename: karrio-carriers-api-openapi.yml
  format: yaml
  label: Karrio Carriers API
  slug: karrio-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-carriers-api-openapi.yml
- filename: karrio-connections-api-openapi.yml
  format: yaml
  label: Karrio Connections API
  slug: karrio-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-connections-api-openapi.yml
- filename: karrio-documents-api-openapi.yml
  format: yaml
  label: Karrio Documents API
  slug: karrio-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-documents-api-openapi.yml
- filename: karrio-manifests-api-openapi.yml
  format: yaml
  label: Karrio Manifests API
  slug: karrio-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-manifests-api-openapi.yml
- filename: karrio-orders-api-openapi.yml
  format: yaml
  label: Karrio Orders API
  slug: karrio-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-orders-api-openapi.yml
- filename: karrio-parcels-api-openapi.yml
  format: yaml
  label: Karrio Parcels API
  slug: karrio-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-parcels-api-openapi.yml
- filename: karrio-pickups-api-openapi.yml
  format: yaml
  label: Karrio Pickups API
  slug: karrio-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-pickups-api-openapi.yml
- filename: karrio-products-api-openapi.yml
  format: yaml
  label: Karrio Products API
  slug: karrio-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-products-api-openapi.yml
- filename: karrio-proxy-api-openapi.yml
  format: yaml
  label: Karrio Proxy API
  slug: karrio-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-proxy-api-openapi.yml
- filename: karrio-shipments-api-openapi.yml
  format: yaml
  label: Karrio Shipments API
  slug: karrio-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-shipments-api-openapi.yml
- filename: karrio-trackers-api-openapi.yml
  format: yaml
  label: Karrio Trackers API
  slug: karrio-trackers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-trackers-api-openapi.yml
- filename: karrio-webhooks-api-openapi.yml
  format: yaml
  label: Karrio Webhooks API
  slug: karrio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-webhooks-api-openapi.yml
consequence_counts:
  physical: 16
  read: 35
  write: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Karrio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/batches/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/batches/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/batches/webhooks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/proxy/rates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/proxy/shipping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/proxy/shipping/{carrier_name}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/shipments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipments/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipments/{id}/documents/{doc}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipments/{id}/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipments/{id}/rates
operation_count: 95
overview: 'Karrio exposes 95 API operations that an AI agent could call, of which 60 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read, 44 write, and 16 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Karrio
provider_slug: karrio
slug: karrio-agentic-access
source_filename: karrio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: generated\nsource: openapi/karrio-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 95\n  by_action_class:\n    connected: 35\n    acting: 60\n  by_consequence:\n    read: 35\n    write: 44\n    physical: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: '&&ping'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/logout\n  method: post\n  operationId: '&&logout'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/token\n  method: post\n  operationId: '&&authenticate'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/token/refresh\n  method: post\n  operationId: '&&refresh_token'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/token/verified\n  method: post\n  operationId: '&&get_verified_token'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/token/verify\n  method: post\n  operationId: '&&verify_token'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tokens\n  method: post\n  operationId: '&&generate_resource_token'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/addresses\n  method: get\n  operationId: $list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/addresses\n  method: post\n  operationId: $create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/addresses/{id}\n  method: get\n  operationId: $retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/addresses/{id}\n  method: patch\n  operationId: $update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/addresses/{id}\n\
  \  method: delete\n  operationId: $discard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches/data/export/{resource_type}.{export_format}\n  method: get\n  operationId: '&&&&$export_file'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batches/data/import\n  method: post\n  operationId: '&&&&$import_file'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches/operations\n  method: get\n  operationId:\
  \ '&&&&$list'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batches/operations/{id}\n  method: get\n  operationId: '&&&&$retrieve'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batches/orders\n  method: post\n  operationId: '&&&&$create_orders'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches/shipments\n  method: post\n  operationId: '&&&&$create_shipments'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches/trackers\n  method: post\n  operationId: '&&&&$create_trackers'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches/webhooks\n  method: post\n  operationId: $$$$$$$$resend_webhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/carriers\n  method: get\n  operationId: '&&list'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/carriers/{carrier_name}\n  method: get\n  operationId: '&&get_details'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/carriers/{carrier_name}/options\n  method: get\n  operationId: '&&get_options'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/carriers/{carrier_name}/services\n  method: get\n  operationId: '&&get_services'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections\n  method: get\n  operationId: '&&&list'\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections\n  method: post\n  operationId: '&&&add'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{id}\n  method: get\n  operationId: '&&&retrieve'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{id}\n  method: patch\n  operationId: '&&&update'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/connections/{id}\n  method: delete\n  operationId: '&&&remove'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/generate\n  method: post\n  operationId: '&&&&$$generateDocument'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/templates\n  method: get\n  operationId: '&&&&$$list'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/templates\n\
  \  method: post\n  operationId: '&&&&$$create'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/templates/{id}\n  method: get\n  operationId: '&&&&$$retrieve'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/templates/{id}\n  method: patch\n  operationId: '&&&&$$update'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/templates/{id}\n  method: delete\n  operationId: '&&&&$$discard'\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/uploads\n  method: get\n  operationId: $$$$$&uploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/uploads\n  method: post\n  operationId: $$$$$&upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/uploads/{id}\n  method: get\n  operationId: $$$$$&retrieve_upload\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/manifests\n  method: get\n  operationId: $$$$&&list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/manifests\n  method: post\n  operationId: $$$$&&create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/manifests/{id}\n  method: get\n  operationId: $$$$&&retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/manifests/{id}/document\n  method: post\n  operationId: $$$$&&document\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders\n  method: get\n  operationId: '&&&&list'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders\n  method: post\n  operationId: '&&&&create'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{id}\n  method: get\n  operationId: '&&&&retrieve'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{id}\n  method: put\n  operationId: '&&&&update'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{id}\n  method: delete\n  operationId: '&&&&dismiss'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{id}/cancel\n  method: post\n  operationId: '&&&&cancel'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels\n  method: get\n  operationId: $$$list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcels\n  method: post\n  operationId: $$$create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels/{id}\n  method: get\n  operationId: $$$retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/parcels/{id}\n  method: patch\n  operationId: $$$update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parcels/{id}\n  method: delete\n  operationId: $$$discard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pickups\n  method: get\n  operationId: $$$$list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pickups\n  method: post\n  operationId: $$$$create\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pickups/{carrier_name}/schedule\n  method: post\n  operationId: $$$$schedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pickups/{id}\n  method: get\n  operationId: $$$$retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pickups/{id}\n  method: post\n  operationId: $$$$update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pickups/{id}/cancel\n  method: post\n  operationId: $$$$cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/products\n  method: get\n  operationId: $&list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products\n  method: post\n  operationId: $&create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/products/{id}\n  method: get\n  operationId: $&retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{id}\n  method: patch\n  operationId: $&update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/products/{id}\n  method: delete\n  operationId: $&discard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proxy/manifest\n\
  \  method: post\n  operationId: '@@@$generate_manifest'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proxy/pickups/{carrier_name}\n  method: post\n  operationId: '@schedule_pickup'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proxy/pickups/{carrier_name}/cancel\n  method: post\n  operationId: '@cancel_pickup'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proxy/pickups/{carrier_name}/update\n  method: post\n  operationId: '@update_pickup'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proxy/rates\n  method: post\n  operationId: '@@fetch_rates'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proxy/shipping\n  method: post\n  operationId: '@@@buy_label'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proxy/shipping/{carrier_name}/cancel\n  method: post\n  operationId: '@@@void_label'\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proxy/tracking\n  method: post\n  operationId: '@@@@get_tracking'\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/proxy/tracking/{carrier_name}/{tracking_number}\n  method: get\n  operationId: '@@@@track_shipment'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/references\n  method: get\n  operationId: '&&data'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments\n  method: get\n  operationId: $$$$$list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments\n  method: post\n  operationId: $$$$$create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipments/{id}\n  method: get\n  operationId: $$$$$retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments/{id}\n  method: put\n  operationId: $$$$$update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipments/{id}/cancel\n  method: post\n  operationId: $$$$$cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipments/{id}/documents/{doc}\n  method: post\n  operationId: $$$$$document\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipments/{id}/purchase\n  method: post\n  operationId: $$$$$purchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipments/{id}/rates\n\
  \  method: post\n  operationId: $$$$$rates\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trackers\n  method: get\n  operationId: $$$$$$list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trackers\n  method: post\n  operationId: $$$$$$add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trackers/{carrier_name}/{tracking_number}\n  method: get\n  operationId:\
  \ $$$$$$create\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trackers/{identifier}\n  method: get\n  operationId: $$$$$$retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trackers/{identifier}\n  method: put\n  operationId: $$$$$$update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trackers/{identifier}\n  method: delete\n  operationId: $$$$$$remove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trackers/{tracker_id}/inject-events\n  method: post\n  operationId: $$$$$$inject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: $$$$$$$list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: $$$$$$$create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /v1/webhooks/{id}\n  method: get\n  operationId: $$$$$$$retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method: patch\n  operationId: $$$$$$$update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: $$$$$$$remove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}/test\n  method: post\n  operationId:\
  \ $$$$$$$test\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/agentic-access/karrio-agentic-access.yml
summary_line: 95 operations · 60 acting
tags:
- Shipping
- Logistics
- Label Generation
- Package Tracking
- Carriers
- Fulfillment
- Open-Source
- Multi-Carrier
- Rating
- Webhook
---
