---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 10
api_specs:
- filename: ezoic-access-api-openapi.yml
  format: yaml
  label: ezoic Access API
  slug: ezoic-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-access-api-openapi.yml
- filename: ezoic-products-api-openapi.yml
  format: yaml
  label: ezoic Products API
  slug: ezoic-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-products-api-openapi.yml
- filename: ezoic-purchases-api-openapi.yml
  format: yaml
  label: ezoic Purchases API
  slug: ezoic-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-purchases-api-openapi.yml
- filename: ezoic-cdn-api-openapi.yml
  format: yaml
  label: ezoic CDN API
  slug: ezoic-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-cdn-api-openapi.yml
- filename: ezoic-data-api-openapi.yml
  format: yaml
  label: ezoic Data API
  slug: ezoic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-data-api-openapi.yml
- filename: ezoic-filters-api-openapi.yml
  format: yaml
  label: ezoic Filters API
  slug: ezoic-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-filters-api-openapi.yml
- filename: ezoic-reports-api-openapi.yml
  format: yaml
  label: ezoic Reports API
  slug: ezoic-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-reports-api-openapi.yml
- filename: ezoic-segments-api-openapi.yml
  format: yaml
  label: ezoic Segments API
  slug: ezoic-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-segments-api-openapi.yml
consequence_counts:
  read: 10
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ezoic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'ezoic exposes 19 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ezoic
provider_slug: ezoic
slug: ezoic-agentic-access
source_filename: ezoic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/ezoic-access-api-openapi.yml, openapi/ezoic-cdn-api-openapi.yml, openapi/ezoic-data-api-openapi.yml,\n  openapi/ezoic-filters-api-openapi.yml, openapi/ezoic-products-api-openapi.yml, openapi/ezoic-purchases-api-openapi.yml,\n  openapi/ezoic-reports-api-openapi.yml, openapi/ezoic-segments-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 10\n    acting: 9\n  by_consequence:\n    read: 10\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /access\n  method: get\n  operationId: checkAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /cdnservices/ping/\n  method: post\n  operationId: cdnPing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdnservices/clearcache\n  method: post\n  operationId: clearCache\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdnservices/bulkclearcache\n  method: post\n  operationId: bulkClearCache\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdnservices/clearbysurrogatekeys\n  method: post\n  operationId: clearBySurrogateKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdnservices/purgecache\n  method: post\n  operationId: purgeCache\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bdaservices/getdata/\n  method: post\n  operationId: getData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bdaservices/getCustomData/\n  method: post\n  operationId: getCustomData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bdaservices/getmultifilters/\n  method: get\n  operationId: getMultiFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bdaservices/getmultifiltertypes/\n  method: get\n  operationId: getMultiFilterTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n\
  \  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchases\n  method: get\n  operationId: listPurchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bdaservices/getreports/\n  method: get\n  operationId: getReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bdaservices/getreport/\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bdaservices/getcustomreports/\n  method: get\n  operationId: getCustomReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bdaservices/createcustomreport/\n  method: post\n  operationId: createCustomReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bdaservices/getcolumns/\n  method: get\n  operationId: getColumns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bdaservices/getsegments/\n  method: get\n  operationId: getSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bdaservices/createsegment/\n  method: post\n  operationId: createSegment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/agentic-access/ezoic-agentic-access.yml
summary_line: 19 operations · 9 acting
tags:
- Company
- Advertising
- AdTech
- Publisher Monetization
- Analytics
- Reporting
- Subscription
- Paywalls
- Identity
- CDN
- Caching
- MCP
- Authentication
- Agents
---
