---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 7
api_specs:
- filename: majr-app-audit-api-openapi.yml
  format: yaml
  label: majr-app Audit API
  slug: majr-app-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-audit-api-openapi.yml
- filename: majr-app-discovery-api-openapi.yml
  format: yaml
  label: majr-app Discovery API
  slug: majr-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-discovery-api-openapi.yml
- filename: majr-app-drafting-api-openapi.yml
  format: yaml
  label: majr-app Drafting API
  slug: majr-app-drafting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-drafting-api-openapi.yml
- filename: majr-app-encode-api-openapi.yml
  format: yaml
  label: majr-app Encode API
  slug: majr-app-encode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-encode-api-openapi.yml
- filename: majr-app-generation-api-openapi.yml
  format: yaml
  label: majr-app Generation API
  slug: majr-app-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-generation-api-openapi.yml
- filename: majr-app-healthz-api-openapi.yml
  format: yaml
  label: majr-app Healthz API
  slug: majr-app-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-healthz-api-openapi.yml
- filename: majr-app-jobs-api-openapi.yml
  format: yaml
  label: majr-app Jobs API
  slug: majr-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-jobs-api-openapi.yml
- filename: majr-app-uploads-api-openapi.yml
  format: yaml
  label: majr-app Uploads API
  slug: majr-app-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-uploads-api-openapi.yml
- filename: majr-app-usage-api-openapi.yml
  format: yaml
  label: majr-app Usage API
  slug: majr-app-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-usage-api-openapi.yml
- filename: majr-app-voice-api-openapi.yml
  format: yaml
  label: majr-app Voice API
  slug: majr-app-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/majr-app/openapi/majr-app-voice-api-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Majr App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/draft-dispatch
operation_count: 15
overview: 'majr-app exposes 15 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 7 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: majr-app
provider_slug: majr-app
slug: majr-app-agentic-access
source_filename: majr-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/dispatch-openapi.json, openapi/encoding-openapi.json, openapi/seo-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 7\n    acting: 8\n  by_consequence:\n    read: 7\n    safety-critical: 1\n    write: 7\n  human_in_the_loop_required: 1\noperations:\n- path: /\n  method: get\n  operationId: getServiceCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog.json\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/draft-dispatch\n  method: post\n  operationId: draftDispatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/voice\n  method: get\n  operationId: getVoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: healthz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/uploads\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/encode\n  method: post\n  operationId: enqueueEncode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobId}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getServiceCard\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/head\n  method: post\n  operationId: generateHead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/robots\n  method: post\n  operationId: generateRobots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sitemap\n  method: post\n  operationId: generateSitemap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/llms-txt\n  method: post\n  operationId: generateLlmsTxt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audit\n  method: post\n  operationId: auditPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/majr-app/agentic-access/majr-app-agentic-access.yml
summary_line: 15 operations · 8 acting · 1 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Media
- SEO
- Encoding
- Agent Services
---
