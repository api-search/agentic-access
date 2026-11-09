---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: certdesk-dev-certificate-api-openapi.yml
  format: yaml
  label: certdesk-dev Certificate API
  slug: certdesk-dev-certificate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-certificate-api-openapi.yml
- filename: certdesk-dev-dns-api-openapi.yml
  format: yaml
  label: certdesk-dev Dns API
  slug: certdesk-dev-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-dns-api-openapi.yml
- filename: certdesk-dev-dns-info-api-openapi.yml
  format: yaml
  label: certdesk-dev Dns Info API
  slug: certdesk-dev-dns-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-dns-info-api-openapi.yml
- filename: certdesk-dev-expiry-api-openapi.yml
  format: yaml
  label: certdesk-dev Expiry API
  slug: certdesk-dev-expiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-expiry-api-openapi.yml
- filename: certdesk-dev-explain-api-openapi.yml
  format: yaml
  label: certdesk-dev Explain API
  slug: certdesk-dev-explain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-explain-api-openapi.yml
- filename: certdesk-dev-security-api-openapi.yml
  format: yaml
  label: certdesk-dev Security API
  slug: certdesk-dev-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-security-api-openapi.yml
- filename: certdesk-dev-watch-api-openapi.yml
  format: yaml
  label: certdesk-dev Watch API
  slug: certdesk-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-watch-api-openapi.yml
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Certdesk Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'certdesk-dev exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: certdesk-dev
provider_slug: certdesk-dev
slug: certdesk-dev-agentic-access
source_filename: certdesk-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /certificate\n  method: get\n  operationId: checkCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expiry\n  method: get\n  operationId: checkExpiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security\n  method: get\n  operationId: checkSecurity\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /explain\n  method: get\n  operationId: explainTlsError\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /watch\n  method: post\n  operationId: watchExpiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns-info\n  method: get\n  operationId: dnsInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns\n  method: get\n  operationId: dnsPropagation\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/certdesk-dev/agentic-access/certdesk-dev-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Company
---
