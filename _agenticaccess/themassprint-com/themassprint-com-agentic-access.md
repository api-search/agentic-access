---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: themassprint-com-catalog-api-openapi.yml
  format: yaml
  label: themassprint-com Catalog API
  slug: themassprint-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/themassprint-com/openapi/themassprint-com-catalog-api-openapi.yml
- filename: themassprint-com-enterprise-api-openapi.yml
  format: yaml
  label: themassprint-com Enterprise API
  slug: themassprint-com-enterprise-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/themassprint-com/openapi/themassprint-com-enterprise-api-openapi.yml
- filename: themassprint-com-health-api-openapi.yml
  format: yaml
  label: themassprint-com Health API
  slug: themassprint-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/themassprint-com/openapi/themassprint-com-health-api-openapi.yml
- filename: themassprint-com-orders-api-openapi.yml
  format: yaml
  label: themassprint-com Orders API
  slug: themassprint-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/themassprint-com/openapi/themassprint-com-orders-api-openapi.yml
- filename: themassprint-com-uploads-api-openapi.yml
  format: yaml
  label: themassprint-com Uploads API
  slug: themassprint-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/themassprint-com/openapi/themassprint-com-uploads-api-openapi.yml
- filename: themassprint-com-webhook-endpoints-api-openapi.yml
  format: yaml
  label: themassprint-com Webhook Endpoints API
  slug: themassprint-com-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/themassprint-com/openapi/themassprint-com-webhook-endpoints-api-openapi.yml
consequence_counts:
  physical: 3
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Themassprint Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/enterprise/apply
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{id}/cancel
operation_count: 12
overview: 'themassprint-com exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 4 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: themassprint-com
provider_slug: themassprint-com
slug: themassprint-com-agentic-access
source_filename: themassprint-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/themassprint-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 5\n    acting: 7\n  by_consequence:\n    read: 5\n    write: 4\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/catalog\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/uploads\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/uploads/{id}/content\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/{id}/validation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{id}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{id}/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/webhook-endpoints/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enterprise/apply\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/themassprint-com/agentic-access/themassprint-com-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Print on Demand
- AI Agents
- E-Commerce
- India
---
