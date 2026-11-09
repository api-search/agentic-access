---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 11
api_specs:
- filename: treezor-beneficiaries-api-openapi.yml
  format: yaml
  label: Treezor Beneficiaries API
  slug: treezor-beneficiaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-beneficiaries-api-openapi.yml
- filename: treezor-cardimages-api-openapi.yml
  format: yaml
  label: Treezor Cardimages API
  slug: treezor-cardimages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-cardimages-api-openapi.yml
- filename: treezor-cards-api-openapi.yml
  format: yaml
  label: Treezor Cards API
  slug: treezor-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-cards-api-openapi.yml
- filename: treezor-core-connect-api-openapi.yml
  format: yaml
  label: Treezor Core Connect API
  slug: treezor-core-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-core-connect-api-openapi.yml
- filename: treezor-customization-api-openapi.yml
  format: yaml
  label: Treezor Customization API
  slug: treezor-customization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-customization-api-openapi.yml
- filename: treezor-default-api-openapi.yml
  format: yaml
  label: Treezor [...] API
  slug: treezor-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-default-api-openapi.yml
- filename: treezor-documents-api-openapi.yml
  format: yaml
  label: Treezor Documents API
  slug: treezor-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-documents-api-openapi.yml
- filename: treezor-oauth-api-openapi.yml
  format: yaml
  label: Treezor OAuth API
  slug: treezor-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-oauth-api-openapi.yml
- filename: treezor-retry-api-openapi.yml
  format: yaml
  label: Treezor Retry API
  slug: treezor-retry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-retry-api-openapi.yml
- filename: treezor-simulation-api-openapi.yml
  format: yaml
  label: Treezor Simulation API
  slug: treezor-simulation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-simulation-api-openapi.yml
- filename: treezor-treezor-api-api-openapi.yml
  format: yaml
  label: Treezor Treezor API
  slug: treezor-treezor-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-treezor-api-api-openapi.yml
- filename: treezor-users-api-openapi.yml
  format: yaml
  label: Treezor Users API
  slug: treezor-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-users-api-openapi.yml
- filename: treezor-wallets-api-openapi.yml
  format: yaml
  label: Treezor Wallets API
  slug: treezor-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/treezor/openapi/treezor-wallets-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Treezor Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /retry/{retryid}
operation_count: 26
overview: 'Treezor exposes 26 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 14 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Treezor
provider_slug: treezor
slug: treezor-agentic-access
source_filename: treezor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/treezor-beneficiaries-api-openapi.yml, openapi/treezor-cardimages-api-openapi.yml,\n  openapi/treezor-cards-api-openapi.yml, openapi/treezor-core-connect-api-openapi.yml, openapi/treezor-customization-api-openapi.yml,\n  openapi/treezor-default-api-openapi.yml, openapi/treezor-documents-api-openapi.yml, openapi/treezor-oauth-api-openapi.yml,\n  openapi/treezor-retry-api-openapi.yml, openapi/treezor-simulation-api-openapi.yml, openapi/treezor-treezor-api-api-openapi.yml,\n  openapi/treezor-users-api-openapi.yml, openapi/treezor-wallets-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 15\n    connected: 11\n  by_consequence:\n    write:\
  \ 14\n    read: 11\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /beneficiaries\n  method: post\n  operationId: post_beneficiaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries\n  method: post\n  operationId: post_v1_beneficiaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cardimages\n  method: get\n  operationId: get_v1_cardimages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /cards\n  method: post\n  operationId: post_cards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardid}/cardImage\n  method: get\n  operationId: get_cards_cardid_cardImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{cardid}\n  method: post\n  operationId: post_v1_cards_cardid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{cardid}/{id}\n  method: put\n  operationId:\
  \ put_v1_cards_cardid_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{id}/Activate\n  method: put\n  operationId: put_v1_cards_id_Activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core-connect/card/bulk\n  method: get\n  operationId: get_core_connect_card_bulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core-connect/card/bulk\n  method: post\n  operationId: post_core_connect_card_bulk\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core-connect/sca/scaOperations\n  method: post\n  operationId: post_core_connect_sca_scaOperations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core-connect/sca/scaOperations/{id}\n  method: get\n  operationId: get_core_connect_sca_scaOperations_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core-connect/sca/scaOperations/{id}\n  method: put\n  operationId:\
  \ put_core_connect_sca_scaOperations_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core-connect/sca/scawallets/{scawalletid}\n  method: get\n  operationId: get_core_connect_sca_scawallets_scawalletid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core-connect/sca/{scaid}\n  method: get\n  operationId: get_core_connect_sca_scaid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customization/templates/{templatename}/example\n  method: get\n  operationId: get_customization_templates_templatename_example\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /[...]\n  method: post\n  operationId: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: get\n  operationId: get_documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: post_oauth_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /retry/exec/{executionid}\n  method: get\n  operationId: get_retry_exec_executionid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retry/{retryid}\n  method: post\n  operationId: post_retry_retryid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /simulation/scaProof\n  method: post\n  operationId: post_simulation_scaProof\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{userid}\n  method: put\n  operationId: put_v1_users_userid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets\n  method: get\n  operationId: get_wallets\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/treezor/agentic-access/treezor-agentic-access.yml
summary_line: 26 operations · 15 acting
tags:
- Fintech
- Payments
- Banking as a Service
- Europe
---
