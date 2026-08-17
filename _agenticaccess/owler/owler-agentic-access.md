---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: owler-enterprise-api-openapi.yml
  format: yaml
  label: Owler Enterprise API
  slug: owler-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/owler/refs/heads/main/openapi/owler-enterprise-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Owler Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Owler exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Owler
provider_slug: owler
slug: owler-agentic-access
source_filename: owler-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/owler-enterprise-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/companypremium/url/{website}\n  method: get\n  operationId: getCompanyByWebsite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companypremium/id/{companyId}\n  method: get\n  operationId: getCompanyById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/competitorpremium/url/{website}\n\
  \  method: get\n  operationId: getCompetitorsForWebsite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/competitorpremium/id/{companyId}\n  method: get\n  operationId: getCompetitorsForId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feed/url\n  method: get\n  operationId: getFeedsByWebsite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feed\n  method: get\n  operationId: getFeeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owler/refs/heads/main/agentic-access/owler-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Company Intelligence
- Sales Intelligence
- Competitive Intelligence
- Business Data
- Data Licensing
- News Monitoring
- Market Research
- Firmographics
- Company Search
- Funding Data
---
