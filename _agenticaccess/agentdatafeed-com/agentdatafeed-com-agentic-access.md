---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 27
api_specs:
- filename: agentdatafeed-com-amsterdam-events-api-openapi.yml
  format: yaml
  label: AgentDataFeed Amsterdam Events API
  slug: agentdatafeed-com-amsterdam-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-amsterdam-events-api-openapi.yml
- filename: agentdatafeed-com-cert-advisories-api-openapi.yml
  format: yaml
  label: AgentDataFeed Cert Advisories API
  slug: agentdatafeed-com-cert-advisories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-cert-advisories-api-openapi.yml
- filename: agentdatafeed-com-datasets-api-openapi.yml
  format: yaml
  label: AgentDataFeed Datasets API
  slug: agentdatafeed-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-datasets-api-openapi.yml
- filename: agentdatafeed-com-drug-shortages-api-openapi.yml
  format: yaml
  label: AgentDataFeed Drug Shortages API
  slug: agentdatafeed-com-drug-shortages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-drug-shortages-api-openapi.yml
- filename: agentdatafeed-com-eu-funding-api-openapi.yml
  format: yaml
  label: AgentDataFeed Eu Funding API
  slug: agentdatafeed-com-eu-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-eu-funding-api-openapi.yml
- filename: agentdatafeed-com-eu-legislation-api-openapi.yml
  format: yaml
  label: AgentDataFeed Eu Legislation API
  slug: agentdatafeed-com-eu-legislation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-eu-legislation-api-openapi.yml
- filename: agentdatafeed-com-eu-medicines-api-openapi.yml
  format: yaml
  label: AgentDataFeed Eu Medicines API
  slug: agentdatafeed-com-eu-medicines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-eu-medicines-api-openapi.yml
- filename: agentdatafeed-com-eu-tenders-api-openapi.yml
  format: yaml
  label: AgentDataFeed Eu Tenders API
  slug: agentdatafeed-com-eu-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-eu-tenders-api-openapi.yml
- filename: agentdatafeed-com-feedback-api-openapi.yml
  format: yaml
  label: AgentDataFeed Feedback API
  slug: agentdatafeed-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-feedback-api-openapi.yml
- filename: agentdatafeed-com-product-recalls-api-openapi.yml
  format: yaml
  label: AgentDataFeed Product Recalls API
  slug: agentdatafeed-com-product-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-product-recalls-api-openapi.yml
- filename: agentdatafeed-com-public-holidays-api-openapi.yml
  format: yaml
  label: AgentDataFeed Public Holidays API
  slug: agentdatafeed-com-public-holidays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-public-holidays-api-openapi.yml
- filename: agentdatafeed-com-sanctions-entities-api-openapi.yml
  format: yaml
  label: AgentDataFeed Sanctions Entities API
  slug: agentdatafeed-com-sanctions-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-sanctions-entities-api-openapi.yml
- filename: agentdatafeed-com-security-advisories-api-openapi.yml
  format: yaml
  label: AgentDataFeed Security Advisories API
  slug: agentdatafeed-com-security-advisories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-security-advisories-api-openapi.yml
- filename: agentdatafeed-com-uk-tenders-api-openapi.yml
  format: yaml
  label: AgentDataFeed Uk Tenders API
  slug: agentdatafeed-com-uk-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-uk-tenders-api-openapi.yml
- filename: agentdatafeed-com-vulnerability-watch-api-openapi.yml
  format: yaml
  label: AgentDataFeed Vulnerability Watch API
  slug: agentdatafeed-com-vulnerability-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdatafeed-com/openapi/agentdatafeed-com-vulnerability-watch-api-openapi.yml
consequence_counts:
  physical: 1
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentdatafeed Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/feedback
operation_count: 28
overview: 'AgentDataFeed exposes 28 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentDataFeed
provider_slug: agentdatafeed-com
slug: agentdatafeed-com-agentic-access
source_filename: agentdatafeed-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentdatafeed-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 27\n    acting: 1\n  by_consequence:\n    read: 27\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback\n  method: post\n  operationId: sendFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/amsterdam-events\n  method: get\n  operationId: query_amsterdam_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/amsterdam-events/sample\n  method: get\n  operationId: sample_amsterdam_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/security-advisories\n  method: get\n  operationId: query_security_advisories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/security-advisories/sample\n  method: get\n  operationId: sample_security_advisories\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vulnerability-watch\n  method: get\n  operationId: query_vulnerability_watch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vulnerability-watch/sample\n  method: get\n  operationId: sample_vulnerability_watch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eu-tenders\n  method: get\n  operationId: query_eu_tenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eu-tenders/sample\n  method: get\n  operationId: sample_eu_tenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/uk-tenders\n  method: get\n  operationId: query_uk_tenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/uk-tenders/sample\n  method: get\n  operationId: sample_uk_tenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eu-funding\n  method: get\n  operationId: query_eu_funding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eu-funding/sample\n  method: get\n  operationId: sample_eu_funding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cert-advisories\n  method: get\n  operationId: query_cert_advisories\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cert-advisories/sample\n  method: get\n  operationId: sample_cert_advisories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eu-medicines\n  method: get\n  operationId: query_eu_medicines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eu-medicines/sample\n  method: get\n  operationId: sample_eu_medicines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sanctions-entities\n  method: get\n  operationId: query_sanctions_entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/sanctions-entities/sample\n  method: get\n  operationId: sample_sanctions_entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/product-recalls\n  method: get\n  operationId: query_product_recalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/product-recalls/sample\n  method: get\n  operationId: sample_product_recalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eu-legislation\n  method: get\n  operationId: query_eu_legislation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eu-legislation/sample\n  method:\
  \ get\n  operationId: sample_eu_legislation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drug-shortages\n  method: get\n  operationId: query_drug_shortages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/drug-shortages/sample\n  method: get\n  operationId: sample_drug_shortages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-holidays\n  method: get\n  operationId: query_public_holidays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-holidays/sample\n  method: get\n  operationId: sample_public_holidays\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentdatafeed-com/agentic-access/agentdatafeed-com-agentic-access.yml
summary_line: 28 operations · 1 acting
tags:
- Data
- Artificial Intelligence
- Public Sector
- Datasets
- Payments
---
