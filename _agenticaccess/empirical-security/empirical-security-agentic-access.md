---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: empirical-security-openapi.yml
  format: yaml
  label: Empirical Security API
  slug: empirical-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/empirical-security/refs/heads/main/openapi/empirical-security-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Empirical Security Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Empirical Security exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Empirical Security
provider_slug: empirical-security
slug: empirical-security-agentic-access
source_filename: empirical-security-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/empirical-security-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /cves/{cve_id}\n  method: get\n  operationId: getCve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cves/{cve_id}/malware\n  method: get\n  operationId: getCveMalware\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cves/{cve_id}/critical_indicators\n  method: get\n  operationId:\
  \ getCveCriticalIndicators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cves/{cve_id}/score_history\n  method: get\n  operationId: getCveScoreHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cves/{cve_id}/history\n  method: get\n  operationId: getCveHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cves/all\n  method: get\n  operationId: getAllCves\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchCves\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /cve_groups\n  method: get\n  operationId: listCveGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve_groups/{id}\n  method: get\n  operationId: getCveGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empirical-security/refs/heads/main/agentic-access/empirical-security-agentic-access.yml
summary_line: 9 operations
tags:
- Company
- Security
- Cybersecurity
- Vulnerability Management
- Vulnerability Prioritization
- CVE
- EPSS
- Exploit Prediction
- Threat Intelligence
---
