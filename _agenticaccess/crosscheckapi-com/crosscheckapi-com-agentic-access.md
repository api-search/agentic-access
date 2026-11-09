---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 4
api_specs:
- filename: crosscheckapi-com-accept-api-openapi.yml
  format: yaml
  label: Crosscheck Accept API
  slug: crosscheckapi-com-accept-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-accept-api-openapi.yml
- filename: crosscheckapi-com-accept-lite-api-openapi.yml
  format: yaml
  label: Crosscheck Accept Lite API
  slug: crosscheckapi-com-accept-lite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-accept-lite-api-openapi.yml
- filename: crosscheckapi-com-acceptance-test-api-openapi.yml
  format: yaml
  label: Crosscheck acceptance test API
  slug: crosscheckapi-com-acceptance-test-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-acceptance-test-api-openapi.yml
- filename: crosscheckapi-com-checks-api-openapi.yml
  format: yaml
  label: Crosscheck Checks API
  slug: crosscheckapi-com-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-checks-api-openapi.yml
- filename: crosscheckapi-com-draft-review-api-openapi.yml
  format: yaml
  label: Crosscheck draft review API
  slug: crosscheckapi-com-draft-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-draft-review-api-openapi.yml
- filename: crosscheckapi-com-quote-api-openapi.yml
  format: yaml
  label: Crosscheck Quote API
  slug: crosscheckapi-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-quote-api-openapi.yml
- filename: crosscheckapi-com-receipts-api-openapi.yml
  format: yaml
  label: Crosscheck Receipts API
  slug: crosscheckapi-com-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-receipts-api-openapi.yml
- filename: crosscheckapi-com-sellercheck-api-openapi.yml
  format: yaml
  label: Crosscheck Sellercheck API
  slug: crosscheckapi-com-sellercheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-sellercheck-api-openapi.yml
- filename: crosscheckapi-com-sellerwatch-api-openapi.yml
  format: yaml
  label: Crosscheck Sellerwatch API
  slug: crosscheckapi-com-sellerwatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-sellerwatch-api-openapi.yml
- filename: crosscheckapi-com-skill-security-api-openapi.yml
  format: yaml
  label: Crosscheck skill security API
  slug: crosscheckapi-com-skill-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-skill-security-api-openapi.yml
- filename: crosscheckapi-com-skillcheck-api-openapi.yml
  format: yaml
  label: Crosscheck Skillcheck API
  slug: crosscheckapi-com-skillcheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-skillcheck-api-openapi.yml
- filename: crosscheckapi-com-skillcheck-lite-api-openapi.yml
  format: yaml
  label: Crosscheck Skillcheck Lite API
  slug: crosscheckapi-com-skillcheck-lite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-skillcheck-lite-api-openapi.yml
- filename: crosscheckapi-com-w-api-openapi.yml
  format: yaml
  label: Crosscheck W API
  slug: crosscheckapi-com-w-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-w-api-openapi.yml
- filename: crosscheckapi-com-x402-seller-api-openapi.yml
  format: yaml
  label: Crosscheck x402 seller API
  slug: crosscheckapi-com-x402-seller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosscheckapi-com/openapi/crosscheckapi-com-x402-seller-api-openapi.yml
consequence_counts:
  read: 4
  safety-critical: 4
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Crosscheckapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/skillcheck
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/skillcheck-lite
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/skillcheck-lite/quote
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/skillcheck/quote
operation_count: 19
overview: 'Crosscheck exposes 19 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 11 write, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crosscheck
provider_slug: crosscheckapi-com
slug: crosscheckapi-com-agentic-access
source_filename: crosscheckapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/crosscheckapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 15\n    connected: 4\n  by_consequence:\n    write: 11\n    safety-critical: 4\n    read: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /v1/check\n  method: post\n  operationId: check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accept\n  method: post\n  operationId: accept\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accept/quote\n  method: post\n  operationId: acceptQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/skillcheck\n  method: post\n  operationId: skillcheck\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/skillcheck/quote\n  method: post\n\
  \  operationId: skillcheckQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/accept-lite\n  method: post\n  operationId: acceptLite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accept-lite/quote\n  method: post\n  operationId: acceptLiteQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/skillcheck-lite\n  method: post\n  operationId: skillcheckLite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/skillcheck-lite/quote\n  method: post\n  operationId: skillcheckLiteQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sellercheck\n  method: post\n  operationId: sellercheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sellercheck/quote\n  method: post\n  operationId: sellercheckQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sellercheck/preflight\n  method: get\n  operationId: sellercheckPreflight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sellerwatch\n  method: post\n  operationId: sellerwatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sellerwatch/quote\n  method: post\n  operationId: sellerwatchQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{watch_id}.json\n  method: get\n  operationId: watchRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/skillcheck/{bundle_sha256}\n  method: get\n  operationId: skillcheckLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receipts/verify\n  method: post\n  operationId: verifyReceipt\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quote\n  method: post\n  operationId: quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checks/{job_id}\n  method: get\n  operationId: result\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/crosscheckapi-com/agentic-access/crosscheckapi-com-agentic-access.yml
summary_line: 19 operations · 15 acting · 4 human-in-the-loop
tags:
- Artificial Intelligence
- Verification
- Payments
- x402
- Blockchain
---
