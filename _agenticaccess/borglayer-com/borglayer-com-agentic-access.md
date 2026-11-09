---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 12
api_specs:
- filename: borglayer-com-balance-api-openapi.yml
  format: yaml
  label: BorgLayer Balance API
  slug: borglayer-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-balance-api-openapi.yml
- filename: borglayer-com-chains-api-openapi.yml
  format: yaml
  label: BorgLayer Chains API
  slug: borglayer-com-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-chains-api-openapi.yml
- filename: borglayer-com-domains-api-openapi.yml
  format: yaml
  label: BorgLayer Domains API
  slug: borglayer-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-domains-api-openapi.yml
- filename: borglayer-com-formation-api-openapi.yml
  format: yaml
  label: BorgLayer Formation API
  slug: borglayer-com-formation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-formation-api-openapi.yml
- filename: borglayer-com-marketplace-api-openapi.yml
  format: yaml
  label: BorgLayer Marketplace API
  slug: borglayer-com-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-marketplace-api-openapi.yml
- filename: borglayer-com-register-api-openapi.yml
  format: yaml
  label: BorgLayer Register API
  slug: borglayer-com-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-register-api-openapi.yml
- filename: borglayer-com-registrant-profiles-api-openapi.yml
  format: yaml
  label: BorgLayer Registrant Profiles API
  slug: borglayer-com-registrant-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-registrant-profiles-api-openapi.yml
- filename: borglayer-com-search-api-openapi.yml
  format: yaml
  label: BorgLayer Search API
  slug: borglayer-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-search-api-openapi.yml
- filename: borglayer-com-transfer-in-api-openapi.yml
  format: yaml
  label: BorgLayer Transfer In API
  slug: borglayer-com-transfer-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-transfer-in-api-openapi.yml
consequence_counts:
  physical: 2
  read: 12
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Borglayer Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /marketplace/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer-in
operation_count: 20
overview: 'BorgLayer exposes 20 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BorgLayer
provider_slug: borglayer-com
slug: borglayer-com-agentic-access
source_filename: borglayer-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/borglayer-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 12\n    acting: 8\n  by_consequence:\n    read: 12\n    write: 6\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chains\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /register\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer-in\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{domain}/dns\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}/dns\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{domain}/dns/{recordId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registrant-profiles\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registrant-profiles\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registrant-profiles/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /formation/quote\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /formation\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /formation/{reference}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketplace/listings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketplace/listings/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketplace/checkout\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /marketplace/orders/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketplace/earnings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/borglayer-com/agentic-access/borglayer-com-agentic-access.yml
summary_line: 20 operations · 8 acting
tags:
- Company
- Wallets
- Domains
- Hosting
- Email
---
