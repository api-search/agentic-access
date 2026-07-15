---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: openapi.json
  format: json
  label: Coalition Exploit Scoring System (ESS) API
  slug: exploit-scoring-system
  spec_type: OpenAPI
  url: https://ess-api.coalitioninc.com/openapi.json
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coalition Inc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Coalition exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Coalition
provider_slug: coalition-inc
slug: coalition-inc-agentic-access
source_filename: coalition-inc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/coalition-ess-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /cve\n  method: get\n  operationId: cve_cve_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve/{cve_id}\n  method: get\n  operationId: cve_by_id_cve__cve_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve/{cve_id}/history\n  method: get\n  operationId: cve_history_by_id_cve__cve_id__history_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve/{cve_id}/exploits/exploitdb\n  method: get\n  operationId: exploits_exploitdb_by_cve_cve__cve_id__exploits_exploitdb_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve/{cve_id}/exploits/metasploit\n  method: get\n  operationId: exploits_metasploit_by_cve_cve__cve_id__exploits_metasploit_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve/{cve_id}/mentions/twitter\n  method: get\n  operationId: mentions_twitter_by_cve_cve__cve_id__mentions_twitter_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve/{cve_id}/repositories/github\n\
  \  method: get\n  operationId: repositories_github_by_cve_cve__cve_id__repositories_github_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coalition-inc/refs/heads/main/agentic-access/coalition-inc-agentic-access.yml
summary_line: 7 operations
tags:
- Cyber Insurance
- Insurance
- Insurtech
- Risk Management
- Cybersecurity
- Vulnerability Management
- CVE
- Exploit Scoring
- Threat Intelligence
- Incident Response
- Attack Surface Management
- Brokers
- MGA
- Executive Risks
- Technology E&O
- Active Insurance
---
