---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: bustup-monitor-com-agent-docs-md-api-openapi.yml
  format: yaml
  label: bustup-monitor-com Agent Docs.md API
  slug: bustup-monitor-com-agent-docs-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bustup-monitor-com/openapi/bustup-monitor-com-agent-docs-md-api-openapi.yml
- filename: bustup-monitor-com-breast-augmentation-api-openapi.yml
  format: yaml
  label: bustup-monitor-com Breast Augmentation API
  slug: bustup-monitor-com-breast-augmentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bustup-monitor-com/openapi/bustup-monitor-com-breast-augmentation-api-openapi.yml
- filename: bustup-monitor-com-clinic-api-openapi.yml
  format: yaml
  label: bustup-monitor-com Clinic API
  slug: bustup-monitor-com-clinic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bustup-monitor-com/openapi/bustup-monitor-com-clinic-api-openapi.yml
- filename: bustup-monitor-com-concerns-api-openapi.yml
  format: yaml
  label: bustup-monitor-com Concerns API
  slug: bustup-monitor-com-concerns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bustup-monitor-com/openapi/bustup-monitor-com-concerns-api-openapi.yml
- filename: bustup-monitor-com-default-api-openapi.yml
  format: yaml
  label: bustup-monitor-com 豊胸モニターナビ API
  slug: bustup-monitor-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bustup-monitor-com/openapi/bustup-monitor-com-default-api-openapi.yml
- filename: bustup-monitor-com-faq-api-openapi.yml
  format: yaml
  label: bustup-monitor-com Faq API
  slug: bustup-monitor-com-faq-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bustup-monitor-com/openapi/bustup-monitor-com-faq-api-openapi.yml
- filename: bustup-monitor-com-generation-api-openapi.yml
  format: yaml
  label: bustup-monitor-com Generation API
  slug: bustup-monitor-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bustup-monitor-com/openapi/bustup-monitor-com-generation-api-openapi.yml
- filename: bustup-monitor-com-monitor-api-openapi.yml
  format: yaml
  label: bustup-monitor-com Monitor API
  slug: bustup-monitor-com-monitor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bustup-monitor-com/openapi/bustup-monitor-com-monitor-api-openapi.yml
- filename: bustup-monitor-com-sitemap-xml-api-openapi.yml
  format: yaml
  label: bustup-monitor-com Sitemap.xml API
  slug: bustup-monitor-com-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bustup-monitor-com/openapi/bustup-monitor-com-sitemap-xml-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bustup Monitor Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'bustup-monitor-com exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: bustup-monitor-com
provider_slug: bustup-monitor-com
slug: bustup-monitor-com-agentic-access
source_filename: bustup-monitor-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/bustup-monitor-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breast-augmentation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breast-augmentation/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clinic\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clinic/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faq\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concerns\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generation\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-docs.md\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bustup-monitor-com/agentic-access/bustup-monitor-com-agentic-access.yml
summary_line: 11 operations
tags:
- Company
---
