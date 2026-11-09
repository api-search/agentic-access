---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 13
api_specs:
- filename: platfone-com-activation-report-api-openapi.yml
  format: yaml
  label: platfone-com Activation Report API
  slug: platfone-com-activation-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/platfone-com/openapi/platfone-com-activation-report-api-openapi.yml
- filename: platfone-com-catalog-api-openapi.yml
  format: yaml
  label: platfone-com Catalog API
  slug: platfone-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/platfone-com/openapi/platfone-com-catalog-api-openapi.yml
- filename: platfone-com-prices-api-openapi.yml
  format: yaml
  label: platfone-com Prices API
  slug: platfone-com-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/platfone-com/openapi/platfone-com-prices-api-openapi.yml
- filename: platfone-com-sms-activation-api-openapi.yml
  format: yaml
  label: platfone-com SMS Activation API
  slug: platfone-com-sms-activation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/platfone-com/openapi/platfone-com-sms-activation-api-openapi.yml
- filename: platfone-com-user-api-openapi.yml
  format: yaml
  label: platfone-com User API
  slug: platfone-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/platfone-com/openapi/platfone-com-user-api-openapi.yml
- filename: platfone-com-webhooks-api-openapi.yml
  format: yaml
  label: platfone-com Webhooks 📡 API
  slug: platfone-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/platfone-com/openapi/platfone-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Platfone Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /activation
operation_count: 18
overview: 'platfone-com exposes 18 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: platfone-com
provider_slug: platfone-com
slug: platfone-com-agentic-access
source_filename: platfone-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/platfone-com-activation-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 13\n    acting: 5\n  by_consequence:\n    read: 13\n    physical: 1\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /user/balance\n  method: get\n  operationId: getUserBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation/countries\n  method: get\n  operationId: getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /activation/services\n  method: get\n  operationId: getServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation/services/popular\n  method: get\n  operationId: getPopularServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation/prices/services/{service_id}/countries/{country_id}\n  method: get\n  operationId: getPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation/prices/countries\n  method: get\n  operationId: getPriceByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation/prices/services\n  method: get\n  operationId:\
  \ getPriceByService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation\n  method: post\n  operationId: newActivation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activation/{activation_id}\n  method: get\n  operationId: getActivation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation/{activation_id}/retry\n  method: put\n  operationId: retryActivation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activation/{activation_id}/cancel\n  method: put\n  operationId: cancelActivation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activation/{activation_id}/finalize\n  method: put\n  operationId: finalizeActivation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activation/history\n  method: get\n  operationId: getActivationsHistory\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wl/activation/history\n  method: get\n  operationId: getWhitelabelCustomersActivationHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation/{activation_id}/report/reasons\n  method: get\n  operationId: getActivationReportReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation/{activation_id}/report\n  method: post\n  operationId: reportActivation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /activation/{activation_id}/report\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activation/reports\n  method: get\n  operationId: getReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/platfone-com/agentic-access/platfone-com-agentic-access.yml
summary_line: 18 operations · 5 acting
tags:
- Company
- Telecommunications
- SMS
- Temporary-Numbers
---
