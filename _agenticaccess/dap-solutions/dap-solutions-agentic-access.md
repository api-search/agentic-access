---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 17
api_specs:
- filename: dap-solutions-change-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Change API
  slug: dap-solutions-change-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-change-api-openapi.yml
- filename: dap-solutions-compute-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Compute API
  slug: dap-solutions-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-compute-api-openapi.yml
- filename: dap-solutions-compute-day-count-to-settlement-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Compute Day Count To Settlement API
  slug: dap-solutions-compute-day-count-to-settlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-compute-day-count-to-settlement-api-openapi.yml
- filename: dap-solutions-convert-unix-timestamp-to-date-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Convert Unix Timestamp To Date API
  slug: dap-solutions-convert-unix-timestamp-to-date-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-convert-unix-timestamp-to-date-api-openapi.yml
- filename: dap-solutions-coverage-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Coverage API
  slug: dap-solutions-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-coverage-api-openapi.yml
- filename: dap-solutions-decode-base64-to-text-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Decode Base64 To Text API
  slug: dap-solutions-decode-base64-to-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-decode-base64-to-text-api-openapi.yml
- filename: dap-solutions-diff-two-line-lists-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Diff Two Line Lists API
  slug: dap-solutions-diff-two-line-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-diff-two-line-lists-api-openapi.yml
- filename: dap-solutions-recent-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Recent API
  slug: dap-solutions-recent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-recent-api-openapi.yml
- filename: dap-solutions-search-api-openapi.yml
  format: yaml
  label: Dartmouth Advisory Partners Search API
  slug: dap-solutions-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dap-solutions/openapi/dap-solutions-search-api-openapi.yml
consequence_counts:
  read: 17
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dap Solutions Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Dartmouth Advisory Partners exposes 22 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dartmouth Advisory Partners
provider_slug: dap-solutions
slug: dap-solutions-agentic-access
source_filename: dap-solutions-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/bellwether-openapi.json, openapi/compute-openapi.json, openapi/foundry-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 17\n    acting: 5\n  by_consequence:\n    read: 17\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/search\n  method: get\n  operationId: searchRegulatoryChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recent\n  method: get\n  operationId: recentRegulatoryChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/change\n  method: get\n  operationId: getRegulatoryChange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/coverage\n  method: get\n  operationId: listCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/contracts\n  method: get\n  operationId: searchComputeContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/events\n  method: get\n  operationId: computeMarketEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/prices\n  method: get\n  operationId: computeListPrices\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/record\n  method: get\n  operationId: getComputeRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/query\n  method: get\n  operationId: computeQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/gpu-price\n  method: get\n  operationId: getGpuPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/cheapest-gpu-hour\n  method: get\n  operationId: findCheapestGpuHour\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/price-changes\n  method: get\n  operationId: listPriceChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/contract\n  method: get\n  operationId: getComputeContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/api/regulator-actions\n  method: get\n  operationId: listRegulatorActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/holdings/\n  method: get\n  operationId: consoleHoldings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/query/\n  method: get\n\
  \  operationId: consoleQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compute/query/\n  method: post\n  operationId: consoleQueryAgentShape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compute/api/coverage\n  method: get\n  operationId: listComputeCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/compute-day-count-to-settlement\n  method: post\n  operationId: compute-day-count-to-settlement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/convert-unix-timestamp-to-date\n  method: post\n  operationId: convert-unix-timestamp-to-date\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decode-base64-to-text\n  method: post\n  operationId: decode-base64-to-text\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/diff-two-line-lists\n  method: post\n  operationId: diff-two-line-lists\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/dap-solutions/agentic-access/dap-solutions-agentic-access.yml
summary_line: 22 operations · 5 acting
tags:
- Governance
- Artificial Intelligence
- Toronto
- Institutional
- Technology
- Company
---
