---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 13
api_specs:
- filename: caper-network-agent-api-openapi.yml
  format: yaml
  label: Caper Agent API
  slug: caper-network-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-agent-api-openapi.yml
- filename: caper-network-blog-api-openapi.yml
  format: yaml
  label: Caper Blog API
  slug: caper-network-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-blog-api-openapi.yml
- filename: caper-network-blog-xml-api-openapi.yml
  format: yaml
  label: Caper Blog.xml API
  slug: caper-network-blog-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-blog-xml-api-openapi.yml
- filename: caper-network-capers-api-openapi.yml
  format: yaml
  label: Caper Capers API
  slug: caper-network-capers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-capers-api-openapi.yml
- filename: caper-network-llms-txt-api-openapi.yml
  format: yaml
  label: Caper Llms.txt API
  slug: caper-network-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-llms-txt-api-openapi.yml
- filename: caper-network-mcp-api-openapi.yml
  format: yaml
  label: Caper MCP API
  slug: caper-network-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-mcp-api-openapi.yml
- filename: caper-network-sitemap-xml-api-openapi.yml
  format: yaml
  label: Caper Sitemap.xml API
  slug: caper-network-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-sitemap-xml-api-openapi.yml
- filename: caper-network-well-known-api-openapi.yml
  format: yaml
  label: Caper .well Known API
  slug: caper-network-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-well-known-api-openapi.yml
- filename: caper-network-wiki-api-openapi.yml
  format: yaml
  label: Caper Wiki API
  slug: caper-network-wiki-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/caper-network/openapi/caper-network-wiki-api-openapi.yml
consequence_counts:
  read: 13
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Caper Network Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Caper exposes 20 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Caper
provider_slug: caper-network
slug: caper-network-agentic-access
source_filename: caper-network-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/caper-network-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 13\n    acting: 7\n  by_consequence:\n    read: 13\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /llms.txt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wiki/{path}.md\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blog/{slug}.md\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wiki\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wiki/{path}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capers/{cashtag}/llms.txt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capers/{cashtag}/dao.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blog.xml\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /sitemap.xml\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capers/{cashtag}/mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/challenge\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/login\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/manifests\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/submit\n  method: post\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/wiki\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/wiki/delete\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/about\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/caper-network/agentic-access/caper-network-agentic-access.yml
summary_line: 20 operations · 7 acting
tags:
- DAO
- Blockchain
- Fundraising
- Radix
- Decentralized
---
