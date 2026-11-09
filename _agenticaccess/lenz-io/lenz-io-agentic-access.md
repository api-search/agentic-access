---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 11
api_specs:
- filename: lenz-io-account-api-openapi.yml
  format: yaml
  label: lenz-io Account API
  slug: lenz-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-account-api-openapi.yml
- filename: lenz-io-ask-api-openapi.yml
  format: yaml
  label: lenz-io Ask API
  slug: lenz-io-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-ask-api-openapi.yml
- filename: lenz-io-assess-api-openapi.yml
  format: yaml
  label: lenz-io Assess API
  slug: lenz-io-assess-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-assess-api-openapi.yml
- filename: lenz-io-citecheck-api-openapi.yml
  format: yaml
  label: lenz-io Citecheck API
  slug: lenz-io-citecheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-citecheck-api-openapi.yml
- filename: lenz-io-discovery-api-openapi.yml
  format: yaml
  label: lenz-io Discovery API
  slug: lenz-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-discovery-api-openapi.yml
- filename: lenz-io-extract-api-openapi.yml
  format: yaml
  label: lenz-io Extract API
  slug: lenz-io-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-extract-api-openapi.yml
- filename: lenz-io-lenz-ai-fact-checking-api-api-openapi.yml
  format: yaml
  label: lenz-io Lenz — AI Fact Checking API
  slug: lenz-io-lenz-ai-fact-checking-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-lenz-ai-fact-checking-api-api-openapi.yml
- filename: lenz-io-library-api-openapi.yml
  format: yaml
  label: lenz-io Library API
  slug: lenz-io-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-library-api-openapi.yml
- filename: lenz-io-review-api-openapi.yml
  format: yaml
  label: lenz-io Review API
  slug: lenz-io-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-review-api-openapi.yml
- filename: lenz-io-verifications-api-openapi.yml
  format: yaml
  label: lenz-io Verifications API
  slug: lenz-io-verifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-verifications-api-openapi.yml
- filename: lenz-io-verify-api-openapi.yml
  format: yaml
  label: lenz-io Verify API
  slug: lenz-io-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-verify-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Lenz Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/ask/{verification_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/ask/{verification_id}
operation_count: 24
overview: 'lenz-io exposes 24 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 11 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: lenz-io
provider_slug: lenz-io
slug: lenz-io-agentic-access
source_filename: lenz-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/lenz-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 11\n    acting: 13\n  by_consequence:\n    read: 11\n    write: 11\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/\n  method: get\n  operationId: apiRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/library\n  method: get\n  operationId: listLibrary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verify\n\
  \  method: post\n  operationId: submit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verify/batch\n  method: post\n  operationId: batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/assess\n  method: post\n  operationId: assess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/extract\n  method: post\n  operationId: extract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verify/{task_id}/select\n  method: post\n  operationId: select\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verify/status/{task_id}\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verify/{task_id}/cancel\n  method: post\n  operationId: cancel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verifications\n  method: get\n  operationId: listVerifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verifications/{verification_id}\n  method: get\n  operationId: getVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verifications/{verification_id}\n\
  \  method: delete\n  operationId: deleteVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verifications/{verification_id}/certificate\n  method: get\n  operationId: getCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verifications/{verification_id}/related\n  method: get\n  operationId: listRelated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ask/{verification_id}\n  method: get\n  operationId: getAskHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ask/{verification_id}\n  method: delete\n  operationId: resetAsk\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/ask/{verification_id}\n  method: post\n  operationId: sendAsk\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/review\n  method: post\n  operationId: review\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reviews/{review_id}\n  method: get\n  operationId: getReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reviews/{review_id}/cancel\n  method: post\n  operationId: cancelReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/citecheck\n  method: post\n  operationId: citecheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/citechecks/{citecheck_id}\n  method: get\n  operationId: getCitecheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/citechecks/{citecheck_id}/cancel\n  method: post\n  operationId: cancelCitecheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/lenz-io/agentic-access/lenz-io-agentic-access.yml
summary_line: 24 operations · 13 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Fact Checking
- Enterprise
- Audit
---
