---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: agent402-dev-openapi.yml
  format: yaml
  label: Agent402 Direct x402 HTTP Resources
  slug: agent402-direct-x402-http-resources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agent402-dev/refs/heads/main/openapi/agent402-dev-openapi.yml
consequence_counts:
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agent402 Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'agent402.dev exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: agent402.dev
provider_slug: agent402-dev
slug: agent402-dev-agentic-access
source_filename: agent402-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/agent402-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 6\n    connected: 6\n  by_consequence:\n    write: 6\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /task-day-plan\n  method: post\n  operationId: taskDayPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /website-preflight\n  method: post\n  operationId: websitePreflight\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /url-evidence\n  method: get\n  operationId: verifiedUrlEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site-release-audit\n  method: post\n  operationId: siteReleaseAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /site-release-audit/eligibility\n  method: post\n  operationId: siteReleaseAuditEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /site-release-audit/sample.json\n  method: get\n  operationId: siteReleaseAuditSample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site-release-audit/methodology.json\n  method: get\n  operationId: siteReleaseAuditMethodology\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site-release-audit/proof/v1/case-study.json\n  method: get\n  operationId: siteReleaseAuditCaseStudy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit-x402\n  method: post\n  operationId: auditX402\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402-health\n  method: post\n  operationId: x402Health\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /download\n  method: get\n  operationId: downloadWayfarersDeck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qr-campaign-pack\n  method: get\n  operationId: downloadQrCampaignPack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agent402-dev/refs/heads/main/agentic-access/agent402-dev-agentic-access.yml
summary_line: 12 operations · 6 acting
tags:
- Company
- x402
- Agentic Payments
- Agentic Commerce
- AI Agents
- A2A
- Technical SEO
- Website Audits
- URL Evidence
- Developer Tools
- Base
---
