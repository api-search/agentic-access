---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 17
api_specs:
- filename: scrunch-ai-data-api-openapi.yml
  format: yaml
  label: Scrunch Data API
  slug: scrunch-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-data-api-openapi.yml
consequence_counts:
  physical: 1
  read: 17
  safety-critical: 1
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Scrunch Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /{brand_id}/ai-referrals/connections/{connection_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orchestration/optimize-and-deploy/{brand_id}
operation_count: 33
overview: 'Scrunch AI exposes 33 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 14 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scrunch AI
provider_slug: scrunch-ai
slug: scrunch-ai-agentic-access
source_filename: scrunch-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/scrunch-ai-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 17\n    acting: 16\n  by_consequence:\n    read: 17\n    safety-critical: 1\n    write: 14\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /{brand_id}/sites/{site_id}/agent-traffic\n  method: get\n  operationId: getAgentTraffic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/ai-referrals/connections/{connection_id}\n  method: delete\n  operationId: disableAiReferralsConnection\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{brand_id}/ai-referrals/connections\n  method: get\n  operationId: listAiReferralsConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/ai-referrals/connections\n  method: post\n  operationId: registerAiReferralsConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /{brand_id}/ai-referrals/connections/{connection_id}/events\n  method: post\n  operationId: pushAiReferralsEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/{brand_id}/competitors/{competitor_id}\n  method: delete\n  operationId: archiveCompetitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/{brand_id}/competitors/{competitor_id}\n  method: get\n  operationId: getCompetitor\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/{brand_id}/competitors/{competitor_id}\n  method: put\n  operationId: updateCompetitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/{brand_id}/personas/{persona_id}\n  method: delete\n  operationId: archivePersona\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/{brand_id}/personas/{persona_id}\n  method: get\n\
  \  operationId: getPersona\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/{brand_id}/personas/{persona_id}\n  method: put\n  operationId: updatePersona\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{brand_id}/prompts/{prompt_id}\n  method: delete\n  operationId: archivePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /orchestration/render-bulk/{brand_id}/sites/{site_id}\n  method: post\n  operationId: bulkRenderOptimizedPages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands\n  method: post\n  operationId: createBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - create-brand\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands\n  method: get\n  operationId: listBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /brands/{brand_id}/competitors\n  method: post\n  operationId: createCompetitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/{brand_id}/competitors\n  method: get\n  operationId: listCompetitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/page-audits\n  method: post\n  operationId: createPageAudits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{brand_id}/page-audits\n  method: get\n  operationId: listPageAudits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/{brand_id}/personas\n  method: post\n  operationId: createPersona\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/{brand_id}/personas\n  method: get\n  operationId: listPersonas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/prompts\n  method: post\n  operationId:\
  \ createPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{brand_id}/prompts\n  method: get\n  operationId: listPrompts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/page-audits/{page_audit_id}\n  method: get\n  operationId: getPageAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/responses\n  method: get\n  operationId: listResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /orchestration/optimize-and-deploy/{brand_id}\n  method: post\n  operationId: createOptimizeAndDeployPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orchestration/optimize-and-deploy/{brand_id}/{token}\n  method: get\n  operationId: getOptimizeAndDeployStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/query\n  method: get\n  operationId: query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /{brand_id}/sitemap/export\n  method: get\n  operationId: exportSitemapPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/sitemap/pages/{page_id}/metrics\n  method: get\n  operationId: getSitemapPageMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/sitemap/pages/{page_id}\n  method: get\n  operationId: getSitemapPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{brand_id}/sitemap/pages\n  method: get\n  operationId: listSitemapPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - query\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/{brand_id}\n  method: patch\n  operationId: patchBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - configure\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/agentic-access/scrunch-ai-agentic-access.yml
summary_line: 33 operations · 16 acting · 1 human-in-the-loop
tags:
- Company
- AI
- AI Search
- Answer Engine Optimization
- Generative Engine Optimization
- Brand Visibility
- Analytics
- SEO
- Agent Experience
- MCP
---
