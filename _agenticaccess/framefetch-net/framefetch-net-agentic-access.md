---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 9
api_specs:
- filename: framefetch-net-account-api-openapi.yml
  format: yaml
  label: framefetch-net Account API
  slug: framefetch-net-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-account-api-openapi.yml
- filename: framefetch-net-batch-api-openapi.yml
  format: yaml
  label: framefetch-net Batch API
  slug: framefetch-net-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-batch-api-openapi.yml
- filename: framefetch-net-billing-api-openapi.yml
  format: yaml
  label: framefetch-net Billing API
  slug: framefetch-net-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-billing-api-openapi.yml
- filename: framefetch-net-checkout-api-openapi.yml
  format: yaml
  label: framefetch-net Checkout API
  slug: framefetch-net-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-checkout-api-openapi.yml
- filename: framefetch-net-demo-api-openapi.yml
  format: yaml
  label: framefetch-net Demo API
  slug: framefetch-net-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-demo-api-openapi.yml
- filename: framefetch-net-extract-api-openapi.yml
  format: yaml
  label: framefetch-net Extract API
  slug: framefetch-net-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-extract-api-openapi.yml
- filename: framefetch-net-framefetch-api-api-openapi.yml
  format: yaml
  label: framefetch-net FrameFetch API
  slug: framefetch-net-framefetch-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-framefetch-api-api-openapi.yml
- filename: framefetch-net-frames-api-openapi.yml
  format: yaml
  label: framefetch-net Frames API
  slug: framefetch-net-frames-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-frames-api-openapi.yml
- filename: framefetch-net-healthz-api-openapi.yml
  format: yaml
  label: framefetch-net Healthz API
  slug: framefetch-net-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-healthz-api-openapi.yml
- filename: framefetch-net-keys-api-openapi.yml
  format: yaml
  label: framefetch-net Keys API
  slug: framefetch-net-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-keys-api-openapi.yml
- filename: framefetch-net-metadata-api-openapi.yml
  format: yaml
  label: framefetch-net Metadata API
  slug: framefetch-net-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-metadata-api-openapi.yml
- filename: framefetch-net-platforms-api-openapi.yml
  format: yaml
  label: framefetch-net Platforms API
  slug: framefetch-net-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-platforms-api-openapi.yml
- filename: framefetch-net-status-api-openapi.yml
  format: yaml
  label: framefetch-net Status API
  slug: framefetch-net-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-status-api-openapi.yml
- filename: framefetch-net-transcript-api-openapi.yml
  format: yaml
  label: framefetch-net Transcript API
  slug: framefetch-net-transcript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-transcript-api-openapi.yml
- filename: framefetch-net-usage-api-openapi.yml
  format: yaml
  label: framefetch-net Usage API
  slug: framefetch-net-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-usage-api-openapi.yml
- filename: framefetch-net-watch-api-openapi.yml
  format: yaml
  label: framefetch-net Watch API
  slug: framefetch-net-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-watch-api-openapi.yml
- filename: framefetch-net-top-up-api-openapi.yml
  format: yaml
  label: framefetch-net Top Up API
  slug: framefetch-net-top-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/framefetch-net/openapi/framefetch-net-top-up-api-openapi.yml
consequence_counts:
  physical: 4
  read: 9
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Framefetch Net Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/auto-topup
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
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/topup
operation_count: 19
overview: 'framefetch-net exposes 19 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 6 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: framefetch-net
provider_slug: framefetch-net
slug: framefetch-net-agentic-access
source_filename: framefetch-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/framefetch-net-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 10\n    connected: 9\n  by_consequence:\n    write: 6\n    read: 9\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extract\n  method: post\n  operationId: extract\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch\n  method: post\n  operationId: batchExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watch\n  method: get\n  operationId: listWatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watch\n  method: post\n  operationId: createWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watch/{id}\n  method: delete\n  operationId: deleteWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/metadata\n  method: post\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcript\n  method: post\n  operationId: getTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/frames\n  method: post\n  operationId: getFrames\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platforms\n  method: get\n  operationId: listPlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topup\n  method: post\n  operationId: topup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: createBillingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/auto-topup\n  method: post\n  operationId: configureAutoTopup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/demo\n  method: post\n  operationId: demo\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/framefetch-net/agentic-access/framefetch-net-agentic-access.yml
summary_line: 19 operations · 10 acting
tags:
- Company
- Video
- Artificial Intelligence
- Data API
- Media
---
