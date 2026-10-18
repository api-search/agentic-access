---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 26
api_specs:
- filename: wisdomtree-accruals-api-openapi.yml
  format: yaml
  label: WisdomTree Accruals API
  slug: wisdomtree-accruals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-accruals-api-openapi.yml
- filename: wisdomtree-dividend-payment-preferences-api-openapi.yml
  format: yaml
  label: WisdomTree Dividend Payment Preferences API
  slug: wisdomtree-dividend-payment-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-dividend-payment-preferences-api-openapi.yml
- filename: wisdomtree-fund-data-api-openapi.yml
  format: yaml
  label: WisdomTree Fund Data API
  slug: wisdomtree-fund-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-fund-data-api-openapi.yml
- filename: wisdomtree-orders-api-openapi.yml
  format: yaml
  label: WisdomTree Orders API
  slug: wisdomtree-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-orders-api-openapi.yml
- filename: wisdomtree-organizations-api-openapi.yml
  format: yaml
  label: WisdomTree Organizations API
  slug: wisdomtree-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-organizations-api-openapi.yml
- filename: wisdomtree-statements-api-openapi.yml
  format: yaml
  label: WisdomTree Statements API
  slug: wisdomtree-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-statements-api-openapi.yml
- filename: wisdomtree-users-api-openapi.yml
  format: yaml
  label: WisdomTree Users API
  slug: wisdomtree-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-users-api-openapi.yml
- filename: wisdomtree-wallets-api-openapi.yml
  format: yaml
  label: WisdomTree Wallets API
  slug: wisdomtree-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/openapi/wisdomtree-wallets-api-openapi.yml
consequence_counts:
  physical: 4
  read: 26
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wisdomtree Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/dividend-payment-preferences/{dpp_guid}/edit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/review
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/{order_reference}/notes
operation_count: 35
overview: 'WisdomTree exposes 35 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 5 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WisdomTree
provider_slug: wisdomtree
slug: wisdomtree-agentic-access
source_filename: wisdomtree-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/wisdomtree-connect-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 26\n    acting: 9\n  by_consequence:\n    read: 26\n    physical: 4\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/accruals/\n  method: get\n  operationId: Retrieves Open Accruals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dividend-payment-preferences/\n  method: get\n  operationId: Retrieves All Dividend Payment Preferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dividend-payment-preferences/{dpp_guid}\n  method: get\n  operationId: Retrieve Dividend Payment Preference Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dividend-payment-preferences/{dpp_guid}/edit\n  method: post\n  operationId: Update Dividend Payment Preferences\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dividend-payment-preferences/export\n  method: get\n  operationId: Download Dividend Payment Preferences Workbook\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/\n  method: post\n  operationId: Create Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_reference}\n  method: get\n  operationId: Retrieves Order Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_reference}/fetch-hash\n  method: post\n  operationId: Fetch Missing Order Hashes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_reference}/notes\n  method: post\n  operationId: Create Order Note\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_reference}/status\n  method: get\n  operationId: Retrieves Order Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/all\n  method: get\n  operationId: Retrieves All Orders for Org\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/deposit_address\n  method: get\n  operationId: Retrieves WisdomTree Deposit Address\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/details/batch\n  method: get\n  operationId: Retrieve Multiple Order Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/export\n  method: get\n  operationId: Download Orders Workbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/hash/{hash}\n  method: get\n  operationId: Retrieve Order Details by Hash\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/latest\n  method: get\n  operationId: Retrieves Latest Accessible Orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/on-receipt-wallet/\n  method: get\n  operationId: Retrieves wallet address for on receipt order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/order-mapping\n  method: get\n  operationId: Retrieve Order Mapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/portfolio\n  method:\
  \ get\n  operationId: Retrieve Connect Portfolio Page\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/portfolio/download\n  method: get\n  operationId: Download Connect Portfolio Workbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/products\n  method: get\n  operationId: Retrieve User Initiated Order Products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/review\n  method: post\n  operationId: Review Order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_guid}/wallets\n  method: get\n  operationId: Retrieves organization wallet details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_guid}/wallets\n  method: post\n  operationId: Creates Wallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_guid}/wallets/{wallet_guid}\n  method: patch\n  operationId:\
  \ Approves Wallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/me\n  method: get\n  operationId: Retrieves current user's organization details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/me/wallets\n  method: get\n  operationId: Retrieves current user's organization wallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/me/wallets/{wallet_guid}/details\n  method: get\n  operationId: Retrieves current user's\
  \ organization wallet edit details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/me/wallets/{wallet_guid}/details\n  method: patch\n  operationId: Updates current user's organization wallet nickname\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/me/wallets/chains\n  method: get\n  operationId: Retrieves current user's organization wallet chains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/statements/{statement_id}/download\n\
  \  method: get\n  operationId: Download Statement File\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/statements/list\n  method: get\n  operationId: Retrieve Statements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/me/api-keys\n  method: get\n  operationId: List Current User API Keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/me/api-keys\n  method: post\n  operationId: Create Current User API Key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/me/api-keys/{application_id}\n  method: delete\n  operationId: Delete Current User API Key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisdomtree/refs/heads/main/agentic-access/wisdomtree-agentic-access.yml
summary_line: 35 operations · 9 acting
tags:
- Company
- Asset Management
- ETFs
- Tokenization
- Tokenized Funds
- Financial Services
- Fund Data
---
