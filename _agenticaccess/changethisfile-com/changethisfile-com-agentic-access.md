---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 3
api_specs:
- filename: changethisfile-com-account-api-openapi.yml
  format: yaml
  label: ChangeThisFile Account API
  slug: changethisfile-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changethisfile-com/openapi/changethisfile-com-account-api-openapi.yml
- filename: changethisfile-com-billing-api-openapi.yml
  format: yaml
  label: ChangeThisFile Billing API
  slug: changethisfile-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changethisfile-com/openapi/changethisfile-com-billing-api-openapi.yml
- filename: changethisfile-com-conversions-api-openapi.yml
  format: yaml
  label: ChangeThisFile Conversions API
  slug: changethisfile-com-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changethisfile-com/openapi/changethisfile-com-conversions-api-openapi.yml
- filename: changethisfile-com-jobs-api-openapi.yml
  format: yaml
  label: ChangeThisFile Jobs API
  slug: changethisfile-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changethisfile-com/openapi/changethisfile-com-jobs-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Changethisfile Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 9
overview: 'ChangeThisFile exposes 9 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ChangeThisFile
provider_slug: changethisfile-com
slug: changethisfile-com-agentic-access
source_filename: changethisfile-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/changethisfile-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 6\n    connected: 3\n  by_consequence:\n    write: 5\n    read: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/convert\n  method: post\n  operationId: convertFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{job_id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/free\n  method: post\n  operationId: createFreeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout\n  method: post\n  operationId: createCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: openBillingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/stripe\n\
  \  method: post\n  operationId: stripeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/changethisfile-com/agentic-access/changethisfile-com-agentic-access.yml
summary_line: 9 operations · 6 acting
tags:
- File Conversion
- Free
- Privacy
- Software-as-a-Service
---
