---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 9
api_specs:
- filename: domaindrift-io-alerts-api-openapi.yml
  format: yaml
  label: DomainDrift Alerts API
  slug: domaindrift-io-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-alerts-api-openapi.yml
- filename: domaindrift-io-changes-api-openapi.yml
  format: yaml
  label: DomainDrift Changes API
  slug: domaindrift-io-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-changes-api-openapi.yml
- filename: domaindrift-io-domains-api-openapi.yml
  format: yaml
  label: DomainDrift Domains API
  slug: domaindrift-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-domains-api-openapi.yml
- filename: domaindrift-io-health-api-openapi.yml
  format: yaml
  label: DomainDrift Health API
  slug: domaindrift-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-health-api-openapi.yml
- filename: domaindrift-io-scan-api-openapi.yml
  format: yaml
  label: DomainDrift Scan API
  slug: domaindrift-io-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-scan-api-openapi.yml
- filename: domaindrift-io-stream-api-openapi.yml
  format: yaml
  label: DomainDrift Stream API
  slug: domaindrift-io-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-stream-api-openapi.yml
consequence_counts:
  read: 9
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Domaindrift Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'DomainDrift exposes 13 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DomainDrift
provider_slug: domaindrift-io
slug: domaindrift-io-agentic-access
source_filename: domaindrift-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/domaindrift-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 9\n    acting: 4\n  by_consequence:\n    read: 9\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/domains/{domain}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}/history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}/provenance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domain}/bundle\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/changes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alerts/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/stream\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scan/{domain}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/domaindrift-io/agentic-access/domaindrift-io-agentic-access.yml
summary_line: 13 operations · 4 acting
tags:
- Security
- Monitoring
- Domain
- Telemetry
---
