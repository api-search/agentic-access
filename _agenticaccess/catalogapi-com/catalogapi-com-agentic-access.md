---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 18
api_specs:
- filename: catalogapi-com-cart-api-openapi.yml
  format: yaml
  label: catalogapi-com Cart API
  slug: catalogapi-com-cart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-cart-api-openapi.yml
- filename: catalogapi-com-catalog-api-openapi.yml
  format: yaml
  label: catalogapi-com Catalog API
  slug: catalogapi-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-catalog-api-openapi.yml
- filename: catalogapi-com-health-api-openapi.yml
  format: yaml
  label: catalogapi-com Health API
  slug: catalogapi-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-health-api-openapi.yml
- filename: catalogapi-com-order-api-openapi.yml
  format: yaml
  label: catalogapi-com Order API
  slug: catalogapi-com-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catalogapi-com/openapi/catalogapi-com-order-api-openapi.yml
consequence_counts:
  read: 18
  safety-critical: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Catalogapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sockets/{socket_id}/cart/{external_user_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sockets/{socket_id}/cart/{external_user_id}/empty
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /sockets/{socket_id}/cart/{external_user_id}/line_items/{line_item_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /sockets/{socket_id}/cart/{external_user_id}/line_items/{line_item_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sockets/{socket_id}/cart/{external_user_id}/line_items/{line_item_id}/revalidate_stock
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /sockets/{socket_id}/cart/{external_user_id}/metadata
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sockets/{socket_id}/cart/{external_user_id}/order_place
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sockets/{socket_id}/cart/{external_user_id}/set_address
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sockets/{socket_id}/cart/{external_user_id}/unlock
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sockets/{socket_id}/cart/{external_user_id}/validate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sockets/{socket_id}/orders/place_direct
operation_count: 29
overview: 'catalogapi-com exposes 29 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: catalogapi-com
provider_slug: catalogapi-com
slug: catalogapi-com-agentic-access
source_filename: catalogapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/catalogapi-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 18\n    acting: 11\n  by_consequence:\n    read: 18\n    safety-critical: 11\n  human_in_the_loop_required: 11\noperations:\n- path: /external_users/{external_user_id}/orders\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.OrderController.get_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{external_order_id}\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.OrderController.track_order\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.HealthController.ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /redemption_active\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.OrderController.redemption_active\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.show\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/brands\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.brands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/cart/{external_user_id}\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.view_cart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/cart/{external_user_id}\n  method: post\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.add_item\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/cart/{external_user_id}/empty\n  method: post\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.empty_cart\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/cart/{external_user_id}/line_items/{line_item_id}\n  method: delete\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.remove_line_item\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/cart/{external_user_id}/line_items/{line_item_id}\n  method: put\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.update_line_item\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/cart/{external_user_id}/line_items/{line_item_id}/revalidate_stock\n  method: post\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.revalidate_stock\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /sockets/{socket_id}/cart/{external_user_id}/metadata\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.get_metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/cart/{external_user_id}/metadata\n  method: put\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.update_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/cart/{external_user_id}/order_place\n  method: post\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.place_order\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/cart/{external_user_id}/set_address\n  method: post\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.set_address\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/cart/{external_user_id}/unlock\n  method: post\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.unlock_cart\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/cart/{external_user_id}/validate\n  method: post\n  operationId: CatalogAPIWeb.Api.Controllers.CartController.validate_cart\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/categories\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/categories/tag/{tag_id}\n  method:\
  \ get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.categories_by_tag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/item_types\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.item_types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/items\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/items/search\n  method: post\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.items_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/items/{catalog_item_id}\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.item_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/items/{catalog_item_id}/stock\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.item_stock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/marketing\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.marketing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sockets/{socket_id}/orders/place_direct\n  method: post\n  operationId:\
  \ CatalogAPIWeb.Api.Controllers.OrderController.place_direct_order\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sockets/{socket_id}/tags\n  method: get\n  operationId: CatalogAPIWeb.Api.Controllers.SocketsController.tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/catalogapi-com/agentic-access/catalogapi-com-agentic-access.yml
summary_line: 29 operations · 11 acting · 11 human-in-the-loop
tags:
- Company
- Rewards
- Gift Cards
- Global
---
