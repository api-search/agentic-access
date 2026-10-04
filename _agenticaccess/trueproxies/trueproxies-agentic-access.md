---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 14
api_specs:
- filename: trueproxies-analytics-api-openapi.yml
  format: yaml
  label: TrueProxies Analytics API
  slug: trueproxies-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trueproxies/refs/heads/main/openapi/trueproxies-analytics-api-openapi.yml
- filename: trueproxies-catalog-api-openapi.yml
  format: yaml
  label: TrueProxies Catalog API
  slug: trueproxies-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trueproxies/refs/heads/main/openapi/trueproxies-catalog-api-openapi.yml
- filename: trueproxies-invoices-api-openapi.yml
  format: yaml
  label: TrueProxies Invoices API
  slug: trueproxies-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trueproxies/refs/heads/main/openapi/trueproxies-invoices-api-openapi.yml
- filename: trueproxies-me-api-openapi.yml
  format: yaml
  label: TrueProxies Me API
  slug: trueproxies-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trueproxies/refs/heads/main/openapi/trueproxies-me-api-openapi.yml
- filename: trueproxies-services-api-openapi.yml
  format: yaml
  label: TrueProxies Services API
  slug: trueproxies-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trueproxies/refs/heads/main/openapi/trueproxies-services-api-openapi.yml
consequence_counts:
  physical: 2
  read: 14
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trueproxies Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoices/{id}/pay
operation_count: 21
overview: 'TrueProxies exposes 21 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TrueProxies
provider_slug: trueproxies
slug: trueproxies-agentic-access
source_filename: trueproxies-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/trueproxies-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 14\n    acting: 7\n  by_consequence:\n    read: 14\n    physical: 2\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/analytics\n  method: get\n  operationId: get_v1_analytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog\n  method: get\n  operationId: get_v1_catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/priced\n\
  \  method: get\n  operationId: get_v1_catalog_priced\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices\n  method: get\n  operationId: get_v1_invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices\n  method: post\n  operationId: post_v1_invoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoices/{id}\n  method: get\n  operationId: get_v1_invoices_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/{id}/pay\n  method: post\n  operationId: post_v1_invoices_id_pay\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoices/{id}/pdf\n  method: get\n  operationId: get_v1_invoices_id_pdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: get_v1_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services\n  method: get\n  operationId: get_v1_services\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{id}\n  method: get\n  operationId: get_v1_services_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{id}/analytics\n  method: get\n  operationId: get_v1_services_id_analytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{id}/check\n  method: post\n  operationId: post_v1_services_id_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/services/{id}/endpoints\n  method: post\n  operationId:\
  \ post_v1_services_id_endpoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/services/{id}/live-metrics\n  method: get\n  operationId: get_v1_services_id_live_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{id}/rotate-password\n  method: post\n  operationId: post_v1_services_id_rotate_password\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/services/{id}/secret\n  method: get\n  operationId:\
  \ get_v1_services_id_secret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{id}/usage\n  method: get\n  operationId: get_v1_services_id_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{id}/whitelist\n  method: get\n  operationId: get_v1_services_id_whitelist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{id}/whitelist\n  method: post\n  operationId: post_v1_services_id_whitelist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/services/{id}/whitelist/{entryId}\n  method: delete\n  operationId: delete_v1_services_id_whitelist_entryId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trueproxies/refs/heads/main/agentic-access/trueproxies-agentic-access.yml
summary_line: 21 operations · 7 acting
tags:
- Proxies
- Residential Proxies
- Datacenter Proxies
- Web Scraping
- Networking
- IPv6
- SOCKS5
- Data Collection
---
