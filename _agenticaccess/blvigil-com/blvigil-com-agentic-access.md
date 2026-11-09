---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 7
api_specs:
- filename: blvigil-com-agent-api-openapi.yml
  format: yaml
  label: Vigil Agent API
  slug: blvigil-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvigil-com/openapi/blvigil-com-agent-api-openapi.yml
- filename: blvigil-com-mcp-api-openapi.yml
  format: yaml
  label: Vigil MCP API
  slug: blvigil-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvigil-com/openapi/blvigil-com-mcp-api-openapi.yml
consequence_counts:
  physical: 8
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blvigil Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agent/commerce/acp/checkout_sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agent/commerce/ucp/checkout-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /agent/commerce/ucp/checkout-sessions/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agent/commerce/ucp/checkout-sessions/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /agent/commerce/ucp/checkout-sessions/{id}/complete
operation_count: 16
overview: 'Vigil exposes 16 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 1 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vigil
provider_slug: blvigil-com
slug: blvigil-com-agentic-access
source_filename: blvigil-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/blvigil-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 7\n    acting: 9\n  by_consequence:\n    read: 7\n    write: 1\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /agent/site.json\n  method: get\n  operationId: siteInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/search\n  method: get\n  operationId: searchPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/read\n  method:\
  \ get\n  operationId: readPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/commerce/ucp/checkout-sessions\n  method: post\n  operationId: ucpCreateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/ucp/checkout-sessions/{id}\n  method: get\n  operationId: ucpGetCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/commerce/ucp/checkout-sessions/{id}\n  method: put\n  operationId: ucpUpdateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/ucp/checkout-sessions/{id}/complete\n  method: post\n  operationId: ucpCompleteCheckout\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/ucp/checkout-sessions/{id}/cancel\n  method: post\n  operationId: ucpCancelCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/acp/checkout_sessions\n  method: post\n  operationId: acpCreateCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}\n  method: get\n  operationId: acpGetCheckoutSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}\n  method: post\n  operationId: acpUpdateCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}/complete\n  method: post\n  operationId: acpCompleteCheckoutSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}/cancel\n  method: post\n  operationId: acpCancelCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/continue/{checkout_id}\n  method: get\n  operationId: continueCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/blvigil-com/agentic-access/blvigil-com-agentic-access.yml
summary_line: 16 operations · 9 acting
tags:
- Home Automation
- Security
- Smart Home
- Software
- Mac
- Windows
---
