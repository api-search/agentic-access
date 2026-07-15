---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 19
api_specs:
- filename: builtwith-domain-openapi.yml
  format: yaml
  label: BuiltWith Domain API
  slug: builtwith-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-domain-openapi.yml
- filename: builtwith-lists-openapi.yml
  format: yaml
  label: BuiltWith Lists API
  slug: builtwith-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-lists-openapi.yml
- filename: builtwith-trends-openapi.yml
  format: yaml
  label: BuiltWith Trends API
  slug: builtwith-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-trends-openapi.yml
- filename: builtwith-change-openapi.yml
  format: yaml
  label: BuiltWith Change API
  slug: builtwith-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-change-openapi.yml
- filename: builtwith-relationships-openapi.yml
  format: yaml
  label: BuiltWith Relationships API
  slug: builtwith-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-relationships-openapi.yml
- filename: builtwith-free-openapi.yml
  format: yaml
  label: BuiltWith Free API
  slug: builtwith-free-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-free-openapi.yml
- filename: builtwith-tags-openapi.yml
  format: yaml
  label: BuiltWith Tags API
  slug: builtwith-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-tags-openapi.yml
consequence_counts:
  read: 19
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Builtwith Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'BuiltWith exposes 20 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BuiltWith
provider_slug: builtwith
slug: builtwith-agentic-access
source_filename: builtwith-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/builtwith-change-openapi.yml, openapi/builtwith-domain-openapi.yml, openapi/builtwith-free-openapi.yml,\n  openapi/builtwith-lists-openapi.yml, openapi/builtwith-relationships-openapi.yml, openapi/builtwith-tags-openapi.yml,\n  openapi/builtwith-trends-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 19\n    acting: 1\n  by_consequence:\n    read: 19\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api.json\n  method: get\n  operationId: getDomainChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.json\n\
  \  method: get\n  operationId: getDomainTechnologiesJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.xml\n  method: get\n  operationId: getDomainTechnologiesXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.csv\n  method: get\n  operationId: getDomainTechnologiesCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domain/bulk\n  method: post\n  operationId: bulkDomainLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api.json\n  method: get\n  operationId: getFreeDomainJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.xml\n  method: get\n  operationId: getFreeDomainXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.json\n  method: get\n  operationId: getTechListJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.xml\n  method: get\n  operationId: getTechListXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.txt\n  method: get\n  operationId: getTechListTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.csv\n  method: get\n  operationId: getTechListCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.tsv\n  method: get\n  operationId: getTechListTsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.json\n  method: get\n  operationId: getDomainRelationshipsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.xml\n  method: get\n  operationId: getDomainRelationshipsXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.csv\n  method: get\n  operationId: getDomainRelationshipsCsv\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.tsv\n  method: get\n  operationId: getDomainRelationshipsTsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.json\n  method: get\n  operationId: getTagDomainsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.xml\n  method: get\n  operationId: getTagDomainsXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.json\n  method: get\n  operationId: getTechTrendJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.xml\n\
  \  method: get\n  operationId: getTechTrendXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/agentic-access/builtwith-agentic-access.yml
summary_line: 20 operations · 1 acting
tags:
- Technology Profiling
- Lead Generation
- Web Intelligence
- Technology Detection
- Website Analysis
- Market Research
---
