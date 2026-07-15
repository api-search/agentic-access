---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Agencies and Offices API
  slug: hawksoft-agencies-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Clients API
  slug: hawksoft-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Log Entries API
  slug: hawksoft-log-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
- filename: hawksoft-openapi.yml
  format: yaml
  label: HawkSoft Attachments and Receipts API
  slug: hawksoft-attachments-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/openapi/hawksoft-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hawksoft Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vendor/agency/{agencyId}/client/{clientId}/receipts
operation_count: 9
overview: 'HawkSoft exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HawkSoft
provider_slug: hawksoft
slug: hawksoft-agentic-access
source_filename: hawksoft-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hawksoft-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /vendor/agencies\n  method: get\n  operationId: listAgencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/agency/{agencyId}/offices\n  method: get\n  operationId: listOffices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/agency/{agencyId}/clients\n\
  \  method: get\n  operationId: listChangedClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/agency/{agencyId}/clients\n  method: post\n  operationId: getClientList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/agency/{agencyId}/clients/search\n  method: get\n  operationId: searchClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vendor/agency/{agencyId}/client/{clientId}\n  method: get\n  operationId: getClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /vendor/agency/{agencyId}/client/{clientId}/log\n  method: post\n  operationId: postLogNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/agency/{agencyId}/client/{clientId}/attachment\n  method: post\n  operationId: postAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendor/agency/{agencyId}/client/{clientId}/receipts\n  method: post\n  operationId: postReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawksoft/refs/heads/main/agentic-access/hawksoft-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Insurance
- Agency Management System
- AMS
- InsurTech
- Property and Casualty
- Partner API
- Gated API
---
