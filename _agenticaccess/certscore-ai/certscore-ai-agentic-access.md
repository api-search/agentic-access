---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 13
api_specs:
- filename: certscore-ai-auth-api-openapi.yml
  format: yaml
  label: certscore-ai Auth API
  slug: certscore-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-auth-api-openapi.yml
- filename: certscore-ai-diagnostics-api-openapi.yml
  format: yaml
  label: certscore-ai Diagnostics API
  slug: certscore-ai-diagnostics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-diagnostics-api-openapi.yml
- filename: certscore-ai-domains-api-openapi.yml
  format: yaml
  label: certscore-ai Domains API
  slug: certscore-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-domains-api-openapi.yml
- filename: certscore-ai-findings-api-openapi.yml
  format: yaml
  label: certscore-ai Findings API
  slug: certscore-ai-findings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-findings-api-openapi.yml
- filename: certscore-ai-pulse-api-openapi.yml
  format: yaml
  label: certscore-ai Pulse API
  slug: certscore-ai-pulse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-pulse-api-openapi.yml
- filename: certscore-ai-runtime-inventory-api-openapi.yml
  format: yaml
  label: certscore-ai Runtime Inventory API
  slug: certscore-ai-runtime-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-runtime-inventory-api-openapi.yml
- filename: certscore-ai-scans-api-openapi.yml
  format: yaml
  label: certscore-ai Scans API
  slug: certscore-ai-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-scans-api-openapi.yml
consequence_counts:
  read: 13
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Certscore Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'certscore-ai exposes 15 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: certscore-ai
provider_slug: certscore-ai
slug: certscore-ai-agentic-access
source_filename: certscore-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/certscore-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 2\n    connected: 13\n  by_consequence:\n    write: 2\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/keys/request\n  method: post\n  operationId: requestReadOnlyApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/auth/check\n  method: get\n  operationId: checkIntegrationCredential\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/scans\n  method: post\n  operationId: createScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/scans/{scanId}\n  method: get\n  operationId: getScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/scans/{scanId}/status\n  method: get\n  operationId: getScanStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/scans/{scanId}/diagnostics\n  method: get\n  operationId: getScanDiagnostics\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/scans/{scanId}/findings\n  method: get\n  operationId: listScanFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/scans/{scanId}/findings/{findingId}\n  method: get\n  operationId: getScanFinding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/domains/{domain}/latest\n  method: get\n  operationId: getLatestDomainScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/scans/{scanId}/pulse\n  method: get\n  operationId: getScanPulse\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/scans/{scanId}/report-evidence\n  method: get\n  operationId: getReportEvidencePage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/scans/{scanId}/report-evidence/form-snapshot\n  method: get\n  operationId: getRetainedFormSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/scans/{scanId}/pre-consent-cookies-trackers\n  method: get\n  operationId: getScanPreConsentCookiesTrackers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/domains/{domain}/latest/pre-consent-cookies-trackers\n  method: get\n  operationId: getLatestDomainPreConsentCookiesTrackers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/health\n  method: get\n  operationId: getApiV2Health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/certscore-ai/agentic-access/certscore-ai-agentic-access.yml
summary_line: 15 operations · 2 acting
tags:
- Company
- Privacy
- Security
- Scanning
- Compliance
---
