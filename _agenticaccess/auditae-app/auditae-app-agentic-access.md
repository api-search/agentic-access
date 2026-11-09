---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 9
api_specs:
- filename: auditae-app-billing-api-openapi.yml
  format: yaml
  label: AuditAE Billing API
  slug: auditae-app-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auditae-app/openapi/auditae-app-billing-api-openapi.yml
- filename: auditae-app-citations-api-openapi.yml
  format: yaml
  label: AuditAE Citations API
  slug: auditae-app-citations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auditae-app/openapi/auditae-app-citations-api-openapi.yml
- filename: auditae-app-schema-api-openapi.yml
  format: yaml
  label: AuditAE Schema API
  slug: auditae-app-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auditae-app/openapi/auditae-app-schema-api-openapi.yml
- filename: auditae-app-technical-api-openapi.yml
  format: yaml
  label: AuditAE Technical API
  slug: auditae-app-technical-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auditae-app/openapi/auditae-app-technical-api-openapi.yml
consequence_counts:
  read: 9
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Auditae App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/crawl/schedule
operation_count: 21
overview: 'AuditAE exposes 21 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 11 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AuditAE
provider_slug: auditae-app
slug: auditae-app-agentic-access
source_filename: auditae-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/auditae-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 12\n    connected: 9\n  by_consequence:\n    write: 11\n    read: 9\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/check\n  method: post\n  operationId: checkCitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audits\n  method: post\n  operationId: createAudit\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audits/{id}\n  method: get\n  operationId: getAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crawl/{id}\n  method: get\n  operationId: getCrawl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crawl/{id}/checks\n  method: get\n  operationId: listCrawlChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crawl/{id}/checks/{check}\n  method: get\n  operationId: getCrawlCheck\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crawl/{id}/compare\n  method: get\n  operationId: compareCrawls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crawl/history\n  method: get\n  operationId: listCrawlHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crawl/schedule\n  method: get\n  operationId: getCrawlSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crawl/schedule\n  method: put\n  operationId: putCrawlSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crawl/schedule\n  method: delete\n  operationId: deleteCrawlSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/billing\n  method: get\n  operationId: getBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/top-up\n  method: post\n  operationId: topUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crawl\n  method: post\n  operationId: crawlSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/crawl/settings\n  method: get\n  operationId: getCrawlSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crawl/settings\n  method: put\n  operationId: putCrawlSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/technical\n  method: post\n  operationId: technicalAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/images/optimize\n  method: post\n  operationId: optimizeImages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/schema/validate\n  method: post\n  operationId: validateSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/schema/generate\n  method: post\n  operationId: generateSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/entities/discover\n  method: post\n  operationId: discoverEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/auditae-app/agentic-access/auditae-app-agentic-access.yml
summary_line: 21 operations · 12 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- SEO
- Marketing
- Software-as-a-Service
- Visibility
---
