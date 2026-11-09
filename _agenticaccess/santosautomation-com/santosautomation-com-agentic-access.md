---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: santosautomation-com-agent-readiness-api-openapi.yml
  format: yaml
  label: santosautomation-com Agent Readiness API
  slug: santosautomation-com-agent-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-agent-readiness-api-openapi.yml
- filename: santosautomation-com-content-extraction-api-openapi.yml
  format: yaml
  label: santosautomation-com Content Extraction API
  slug: santosautomation-com-content-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-content-extraction-api-openapi.yml
- filename: santosautomation-com-deep-page-audit-api-openapi.yml
  format: yaml
  label: santosautomation-com Deep Page Audit API
  slug: santosautomation-com-deep-page-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-deep-page-audit-api-openapi.yml
- filename: santosautomation-com-deep-website-intelligence-api-openapi.yml
  format: yaml
  label: santosautomation-com Deep Website Intelligence API
  slug: santosautomation-com-deep-website-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-deep-website-intelligence-api-openapi.yml
- filename: santosautomation-com-feed-parser-api-openapi.yml
  format: yaml
  label: santosautomation-com Feed Parser API
  slug: santosautomation-com-feed-parser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-feed-parser-api-openapi.yml
- filename: santosautomation-com-free-tools-api-openapi.yml
  format: yaml
  label: santosautomation-com Free Tools API
  slug: santosautomation-com-free-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-free-tools-api-openapi.yml
- filename: santosautomation-com-link-map-api-openapi.yml
  format: yaml
  label: santosautomation-com Link Map API
  slug: santosautomation-com-link-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-link-map-api-openapi.yml
- filename: santosautomation-com-quick-intelligence-api-openapi.yml
  format: yaml
  label: santosautomation-com Quick Intelligence API
  slug: santosautomation-com-quick-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-quick-intelligence-api-openapi.yml
- filename: santosautomation-com-safe-fetch-api-openapi.yml
  format: yaml
  label: santosautomation-com Safe Fetch API
  slug: santosautomation-com-safe-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-safe-fetch-api-openapi.yml
- filename: santosautomation-com-screenshot-pdf-render-api-openapi.yml
  format: yaml
  label: santosautomation-com Screenshot & PDF Render API
  slug: santosautomation-com-screenshot-pdf-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-screenshot-pdf-render-api-openapi.yml
- filename: santosautomation-com-structured-extraction-api-openapi.yml
  format: yaml
  label: santosautomation-com Structured Extraction API
  slug: santosautomation-com-structured-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-structured-extraction-api-openapi.yml
- filename: santosautomation-com-summarizer-api-openapi.yml
  format: yaml
  label: santosautomation-com Summarizer API
  slug: santosautomation-com-summarizer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/santosautomation-com/openapi/santosautomation-com-summarizer-api-openapi.yml
consequence_counts:
  read: 9
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Santosautomation Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'santosautomation-com exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: santosautomation-com
provider_slug: santosautomation-com
slug: santosautomation-com-agentic-access
source_filename: santosautomation-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/santosautomation-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 9\n    acting: 8\n  by_consequence:\n    read: 9\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/agent-readiness\n  method: get\n  operationId: auditAgentReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/audit\n  method: get\n  operationId: auditWebsite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/audit/batch\n\
  \  method: post\n  operationId: auditWebsiteBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/audit/remediate\n  method: post\n  operationId: remediateAiReadiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fetch\n  method: get\n  operationId: safeFetchUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/extract\n  method: post\n  operationId: extractPageMarkdown\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extract/structured\n  method: post\n  operationId: extractStructuredData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feed\n  method: get\n  operationId: parseFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/links\n  method: get\n  operationId: mapPageLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/summarize\n  method: post\n  operationId: summarizePage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screenshot\n  method: get\n  operationId: renderScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/badge\n  method: get\n  operationId: getAgentReadyBadge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify\n  method: post\n  operationId: verifyReportSignature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audits\n  method: post\n  operationId: createDeepAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audits/{job_id}\n  method: get\n  operationId: getDeepAuditStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audits/{job_id}/report\n  method: get\n  operationId: getDeepAuditReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audits/{job_id}/cancel\n  method: post\n\
  \  operationId: cancelDeepAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/santosautomation-com/agentic-access/santosautomation-com-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Artificial Intelligence
- Automation
- Website Intelligence
- Agent Readiness
- OpenAPI
- Security
---
