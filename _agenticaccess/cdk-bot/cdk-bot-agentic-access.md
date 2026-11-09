---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: cdk-bot-games-api-openapi.yml
  format: yaml
  label: CDK Bot Games API
  slug: cdk-bot-games-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cdk-bot/openapi/cdk-bot-games-api-openapi.yml
- filename: cdk-bot-meta-api-openapi.yml
  format: yaml
  label: CDK Bot Meta API
  slug: cdk-bot-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cdk-bot/openapi/cdk-bot-meta-api-openapi.yml
- filename: cdk-bot-orders-api-openapi.yml
  format: yaml
  label: CDK Bot Orders API
  slug: cdk-bot-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cdk-bot/openapi/cdk-bot-orders-api-openapi.yml
- filename: cdk-bot-purchase-api-openapi.yml
  format: yaml
  label: CDK Bot Purchase API
  slug: cdk-bot-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cdk-bot/openapi/cdk-bot-purchase-api-openapi.yml
- filename: cdk-bot-refunds-api-openapi.yml
  format: yaml
  label: CDK Bot Refunds API
  slug: cdk-bot-refunds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cdk-bot/openapi/cdk-bot-refunds-api-openapi.yml
- filename: cdk-bot-status-api-openapi.yml
  format: yaml
  label: CDK Bot Status API
  slug: cdk-bot-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cdk-bot/openapi/cdk-bot-status-api-openapi.yml
consequence_counts:
  physical: 2
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cdk Bot Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refund
operation_count: 13
overview: 'CDK Bot exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CDK Bot
provider_slug: cdk-bot
slug: cdk-bot-agentic-access
source_filename: cdk-bot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cdk-bot-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 11\n    acting: 2\n  by_consequence:\n    read: 11\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /games\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /games/match\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /games/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchase\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}/receipt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refund\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n  \
  \    exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /platforms\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product-types\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /languages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cdk-bot/agentic-access/cdk-bot-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Digital Products
- Crypto Payments
- Autonomous Agents
---
