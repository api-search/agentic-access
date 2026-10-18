---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 2
api_specs:
- filename: bloomberg-apis-apiflds-api-openapi.yml
  format: yaml
  label: Bloomberg APIs Apiflds API
  slug: bloomberg-apis-apiflds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-apiflds-api-openapi.yml
- filename: bloomberg-apis-instruments-api-openapi.yml
  format: yaml
  label: Bloomberg APIs Instruments API
  slug: bloomberg-apis-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-instruments-api-openapi.yml
- filename: bloomberg-apis-mktbar-api-openapi.yml
  format: yaml
  label: Bloomberg APIs Mktbar API
  slug: bloomberg-apis-mktbar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-mktbar-api-openapi.yml
- filename: bloomberg-apis-mktdata-api-openapi.yml
  format: yaml
  label: Bloomberg APIs Mktdata API
  slug: bloomberg-apis-mktdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-mktdata-api-openapi.yml
- filename: bloomberg-apis-mktvwap-api-openapi.yml
  format: yaml
  label: Bloomberg APIs Mktvwap API
  slug: bloomberg-apis-mktvwap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-mktvwap-api-openapi.yml
- filename: bloomberg-apis-pagedata-api-openapi.yml
  format: yaml
  label: Bloomberg APIs Pagedata API
  slug: bloomberg-apis-pagedata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-pagedata-api-openapi.yml
- filename: bloomberg-apis-tasvc-api-openapi.yml
  format: yaml
  label: Bloomberg APIs Tasvc API
  slug: bloomberg-apis-tasvc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-tasvc-api-openapi.yml
- filename: bloomberg-apis-api-auth-api-openapi.yml
  format: yaml
  label: Bloomberg APIs API Auth API
  slug: bloomberg-apis-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-api-auth-api-openapi.yml
- filename: bloomberg-apis-ref-data-api-openapi.yml
  format: yaml
  label: Bloomberg APIs Ref Data API
  slug: bloomberg-apis-ref-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-ref-data-api-openapi.yml
consequence_counts:
  read: 2
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bloomberg Apis Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Bloomberg APIs exposes 22 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bloomberg APIs
provider_slug: bloomberg-apis
slug: bloomberg-apis-agentic-access
source_filename: bloomberg-apis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/bloomberg-apis-api-auth-api-openapi.yml, openapi/bloomberg-apis-apiflds-api-openapi.yml,\n  openapi/bloomberg-apis-instruments-api-openapi.yml, openapi/bloomberg-apis-mktbar-api-openapi.yml,\n  openapi/bloomberg-apis-mktdata-api-openapi.yml, openapi/bloomberg-apis-mktvwap-api-openapi.yml,\n  openapi/bloomberg-apis-pagedata-api-openapi.yml, openapi/bloomberg-apis-ref-data-api-openapi.yml,\n  openapi/bloomberg-apis-tasvc-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 20\n    connected: 2\n  by_consequence:\n    write: 20\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /apiauth/AuthorizationRequest\n  method: post\n\
  \  operationId: authorizationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apiauth/LogonStatusRequest\n  method: post\n  operationId: logonStatusRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apiauth/UserEntitlementsRequest\n  method: post\n  operationId: userEntitlementsRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apiauth/SecurityEntitlementsRequest\n  method: post\n  operationId:\
  \ securityEntitlementsRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apiauth/AuthorizationTokenRequest\n  method: post\n  operationId: authorizationTokenRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apiflds/FieldInfoRequest\n  method: post\n  operationId: fieldInfoRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /apiflds/FieldSearchRequest\n  method: post\n  operationId: fieldSearchRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apiflds/CategorizedFieldSearchRequest\n  method: post\n  operationId: categorizedFieldSearchRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/SecurityLookupRequest\n  method: post\n  operationId: securityLookupRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /instruments/CurveLookupRequest\n  method: post\n  operationId: curveLookupRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instruments/GovtLookupRequest\n  method: post\n  operationId: govtLookupRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mktbar/subscribe\n  method: post\n  operationId: marketBarSubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mktdata/subscribe\n  method: post\n  operationId: marketDataSubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mktvwap/subscribe\n  method: post\n  operationId: customVWAPSubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pagedata/subscribe\n  method: post\n  operationId: pageDataSubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refdata/ReferenceDataRequest\n  method: post\n  operationId: referenceDataRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refdata/HistoricalDataRequest\n  method: post\n  operationId: historicalDataRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refdata/IntradayTickRequest\n  method: post\n \
  \ operationId: intradayTickRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refdata/IntradayBarRequest\n  method: post\n  operationId: intradayBarRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refdata/PortfolioDataRequest\n  method: post\n  operationId: portfolioDataRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /refdata/BeqsRequest\n  method: post\n  operationId: beqsRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasvc/StudyRequest\n  method: post\n  operationId: studyRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/agentic-access/bloomberg-apis-agentic-access.yml
summary_line: 22 operations · 20 acting
tags:
- Analytics
- Financial Data
- Market Data
- News
- Terminal
---
