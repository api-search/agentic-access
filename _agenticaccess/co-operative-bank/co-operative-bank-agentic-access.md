---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: co-operative-bank-atm-api-openapi.yml
  format: yaml
  label: The Co-operative Bank ATM API
  slug: co-operative-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-atm-api-openapi.yml
- filename: co-operative-bank-bca-api-openapi.yml
  format: yaml
  label: The Co-operative Bank BCA API
  slug: co-operative-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-bca-api-openapi.yml
- filename: co-operative-bank-branch-api-openapi.yml
  format: yaml
  label: The Co-operative Bank Branch API
  slug: co-operative-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-branch-api-openapi.yml
- filename: co-operative-bank-ccc-api-openapi.yml
  format: yaml
  label: The Co-operative Bank CCC API
  slug: co-operative-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-ccc-api-openapi.yml
- filename: co-operative-bank-pca-api-openapi.yml
  format: yaml
  label: The Co-operative Bank PCA API
  slug: co-operative-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-pca-api-openapi.yml
- filename: co-operative-bank-sme-api-openapi.yml
  format: yaml
  label: The Co-operative Bank SME API
  slug: co-operative-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/co-operative-bank-sme-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Co Operative Bank Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'The Co-operative Bank exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Co-operative Bank
provider_slug: co-operative-bank
slug: co-operative-bank-agentic-access
source_filename: co-operative-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/obie-open-data-api-standard-swagger.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /branches\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branches\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atms\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /atms\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-current-accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-current-accounts\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-current-accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-current-accounts\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /unsecured-sme-loans\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unsecured-sme-loans\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial-credit-cards\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial-credit-cards\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/agentic-access/co-operative-bank-agentic-access.yml
summary_line: 12 operations
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Fintech
---
