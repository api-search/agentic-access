---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: utilityhouse-xyz-grants-api-openapi.yml
  format: yaml
  label: utilityhouse-xyz Grants API
  slug: utilityhouse-xyz-grants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/utilityhouse-xyz/openapi/utilityhouse-xyz-grants-api-openapi.yml
- filename: utilityhouse-xyz-woo-api-openapi.yml
  format: yaml
  label: utilityhouse-xyz Woo API
  slug: utilityhouse-xyz-woo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/utilityhouse-xyz/openapi/utilityhouse-xyz-woo-api-openapi.yml
- filename: utilityhouse-xyz-wp-updates-api-openapi.yml
  format: yaml
  label: utilityhouse-xyz Wp Updates API
  slug: utilityhouse-xyz-wp-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/utilityhouse-xyz/openapi/utilityhouse-xyz-wp-updates-api-openapi.yml
consequence_counts:
  physical: 1
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Utilityhouse Xyz Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/woo/release-risk
operation_count: 7
overview: 'utilityhouse-xyz exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: utilityhouse-xyz
provider_slug: utilityhouse-xyz
slug: utilityhouse-xyz-agentic-access
source_filename: utilityhouse-xyz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/utilityhouse-xyz-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 2\n    acting: 5\n  by_consequence:\n    read: 2\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/grants/search\n  method: post\n  operationId: search_federal_grants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/grants/analyze\n  method: post\n  operationId: analyze_federal_grant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/grants/evidence-pack\n  method: post\n  operationId: get_federal_grant_evidence_pack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wp-updates/check\n  method: post\n  operationId: wp_update_radar_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/wp-updates/check-many\n  method: post\n  operationId: wp_update_radar_check_many\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/woo/readiness-scan\n  method: post\n  operationId: scan_woo_store_readiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/woo/release-risk\n  method: post\n  operationId: check_checkout_change_risk\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/utilityhouse-xyz/agentic-access/utilityhouse-xyz-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- Company
- Software
- Grants
- WordPress
- WooCommerce
---
