---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 7
api_specs:
- filename: baloise-contracts-api-openapi.yml
  format: yaml
  label: Baloise Contracts API
  slug: baloise-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/openapi/baloise-contracts-api-openapi.yml
- filename: baloise-db-api-openapi.yml
  format: yaml
  label: Baloise DB API
  slug: baloise-db-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/openapi/baloise-db-api-openapi.yml
- filename: baloise-documents-api-openapi.yml
  format: yaml
  label: Baloise Documents API
  slug: baloise-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/openapi/baloise-documents-api-openapi.yml
- filename: baloise-jboss-api-openapi.yml
  format: yaml
  label: Baloise J Boss API
  slug: baloise-jboss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/openapi/baloise-jboss-api-openapi.yml
- filename: baloise-middlewares-api-openapi.yml
  format: yaml
  label: Baloise Middlewares API
  slug: baloise-middlewares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/openapi/baloise-middlewares-api-openapi.yml
- filename: baloise-orders-api-openapi.yml
  format: yaml
  label: Baloise Orders API
  slug: baloise-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/openapi/baloise-orders-api-openapi.yml
- filename: baloise-pgsql-api-openapi.yml
  format: yaml
  label: Baloise Pgsql API
  slug: baloise-pgsql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/openapi/baloise-pgsql-api-openapi.yml
- filename: baloise-version-api-openapi.yml
  format: yaml
  label: Baloise Version API
  slug: baloise-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/openapi/baloise-version-api-openapi.yml
- filename: baloise-vms-api-openapi.yml
  format: yaml
  label: Baloise VMs API
  slug: baloise-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/openapi/baloise-vms-api-openapi.yml
consequence_counts:
  read: 7
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Baloise Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Baloise exposes 17 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Baloise
provider_slug: baloise
slug: baloise-agentic-access
source_filename: baloise-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/baloise-corellia-contracts-openapi.yml, openapi/baloise-oim-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 7\n    acting: 10\n  by_consequence:\n    read: 7\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /contracts/v2/version\n  method: get\n  operationId: version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/v2/documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/v2/cancellations\n  method: post\n  operationId: cancelContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/v2\n  method: post\n  operationId: uploadContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/{id}\n  method: get\n  operationId: api.calls_phs.order_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/{id}/details\n  method: get\n  operationId: api.calls_phs.order_get_detail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vm\n  method: get\n  operationId: api.calls_phs.vm_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vm\n  method: post\n  operationId: api.calls_phs.vm_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vm/{name}\n  method: get\n  operationId: api.calls_phs.vm_get\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vm/{name}\n  method: delete\n  operationId: api.calls_phs.vm_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vm/{name}\n  method: patch\n  operationId: api.calls_phs.vm_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbpg\n  method: get\n  operationId: api.calls_phs.pgsql_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /dbpg\n  method: post\n  operationId: api.calls_phs.pgsql_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbpg/{dbid}\n  method: get\n  operationId: api.calls_phs.pgsql_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dbpg/{dbid}\n  method: patch\n  operationId: api.calls_phs.pgsql_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dbpg/{dbid}\n  method: delete\n  operationId:\
  \ api.calls_phs.pgsql_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jb\n  method: post\n  operationId: api.calls_phs.jb_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baloise/refs/heads/main/agentic-access/baloise-agentic-access.yml
summary_line: 17 operations · 10 acting
tags:
- Company
- Insurance
- Financial Services
- Switzerland
- Open Source
- API Governance
- Spectral
- Linting
---
