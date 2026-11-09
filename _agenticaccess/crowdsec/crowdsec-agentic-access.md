---
acting_count: 1
action_class_counts:
  acting: 1
api_specs:
- filename: crowdsec-allow-lists-api-openapi.yml
  format: yaml
  label: Crowdsec Allow Lists API
  slug: crowdsec-allow-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-allow-lists-api-openapi.yml
- filename: crowdsec-blocklists-api-openapi.yml
  format: yaml
  label: Crowdsec Blocklists API
  slug: crowdsec-blocklists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-blocklists-api-openapi.yml
- filename: crowdsec-cves-api-openapi.yml
  format: yaml
  label: Crowdsec CVEs API
  slug: crowdsec-cves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-cves-api-openapi.yml
- filename: crowdsec-hub-api-openapi.yml
  format: yaml
  label: Crowdsec Hub API
  slug: crowdsec-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-hub-api-openapi.yml
- filename: crowdsec-info-api-openapi.yml
  format: yaml
  label: Crowdsec Info API
  slug: crowdsec-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-info-api-openapi.yml
- filename: crowdsec-integrations-api-openapi.yml
  format: yaml
  label: Crowdsec Integrations API
  slug: crowdsec-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-integrations-api-openapi.yml
- filename: crowdsec-metrics-api-openapi.yml
  format: yaml
  label: Crowdsec Metrics API
  slug: crowdsec-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-metrics-api-openapi.yml
consequence_counts:
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crowdsec Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'Crowdsec exposes 1 API operation that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crowdsec
provider_slug: crowdsec
slug: crowdsec-agentic-access
source_filename: crowdsec-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: generated\nsource: openapi/crowdsec-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    acting: 1\n  by_consequence:\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /allowlists\n  method: post\n  operationId: createAllowlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/crowdsec/agentic-access/crowdsec-agentic-access.yml
summary_line: 1 operation · 1 acting
tags:
- Security
- Threat Intelligence
- Open Source
- Community
- Automation
- CrowdSec
---
