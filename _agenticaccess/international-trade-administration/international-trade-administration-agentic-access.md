---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: international-trade-administration-consolidated-screening-list-api-openapi.yml
  format: yaml
  label: International Trade Administration Consolidated Screening List API
  slug: international-trade-administration-consolidated-screening-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-consolidated-screening-list-api-openapi.yml
- filename: international-trade-administration-country-commercial-guides-api-openapi.yml
  format: yaml
  label: International Trade Administration Country Commercial Guides API
  slug: international-trade-administration-country-commercial-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-country-commercial-guides-api-openapi.yml
- filename: international-trade-administration-customs-tariff-api-openapi.yml
  format: yaml
  label: International Trade Administration Customs Tariff API
  slug: international-trade-administration-customs-tariff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-customs-tariff-api-openapi.yml
- filename: international-trade-administration-de-minimis-api-openapi.yml
  format: yaml
  label: International Trade Administration De Minimis API
  slug: international-trade-administration-de-minimis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-de-minimis-api-openapi.yml
- filename: international-trade-administration-market-intelligence-api-openapi.yml
  format: yaml
  label: International Trade Administration Market Intelligence API
  slug: international-trade-administration-market-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-market-intelligence-api-openapi.yml
- filename: international-trade-administration-trade-events-api-openapi.yml
  format: yaml
  label: International Trade Administration Trade Events API
  slug: international-trade-administration-trade-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/openapi/international-trade-administration-trade-events-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: International Trade Administration Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'International Trade Administration exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: International Trade Administration
provider_slug: international-trade-administration
slug: international-trade-administration-agentic-access
source_filename: international-trade-administration-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/international-trade-administration-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /consolidated_screening_list/v1/search\n  method: get\n  operationId: searchConsolidatedScreeningList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consolidated_screening_list/v1/sources\n  method: get\n  operationId: listScreeningSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /CCG/v2/search\n  method: get\n  operationId: searchCountryCommercialGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market_intelligence/v1/search\n  method: get\n  operationId: searchMarketIntelligence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/v1/search\n  method: get\n  operationId: searchTradeEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customs_tariff/v1/search\n  method: get\n  operationId: searchCustomsTariff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /de_minimis/v1/search\n  method: get\n \
  \ operationId: searchDeMinimis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/international-trade-administration/refs/heads/main/agentic-access/international-trade-administration-agentic-access.yml
summary_line: 7 operations
tags:
- Compliance
- Customs
- Export
- Federal-Government
- International Business
- Screening List
- Tariffs
- Trade
- Trade Data
- Trade Events
---
