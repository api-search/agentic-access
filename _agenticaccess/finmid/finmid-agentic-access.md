---
acting_count: 43
action_class_counts:
  acting: 43
  connected: 22
api_specs:
- filename: finmid-beta-endpoints-api-openapi.yml
  format: yaml
  label: Finmid Beta Endpoints API
  slug: finmid-beta-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-beta-endpoints-api-openapi.yml
- filename: finmid-business-api-openapi.yml
  format: yaml
  label: Finmid Business API
  slug: finmid-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-business-api-openapi.yml
- filename: finmid-buyer-api-openapi.yml
  format: yaml
  label: Finmid Buyer API
  slug: finmid-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-buyer-api-openapi.yml
- filename: finmid-capital-max-api-openapi.yml
  format: yaml
  label: Finmid Capital Max API
  slug: finmid-capital-max-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-capital-max-api-openapi.yml
- filename: finmid-csp-financial-document-api-openapi.yml
  format: yaml
  label: Finmid CSP Financial Document API
  slug: finmid-csp-financial-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-csp-financial-document-api-openapi.yml
- filename: finmid-document-api-openapi.yml
  format: yaml
  label: Finmid Document API
  slug: finmid-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-document-api-openapi.yml
- filename: finmid-funding-api-openapi.yml
  format: yaml
  label: Finmid Funding API
  slug: finmid-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-funding-api-openapi.yml
- filename: finmid-funding-application-api-openapi.yml
  format: yaml
  label: Finmid Funding Application API
  slug: finmid-funding-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-funding-application-api-openapi.yml
- filename: finmid-incoming-webhook-api-openapi.yml
  format: yaml
  label: Finmid Incoming Webhook API
  slug: finmid-incoming-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-incoming-webhook-api-openapi.yml
- filename: finmid-offer-api-openapi.yml
  format: yaml
  label: Finmid Offer API
  slug: finmid-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-offer-api-openapi.yml
- filename: finmid-offer-group-api-openapi.yml
  format: yaml
  label: Finmid Offer Group API
  slug: finmid-offer-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-offer-group-api-openapi.yml
- filename: finmid-onboarding-api-openapi.yml
  format: yaml
  label: Finmid Onboarding API
  slug: finmid-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-onboarding-api-openapi.yml
- filename: finmid-payment-api-openapi.yml
  format: yaml
  label: Finmid Payment API
  slug: finmid-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-payment-api-openapi.yml
- filename: finmid-payment-request-api-openapi.yml
  format: yaml
  label: Finmid Payment Request API
  slug: finmid-payment-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-payment-request-api-openapi.yml
- filename: finmid-sales-statements-api-openapi.yml
  format: yaml
  label: Finmid Sales statements API
  slug: finmid-sales-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-sales-statements-api-openapi.yml
- filename: finmid-seller-api-openapi.yml
  format: yaml
  label: Finmid Seller API
  slug: finmid-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-seller-api-openapi.yml
- filename: finmid-simulation-api-openapi.yml
  format: yaml
  label: Finmid Simulation API
  slug: finmid-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-simulation-api-openapi.yml
- filename: finmid-tasks-api-openapi.yml
  format: yaml
  label: Finmid Tasks API
  slug: finmid-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-tasks-api-openapi.yml
consequence_counts:
  physical: 22
  read: 22
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Finmid Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/capital/payment-batches/{batch_id}/incoming-funds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/capital/payment-batches/{batch_id}/payments/{payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/capital/payments/webhooks/payout/outcome
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/capital/simulation/batches/{batch_id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/capital/simulation/credits/{credit_id}/payout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/capital/simulation/payments/{payment_id}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/capital/simulation/payments/{payment_id}/fail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/capital/simulation/payments/{payment_id}/schedule
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transaction
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/b2b-payments/buyers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/b2b-payments/buyers/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/b2b-payments/payment-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/b2b-payments/payment-requests/documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v2/b2b-payments/payment-requests/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/b2b-payments/payment-requests/{id}/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/b2b-payments/payment-requests/{id}/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/b2b-payments/sellers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/b2b-payments/sellers/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/b2b-payments/sellers/{id}/bank-details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/b2b-payments/simulation/buyer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/b2b-payments/simulation/payment-requests/repayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v2/b2b-payments/simulation/seller
operation_count: 65
overview: 'Finmid exposes 65 API operations that an AI agent could call, of which 43 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 21 write, and 22 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Finmid
provider_slug: finmid
slug: finmid-agentic-access
source_filename: finmid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/finmid-b2b-payments-api-openapi.yml, openapi/finmid-capital-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    acting: 43\n    connected: 22\n  by_consequence:\n    physical: 22\n    read: 22\n    write: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/b2b-payments/buyers\n  method: post\n  operationId: create-buyer-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v2/b2b-payments/buyers/list\n  method: get\n  operationId: get-buyers-for-platform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/b2b-payments/buyers/{id}\n  method: get\n  operationId: get-buyer-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/b2b-payments/buyers/{id}\n  method: patch\n  operationId: update-buyer-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/buyers/{id}/payment-limit\n  method: get\n  operationId:\
  \ get-buyer-limit-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/b2b-payments/payment-requests\n  method: post\n  operationId: create-payment-request-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/payment-requests/documents\n  method: post\n  operationId: upload-payment-request-documents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/payment-requests/list\n  method: get\n  operationId: get-payment-requests-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/b2b-payments/payment-requests/{id}\n  method: get\n  operationId: get-payment-request-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/b2b-payments/payment-requests/{id}/cancel\n  method: put\n  operationId: cancel-payment-request-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v2/b2b-payments/payment-requests/{id}/payouts\n  method: post\n  operationId: create-payment-request-payout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/payment-requests/{id}/update\n  method: patch\n  operationId: update-payment-request-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/reports/settlement\n  method: get\n  operationId: get-settlement-report\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/b2b-payments/sellers\n  method: post\n  operationId: create-seller-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/sellers/list\n  method: get\n  operationId: get-sellers-for-platform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/b2b-payments/sellers/{id}\n  method: get\n  operationId: get-seller-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v2/b2b-payments/sellers/{id}\n  method: patch\n  operationId: update-seller-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/sellers/{id}/bank-details\n  method: patch\n  operationId: update-seller-bank-account-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/simulation/buyer\n  method: patch\n  operationId: simulate-buyer-v2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/simulation/payment-requests/repayment\n  method: post\n  operationId: simulate-payment-request-repayment-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/simulation/seller\n  method: patch\n  operationId: simulate-seller-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/b2b-payments/tasks\n  method: get\n  operationId: get-tasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/businesses\n  method: post\n  operationId: create-business\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/businesses/{business_id}\n  method: get\n  operationId: get-business\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/businesses/{business_id}/capital-max\n  method: get\n  operationId: get-capital-max\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/businesses/{business_id}/credits\n  method: get\n  operationId: get-fundings-for-business\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/businesses/{business_id}/documents/csp\n  method: get\n  operationId: list-csp-documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/businesses/{business_id}/documents/csp/submit\n  method: post\n  operationId: finalize-csp-document-submission\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/businesses/{business_id}/documents/csp/uploads\n  method: post\n  operationId: create-csp-document-upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/businesses/{business_id}/documents/csp/{document_id}\n  method: delete\n  operationId: delete-csp-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/businesses/{business_id}/fundings/applications\n  method: get\n  operationId: get-funding-applications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/businesses/{business_id}/kyb-data\n  method: post\n  operationId: add-business-kyb-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/businesses/{business_id}/kyb-document-uploads\n  method: post\n  operationId: create-kyb-business-document-upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/businesses/{business_id}/non-pi\n  method: put\n  operationId: update-business-non-pi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/businesses/{business_id}/offers/current\n  method: get\n  operationId: get-current-offer-state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/businesses/{business_id}/offers/{offer_group_id}/platform-checks\n  method: post\n  operationId: report-platform-check\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/businesses/{business_id}/offers/{offer_group_id}/signature-link\n  method: post\n  operationId: create-signature-link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/businesses/{business_id}/onboardings/latest\n  method: get\n  operationId: get-latest-onboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/businesses/{business_id}/performance-data\n  method: post\n  operationId:\
  \ submit-business-performance-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/credits/{credit_id}/documents\n  method: get\n  operationId: list-funding-documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/credits/{credit_id}/payments\n  method: get\n  operationId: get-payments-for-credit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/documents/{document_id}/url\n  method: get\n  operationId: get-document-url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/incoming-webhooks\n  method: post\n  operationId: receive-incoming-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/payment-batches/{batch_id}\n  method: get\n  operationId: get-payment-batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/payment-batches/{batch_id}/incoming-funds\n  method: post\n  operationId: report-funds-collection\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/payment-batches/{batch_id}/payments/{payment_id}\n  method: post\n  operationId: report-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/payments/webhooks/payout/outcome\n  method: post\n  operationId: receive-payout-outcome\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /api/v1/capital/sales-statements/batches/{id}\n  method: get\n  operationId: get-sales-statements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capital/sales-statements/batches/{id}\n  method: post\n  operationId: add-sales-statements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/batches/{batch_id}/payments\n  method: post\n  operationId: simulate-batch-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/businesses/{business_id}/accept-offers\n  method: post\n  operationId: simulate-accept-offers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/businesses/{business_id}/capital-max-review\n  method: post\n  operationId: simulate-capital-max-review\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/businesses/{business_id}/create-offers\n\
  \  method: post\n  operationId: simulate-create-offers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/businesses/{business_id}/expire-offers\n  method: post\n  operationId: simulate-expire-offers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/credits\n  method: post\n  operationId: simulate-create-funding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/credits/{credit_id}/payout\n  method: post\n  operationId: payout-credit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/credits/{credit_id}/reject\n  method: post\n  operationId: reject-credit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/fundings/applications/{application_id}/accept\n\
  \  method: post\n  operationId: accept-funding-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/fundings/applications/{application_id}/cancel\n  method: post\n  operationId: cancel-funding-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/fundings/applications/{application_id}/reject\n  method: post\n  operationId: reject-funding-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/payments/{payment_id}/complete\n  method: post\n  operationId: complete-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/payments/{payment_id}/fail\n  method: post\n  operationId: fail-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/capital/simulation/payments/{payment_id}/schedule\n  method: post\n  operationId: schedule-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transaction\n  method: post\n  operationId: execute-payment-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/capital/businesses/{business_id}/offers/active\n  method:\
  \ get\n  operationId: get-active-offer-group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/agentic-access/finmid-agentic-access.yml
summary_line: 65 operations · 43 acting
tags:
- Company
- Embedded Finance
- Embedded Lending
- B2B Payments
- Fintech
- Lending
- Capital
- Financing
- Payments
- Marketplace
---
