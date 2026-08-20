---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 16
api_specs:
- filename: bloomberg-aim-broker-strategies-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Broker Strategies API
  slug: bloomberg-aim-broker-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-broker-strategies-api-openapi.yml
- filename: bloomberg-aim-catalogs-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Catalogs API
  slug: bloomberg-aim-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-catalogs-api-openapi.yml
- filename: bloomberg-aim-distributions-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Distributions API
  slug: bloomberg-aim-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-distributions-api-openapi.yml
- filename: bloomberg-aim-field-lists-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Field Lists API
  slug: bloomberg-aim-field-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-field-lists-api-openapi.yml
- filename: bloomberg-aim-field-search-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Field Search API
  slug: bloomberg-aim-field-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-field-search-api-openapi.yml
- filename: bloomberg-aim-fills-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Fills API
  slug: bloomberg-aim-fills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-fills-api-openapi.yml
- filename: bloomberg-aim-historical-data-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Historical Data API
  slug: bloomberg-aim-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-historical-data-api-openapi.yml
- filename: bloomberg-aim-instruments-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Instruments API
  slug: bloomberg-aim-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-instruments-api-openapi.yml
- filename: bloomberg-aim-intraday-data-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Intraday Data API
  slug: bloomberg-aim-intraday-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-intraday-data-api-openapi.yml
- filename: bloomberg-aim-orders-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Orders API
  slug: bloomberg-aim-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-orders-api-openapi.yml
- filename: bloomberg-aim-reference-data-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Reference Data API
  slug: bloomberg-aim-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-reference-data-api-openapi.yml
- filename: bloomberg-aim-replies-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Replies API
  slug: bloomberg-aim-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-replies-api-openapi.yml
- filename: bloomberg-aim-requests-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Requests API
  slug: bloomberg-aim-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-requests-api-openapi.yml
- filename: bloomberg-aim-routes-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Routes API
  slug: bloomberg-aim-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-routes-api-openapi.yml
- filename: bloomberg-aim-teams-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Teams API
  slug: bloomberg-aim-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-teams-api-openapi.yml
- filename: bloomberg-aim-triggers-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Triggers API
  slug: bloomberg-aim-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-triggers-api-openapi.yml
- filename: bloomberg-aim-universes-api-openapi.yml
  format: yaml
  label: Bloomberg AIM Universes API
  slug: bloomberg-aim-universes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-aim-universes-api-openapi.yml
consequence_counts:
  physical: 9
  read: 16
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bloomberg Aim Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request/blp/emapisvc/AssignTrader
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request/blp/emapisvc/CreateOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request/blp/emapisvc/CreateOrderAndRouteEx
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request/blp/emapisvc/DeleteOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request/blp/emapisvc/GetOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request/blp/emapisvc/GroupRouteEx
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request/blp/emapisvc/ModifyOrderEx
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /request/blp/emapisvc/RouteEx
operation_count: 47
overview: 'Bloomberg AIM exposes 47 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 22 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
slug: bloomberg-aim-agentic-access
source_filename: bloomberg-aim-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bloomberg-data-license-api.yml, openapi/bloomberg-emsx-api.yml, openapi/bloomberg-http-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 16\n    acting: 31\n  by_consequence:\n    read: 16\n    write: 22\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /catalogs\n  method: get\n  operationId: listCatalogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/fields\n  method: get\n  operationId: listCatalogFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/universes\n  method: get\n  operationId: listUniverses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/universes\n  method: post\n  operationId: createUniverse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/{catalogId}/universes/{universeId}\n  method: get\n  operationId: getUniverse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/fieldLists\n  method: get\n  operationId: listFieldLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/fieldLists\n  method: post\n  operationId: createFieldList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/{catalogId}/fieldLists/{fieldListId}\n\
  \  method: get\n  operationId: getFieldList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/triggers\n  method: get\n  operationId: listTriggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/triggers\n  method: post\n  operationId: createTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/{catalogId}/triggers/{triggerId}\n  method: get\n  operationId: getTrigger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /catalogs/{catalogId}/requests\n  method: get\n  operationId: listRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/requests\n  method: post\n  operationId: createRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/{catalogId}/requests/{requestId}\n  method: get\n  operationId: getRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/requests/{requestId}\n  method: delete\n  operationId: deleteRequest\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalogs/{catalogId}/distributions\n  method: get\n  operationId: listDistributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/distributions/{distributionId}\n  method: get\n  operationId: getDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/distributions/{distributionId}/replies\n  method: get\n  operationId: listReplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalogs/{catalogId}/distributions/{distributionId}/replies/{replyId}\n\
  \  method: get\n  operationId: getReply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /request/blp/emapisvc/CreateOrder\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/CreateOrderAndRouteEx\n  method: post\n  operationId: createOrderAndRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /request/blp/emapisvc/ModifyOrderEx\n  method: post\n  operationId: modifyOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/DeleteOrder\n  method: post\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/GroupRouteEx\n  method: post\n  operationId: groupRoute\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/RouteEx\n  method: post\n  operationId: routeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/ModifyRouteEx\n  method: post\n  operationId: modifyRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/DeleteRoute\n  method: post\n  operationId: deleteRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/GetOrders\n  method: post\n  operationId: getOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/GetRoutes\n  method: post\n  operationId: getRoutes\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/GetFills\n  method: post\n  operationId: getFills\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/GetBrokerStrategiesWithAssetClass\n  method: post\n  operationId: getBrokerStrategies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/GetBrokerStrategyInfoWithAssetClass\n\
  \  method: post\n  operationId: getBrokerStrategyInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/GetTeams\n  method: post\n  operationId: getTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/AssignTrader\n  method: post\n  operationId: assignTrader\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/emapisvc/ManualFill\n  method: post\n  operationId: manualFill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request\n  method: post\n  operationId: sendRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/refdata/ReferenceDataRequest\n  method: post\n  operationId: referenceDataRequest\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/refdata/HistoricalDataRequest\n  method: post\n  operationId: historicalDataRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/refdata/IntradayTickRequest\n  method: post\n  operationId: intradayTickRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /request/blp/refdata/IntradayBarRequest\n  method: post\n  operationId: intradayBarRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/refdata/FieldInfoRequest\n  method: post\n  operationId: fieldInfoRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/refdata/FieldSearchRequest\n  method: post\n  operationId: fieldSearchRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/instruments/InstrumentListRequest\n  method: post\n  operationId: instrumentListRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/instruments/CurveListRequest\n  method: post\n  operationId: curveListRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request/blp/instruments/GovernmentLookupRequest\n  method: post\n  operationId: governmentLookupRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/agentic-access/bloomberg-aim-agentic-access.yml
summary_line: 47 operations · 31 acting
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio-Management
- Trading
---
