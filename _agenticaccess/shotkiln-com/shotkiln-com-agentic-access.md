---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 5
api_specs:
- filename: shotkiln-com-billing-api-openapi.yml
  format: yaml
  label: shotkiln-com Billing API
  slug: shotkiln-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkiln-com/openapi/shotkiln-com-billing-api-openapi.yml
- filename: shotkiln-com-checkout-api-openapi.yml
  format: yaml
  label: shotkiln-com Checkout API
  slug: shotkiln-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkiln-com/openapi/shotkiln-com-checkout-api-openapi.yml
- filename: shotkiln-com-keys-api-openapi.yml
  format: yaml
  label: shotkiln-com Keys API
  slug: shotkiln-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkiln-com/openapi/shotkiln-com-keys-api-openapi.yml
- filename: shotkiln-com-mcp-api-openapi.yml
  format: yaml
  label: shotkiln-com MCP API
  slug: shotkiln-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkiln-com/openapi/shotkiln-com-mcp-api-openapi.yml
- filename: shotkiln-com-og-api-openapi.yml
  format: yaml
  label: shotkiln-com Og API
  slug: shotkiln-com-og-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkiln-com/openapi/shotkiln-com-og-api-openapi.yml
- filename: shotkiln-com-pdf-api-openapi.yml
  format: yaml
  label: shotkiln-com PDF API
  slug: shotkiln-com-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkiln-com/openapi/shotkiln-com-pdf-api-openapi.yml
- filename: shotkiln-com-screenshot-api-openapi.yml
  format: yaml
  label: shotkiln-com Screenshot API
  slug: shotkiln-com-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkiln-com/openapi/shotkiln-com-screenshot-api-openapi.yml
- filename: shotkiln-com-usage-api-openapi.yml
  format: yaml
  label: shotkiln-com Usage API
  slug: shotkiln-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkiln-com/openapi/shotkiln-com-usage-api-openapi.yml
consequence_counts:
  physical: 2
  read: 5
  safety-critical: 3
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Shotkiln Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/keys/recover
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/keys/rotate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/keys/signing-secret/rotate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/portal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout
operation_count: 16
overview: 'shotkiln-com exposes 16 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 6 write, 2 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: shotkiln-com
provider_slug: shotkiln-com
slug: shotkiln-com-agentic-access
source_filename: shotkiln-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/shotkiln-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 5\n    acting: 11\n  by_consequence:\n    read: 5\n    write: 6\n    safety-critical: 3\n    physical: 2\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/screenshot\n  method: get\n  operationId: screenshotGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/screenshot\n  method: post\n  operationId: screenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pdf\n  method: get\n  operationId: pdfGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pdf\n  method: post\n  operationId: pdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/og\n  method: get\n  operationId: ogImageGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/og\n  method: post\n  operationId: ogImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/og/sign\n  method: post\n  operationId: signOgUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/signing-secret\n  method: post\n  operationId: getSigningSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/signing-secret/rotate\n  method: post\n  operationId: rotateSigningSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: createFreeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/rotate\n  method: post\n  operationId: rotateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/keys/recover\n  method: post\n  operationId: recoverKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: billingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout\n  method: post\n  operationId: checkout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/shotkiln-com/agentic-access/shotkiln-com-agentic-access.yml
summary_line: 16 operations · 11 acting · 3 human-in-the-loop
tags:
- Company
- Screenshots
- Web
- Automation
---
