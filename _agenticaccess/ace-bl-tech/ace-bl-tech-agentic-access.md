---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 21
api_specs:
- filename: ace-bl-tech-agent-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Agent API
  slug: ace-bl-tech-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-agent-api-openapi.yml
- filename: ace-bl-tech-apps-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Apps API
  slug: ace-bl-tech-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-apps-api-openapi.yml
- filename: ace-bl-tech-catalog-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Catalog API
  slug: ace-bl-tech-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-catalog-api-openapi.yml
- filename: ace-bl-tech-connections-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Connections API
  slug: ace-bl-tech-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-connections-api-openapi.yml
- filename: ace-bl-tech-custom-connectors-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Custom Connectors API
  slug: ace-bl-tech-custom-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-custom-connectors-api-openapi.yml
- filename: ace-bl-tech-events-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Events API
  slug: ace-bl-tech-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-events-api-openapi.yml
- filename: ace-bl-tech-mcp-api-openapi.yml
  format: yaml
  label: Ace AI Assistant MCP API
  slug: ace-bl-tech-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-mcp-api-openapi.yml
- filename: ace-bl-tech-me-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Me API
  slug: ace-bl-tech-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-me-api-openapi.yml
- filename: ace-bl-tech-runs-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Runs API
  slug: ace-bl-tech-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-runs-api-openapi.yml
- filename: ace-bl-tech-tools-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Tools API
  slug: ace-bl-tech-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-tools-api-openapi.yml
- filename: ace-bl-tech-triggers-api-openapi.yml
  format: yaml
  label: Ace AI Assistant Triggers API
  slug: ace-bl-tech-triggers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ace-bl-tech/openapi/ace-bl-tech-triggers-api-openapi.yml
consequence_counts:
  physical: 8
  read: 21
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Ace Bl Tech Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/triggers/{id}
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
operation_count: 38
overview: 'Ace AI Assistant exposes 38 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 8 write, 8 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ace AI Assistant
provider_slug: ace-bl-tech
slug: ace-bl-tech-agentic-access
source_filename: ace-bl-tech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/ace-bl.tech-openapi.json, openapi/tryacee.com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 21\n    acting: 17\n  by_consequence:\n    read: 21\n    write: 8\n    physical: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /agent/site.json\n  method: get\n  operationId: siteInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/search\n  method: get\n  operationId: searchPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /agent/read\n  method: get\n  operationId: readPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/commerce/ucp/checkout-sessions\n  method: post\n  operationId: ucpCreateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/ucp/checkout-sessions/{id}\n  method: get\n  operationId: ucpGetCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/commerce/ucp/checkout-sessions/{id}\n  method: put\n  operationId: ucpUpdateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/ucp/checkout-sessions/{id}/complete\n  method: post\n  operationId: ucpCompleteCheckout\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/ucp/checkout-sessions/{id}/cancel\n  method: post\n  operationId: ucpCancelCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/acp/checkout_sessions\n  method: post\n  operationId: acpCreateCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}\n  method: get\n  operationId: acpGetCheckoutSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}\n  method: post\n  operationId: acpUpdateCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}/complete\n\
  \  method: post\n  operationId: acpCompleteCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/acp/checkout_sessions/{checkout_session_id}/cancel\n  method: post\n  operationId: acpCancelCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/commerce/continue/{checkout_id}\n  method: get\n  operationId: continueCheckout\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/catalog\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app}/connect\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{app}/request\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/connections\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/connections/{connectionId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/find\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/{tool}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/{tool}/run\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/custom-connectors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/custom-connectors\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/custom-connectors/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/triggers/types\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/triggers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/triggers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/triggers/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/runs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ace-bl-tech/agentic-access/ace-bl-tech-agentic-access.yml
summary_line: 38 operations · 17 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Productivity
- Assistant
- macOS
- Windows
- iOS
---
