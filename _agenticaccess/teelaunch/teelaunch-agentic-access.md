---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 24
api_specs:
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Account API
  slug: teelaunch-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Blank Catalog API
  slug: teelaunch-blank-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Products API
  slug: teelaunch-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Orders API
  slug: teelaunch-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Shipping & Tracking API
  slug: teelaunch-shipping-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
- filename: teelaunch-openapi.yml
  format: yaml
  label: Teelaunch Platforms & Stores API
  slug: teelaunch-platforms-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-openapi.yml
consequence_counts:
  physical: 5
  read: 24
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Teelaunch Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/pro
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{id}/hold
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{id}/release
operation_count: 36
overview: 'Teelaunch exposes 36 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 7 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Teelaunch
provider_slug: teelaunch
slug: teelaunch-agentic-access
source_filename: teelaunch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/teelaunch-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 24\n    acting: 12\n  by_consequence:\n    read: 24\n    write: 7\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /account\n  method: get\n  operationId: 2568f6551774f5a58a2e1b7e5aad8115\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/payment-history\n  method: get\n  operationId: ad402e84d315e0489a7293ad6c657278\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /account/payment-history/{id}\n  method: get\n  operationId: d0f6b4a170c810850fa4232399e6dddb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/settings\n  method: get\n  operationId: 36147cdcf2d975057c6846c7a43a481b\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/settings/{id}\n  method: get\n  operationId: 849c2a043635e8e054c3cfb802078d84\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/settings/{accountId}\n  method: put\n  operationId: b3d49efa73678cddfc3a06c3da79a875\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories\n  method: get\n  operationId: 3cf29949d6a59edf1bfbdca9319518d9\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{id}\n  method: get\n  operationId: 7bd6346eeb8f9e067822a1bb5e554f97\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{id}/blanks\n  method: get\n  operationId: a7238e30037699428ecc2f0a35538f48\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blanks\n  method: get\n  operationId: f33ed3c07d628928c695d015706213e2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /blanks/{id}\n  method: get\n  operationId: 4073123195b174f93c22a2e39ba43e84\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blanks/country/shipping/cost/{id}\n  method: get\n  operationId: 9c109d7727861f3df589d68698789840\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blanks/{id}/create\n  method: post\n  operationId: b8af01928da4a18ca202e09b28f49041\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: 2f71f731d00917eaf4cf488100ee4a68\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: 2bbb6d29d3345bb1d0d38877b33030f0\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}\n  method: get\n  operationId: 50d90d5c46e6459e22cbd89ca05e879f\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}/cancel\n  method: post\n  operationId: 59facf5d09499d6376eb0c9731cdb736\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}/release\n  method: post\n  operationId: 3a94a0e0d5c256d26f33cd58de6fab66\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}/hold\n  method: post\n  operationId: d29a3a373c10dfb35f2d71743c9b20cd\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /orders/pro\n  method: post\n  operationId: d8d545a21521bc4d460011d0f946ddbe\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}/shipments\n  method: get\n  operationId: 240dd75ed623c423755bef1843635581\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/line-item/{id}/shipments\n  method: get\n  operationId: b7e91b64cf7a7b7cf6d4018b3bdcdb69\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/platform/{id}/shipments\n\
  \  method: get\n  operationId: d5e42a4442f4058bb2830cc58e623f97\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms\n  method: get\n  operationId: ea7be5e215e4581e1c38dc5a9c7414ef\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/{id}\n  method: get\n  operationId: cc3d714e5f357e1dbe48c1dfd6c64ff1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores\n  method: get\n  operationId: 029dfe0bb9acd7df4230201a637a1ac1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{id}\n  method: get\n  operationId: 5ebb71f384e9969ae7bfca07c4cf7450\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/products/variants/{id}/unlink\n  method: post\n  operationId: dbbcc24e2bc2247f2f013ea856fdb091\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/products/variants/{id}/ignore\n  method: post\n  operationId: 4c4c73196aad959c84a922c39cf1be8e\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/products/variants/{id}/unignore\n  method: post\n  operationId: 988135adcca30eef5d9d08bc0930b695\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{platformStoreId}/products/{id}\n  method: get\n  operationId: 3fa7a6faf46bb48fd6a78c2a133d7cf8\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{platformStoreId}/products\n  method: get\n  operationId: aeb6e9973ad802d72917350ef1b41e2d\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stores/{platformStoreId}/products/{id}/ignore\n  method: post\n  operationId: 2636ded800a48cf2f66eefa4db1cf915\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stores/{platformStoreId}/products/{id}/unignore\n  method: post\n  operationId: 9f1bf75602027f29bba07b1ffb89d345\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products\n  method: get\n  operationId: cbd3820f1c54e85489d86c79c20ec741\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{id}\n  method: get\n  operationId: 163fa1b107c906fbd20e5a804078dfa4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/agentic-access/teelaunch-agentic-access.yml
summary_line: 36 operations · 12 acting
tags:
- Print on Demand
- POD
- Ecommerce
- Fulfillment
- Dropshipping
- Orders
- Shipping
---
