---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: sitegrab-screenshot-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API
  slug: sitegrab-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-screenshot-api-openapi.yml
- filename: sitegrab-checkout-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Checkout API
  slug: sitegrab-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-checkout-api-openapi.yml
- filename: sitegrab-docs-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Docs API
  slug: sitegrab-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-docs-api-openapi.yml
- filename: sitegrab-health-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Health API
  slug: sitegrab-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-health-api-openapi.yml
- filename: sitegrab-keys-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Keys API
  slug: sitegrab-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-keys-api-openapi.yml
- filename: sitegrab-screenshot-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Screenshot API
  slug: sitegrab-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-screenshot-api-openapi.yml
- filename: sitegrab-signup-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Signup API
  slug: sitegrab-signup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-signup-api-openapi.yml
- filename: sitegrab-sitegrab-screenshot-api-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) SiteGrab Screenshot API
  slug: sitegrab-sitegrab-screenshot-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-sitegrab-screenshot-api-api-openapi.yml
- filename: sitegrab-usage-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Usage API
  slug: sitegrab-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-usage-api-openapi.yml
- filename: sitegrab-webhook-api-openapi.yml
  format: yaml
  label: SiteGrab Screenshot API (LaminarForge) Webhook API
  slug: sitegrab-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/openapi/sitegrab-webhook-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sitegrab Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout
operation_count: 10
overview: 'SiteGrab Screenshot API (LaminarForge) exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SiteGrab Screenshot API (LaminarForge)
provider_slug: sitegrab
slug: sitegrab-agentic-access
source_filename: sitegrab-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/sitegrab-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 4\n    connected: 6\n  by_consequence:\n    write: 3\n    read: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/screenshot\n  method: post\n  operationId: captureScreenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screenshot\n  method: get\n  operationId: quickScreenshot\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook\n  method: post\n  operationId: stripeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /docs\n  method: get\n  operationId: getDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signup\n  method: get\n  operationId: getSignup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /\n  method: get\n  operationId: getHome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitegrab/refs/heads/main/agentic-access/sitegrab-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Screenshots
- Automation
- Image
- Web
---
