---
acting_count: 51
action_class_counts:
  acting: 51
  connected: 36
api_specs:
- filename: immix-account-addresses-api-openapi.yml
  format: yaml
  label: IMMIX Account addresses API
  slug: immix-account-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-account-addresses-api-openapi.yml
- filename: immix-account-balances-api-openapi.yml
  format: yaml
  label: IMMIX Account balances API
  slug: immix-account-balances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-account-balances-api-openapi.yml
- filename: immix-accounts-api-openapi.yml
  format: yaml
  label: IMMIX Accounts API
  slug: immix-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-accounts-api-openapi.yml
- filename: immix-algos-api-openapi.yml
  format: yaml
  label: IMMIX Algos API
  slug: immix-algos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-algos-api-openapi.yml
- filename: immix-asset-policies-api-openapi.yml
  format: yaml
  label: IMMIX Asset policies API
  slug: immix-asset-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-asset-policies-api-openapi.yml
- filename: immix-assets-api-openapi.yml
  format: yaml
  label: IMMIX Assets API
  slug: immix-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-assets-api-openapi.yml
- filename: immix-chain-policies-api-openapi.yml
  format: yaml
  label: IMMIX Chain policies API
  slug: immix-chain-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-chain-policies-api-openapi.yml
- filename: immix-credentials-api-openapi.yml
  format: yaml
  label: IMMIX Credentials API
  slug: immix-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-credentials-api-openapi.yml
- filename: immix-enquiry-api-openapi.yml
  format: yaml
  label: IMMIX Enquiry API
  slug: immix-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-enquiry-api-openapi.yml
- filename: immix-executions-api-openapi.yml
  format: yaml
  label: IMMIX Executions API
  slug: immix-executions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-executions-api-openapi.yml
- filename: immix-instruments-api-openapi.yml
  format: yaml
  label: IMMIX Instruments API
  slug: immix-instruments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-instruments-api-openapi.yml
- filename: immix-operations-api-openapi.yml
  format: yaml
  label: IMMIX Operations API
  slug: immix-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-operations-api-openapi.yml
- filename: immix-orders-api-openapi.yml
  format: yaml
  label: IMMIX Orders API
  slug: immix-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-orders-api-openapi.yml
- filename: immix-portfolios-api-openapi.yml
  format: yaml
  label: IMMIX Portfolios API
  slug: immix-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-portfolios-api-openapi.yml
- filename: immix-trading-policies-api-openapi.yml
  format: yaml
  label: IMMIX Trading policies API
  slug: immix-trading-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-trading-policies-api-openapi.yml
- filename: immix-users-api-openapi.yml
  format: yaml
  label: IMMIX Users API
  slug: immix-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-users-api-openapi.yml
- filename: immix-venues-api-openapi.yml
  format: yaml
  label: IMMIX Venues API
  slug: immix-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immix/openapi/immix-venues-api-openapi.yml
consequence_counts:
  physical: 7
  read: 36
  safety-critical: 5
  write: 39
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Immix Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /algos/halt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /algos/instances/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /credentials/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /trading-policies/{id}/halt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users/{id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{id}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /asset-policies/{id}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chain-policies/{id}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /credentials/{id}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trading-policies/{id}/withdraw
operation_count: 87
overview: 'IMMIX exposes 87 API operations that an AI agent could call, of which 51 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read, 39 write, 7 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IMMIX
provider_slug: immix
slug: immix-agentic-access
source_filename: immix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/immix-enquiry-openapi.json, openapi/immix-rest-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 87\n  by_action_class:\n    acting: 51\n    connected: 36\n  by_consequence:\n    write: 39\n    read: 36\n    safety-critical: 5\n    physical: 7\n  human_in_the_loop_required: 5\noperations:\n- path: /api/leads\n  method: post\n  operationId: submitLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: users_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: users_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: get\n  operationId: users_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: put\n  operationId: users_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /users/{id}/disable\n  method: post\n  operationId: users_disable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/invitations\n  method: post\n  operationId: users_invite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/invitation\n  method: post\n  operationId: users_reinvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId: users_get_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/orgs\n  method: get\n  operationId: users_get_my_orgs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials\n  method: get\n  operationId: credentials_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials\n  method: post\n  operationId: credentials_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credentials/{id}\n  method: get\n  operationId: credentials_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials/{id}\n  method: put\n  operationId: credentials_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credentials/{id}/approve\n  method: post\n  operationId: credentials_approve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /credentials/{id}/suspend\n  method: post\n  operationId: credentials_suspend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credentials/{id}/reactivate\n  method: post\n  operationId: credentials_reactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credentials/{id}/revoke\n  method: post\n  operationId: credentials_revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /credentials/{id}/rotate\n  method: post\n  operationId: credentials_rotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credentials/{id}/withdraw\n  method: post\n  operationId: credentials_withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method:\
  \ get\n  operationId: accounts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}\n  method: get\n  operationId: accounts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}/classify\n  method: post\n  operationId: accounts_classify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}/approve\n  method: post\n  operationId: accounts_approve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}/freeze\n  method: post\n  operationId: accounts_freeze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}/unfreeze\n  method: post\n  operationId: accounts_unfreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}/retire\n  method: post\n  operationId: accounts_retire\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}/withdraw\n  method: post\n  operationId: accounts_withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolios\n  method: get\n  operationId: portfolios_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolios\n  method: post\n  operationId: portfolios_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolios/{id}\n  method: get\n  operationId: portfolios_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolios/{id}\n  method: put\n  operationId: portfolios_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolios/{id}/retire\n  method: post\n  operationId: portfolios_retire\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-addresses\n  method: get\n  operationId: accountAddresses_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-addresses\n  method: post\n  operationId: accountAddresses_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-addresses/{id}\n  method: get\n  operationId: accountAddresses_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-addresses/{id}/verify\n  method: post\n  operationId: accountAddresses_verify\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-addresses/{id}/retire\n  method: post\n  operationId: accountAddresses_retire\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trading-policies\n  method: get\n  operationId: tradingPolicies_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trading-policies\n  method: post\n  operationId: tradingPolicies_create\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trading-policies/{id}\n  method: get\n  operationId: tradingPolicies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trading-policies/{id}\n  method: put\n  operationId: tradingPolicies_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trading-policies/{id}/approve\n  method: post\n  operationId: tradingPolicies_approve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trading-policies/{id}/retire\n  method: post\n  operationId: tradingPolicies_retire\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trading-policies/{id}/withdraw\n  method: post\n  operationId: tradingPolicies_withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /trading-policies/{id}/halt\n  method: post\n  operationId: tradingPolicies_halt\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /trading-policies/{id}/resume\n  method: post\n  operationId: tradingPolicies_resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset-policies\n  method: get\n  operationId: assetPolicies_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset-policies\n\
  \  method: post\n  operationId: assetPolicies_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset-policies/{id}\n  method: get\n  operationId: assetPolicies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset-policies/{id}\n  method: put\n  operationId: assetPolicies_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset-policies/{id}/approve\n  method: post\n  operationId: assetPolicies_approve\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset-policies/{id}/retire\n  method: post\n  operationId: assetPolicies_retire\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset-policies/{id}/withdraw\n  method: post\n  operationId: assetPolicies_withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain-policies\n  method: get\n  operationId: chainPolicies_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain-policies\n  method: post\n  operationId: chainPolicies_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain-policies/{id}\n  method: get\n  operationId: chainPolicies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain-policies/{id}\n  method: put\n  operationId: chainPolicies_update\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain-policies/{id}/approve\n  method: post\n  operationId: chainPolicies_approve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain-policies/{id}/retire\n  method: post\n  operationId: chainPolicies_retire\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chain-policies/{id}/withdraw\n\
  \  method: post\n  operationId: chainPolicies_withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: orders_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: orders_submit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}\n\
  \  method: get\n  operationId: orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}/cancel\n  method: post\n  operationId: orders_cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /executions\n  method: get\n  operationId: executions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /executions/{id}\n  method: get\n  operationId: executions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /account-balances\n  method: get\n  operationId: accountBalances_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /algos/instances\n  method: get\n  operationId: algos_list_instances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /algos/instances\n  method: post\n  operationId: algos_create_instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /algos/instances/{id}\n  method: get\n  operationId: algos_get_instance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /algos/instances/{id}/config\n  method: put\n  operationId: algos_update_instance_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /algos/instances/{id}/configs\n  method: get\n  operationId: algos_list_instance_configs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /algos/instances/{id}/configs/{seq}\n  method: get\n  operationId: algos_get_instance_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /algos/instances/{id}/orders\n  method: get\n  operationId: algos_list_instance_orders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /algos/instances/{id}/start\n  method: post\n  operationId: algos_start_instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /algos/instances/{id}/stop\n  method: post\n  operationId: algos_stop_instance\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /algos/instances/{id}/delete\n  method: post\n  operationId: algos_delete_instance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /algos/halt\n  method: post\n  operationId: algos_halt\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /algos/versions\n  method: get\n  operationId: algos_list_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /venues\n  method: get\n  operationId: venues_list\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /venues/{venueId}\n  method: get\n  operationId: venues_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments\n  method: get\n  operationId: instruments_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instruments/{instrumentId}\n  method: get\n  operationId: instruments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets\n  method: get\n  operationId: assets_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetId}\n  method: get\n  operationId:\
  \ assets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/{key}\n  method: get\n  operationId: operations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/immix/agentic-access/immix-agentic-access.yml
summary_line: 87 operations · 51 acting · 5 human-in-the-loop
tags:
- Company
- Fintech
- Stablecoins
- Foreign Exchange
- Artificial Intelligence
---
