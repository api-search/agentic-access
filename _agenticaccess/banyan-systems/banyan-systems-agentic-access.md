---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 23
api_specs:
- filename: banyan-systems-authentication-api-openapi.yml
  format: yaml
  label: Banyan Systems Authentication API
  slug: banyan-systems-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-authentication-api-openapi.yml
- filename: banyan-systems-card-linked-offer-api-openapi.yml
  format: yaml
  label: Banyan Systems Card Linked Offer API
  slug: banyan-systems-card-linked-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-card-linked-offer-api-openapi.yml
- filename: banyan-systems-consent-api-openapi.yml
  format: yaml
  label: Banyan Systems Consent API
  slug: banyan-systems-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-consent-api-openapi.yml
- filename: banyan-systems-enriched-data-api-openapi.yml
  format: yaml
  label: Banyan Systems Enriched Data API
  slug: banyan-systems-enriched-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-enriched-data-api-openapi.yml
- filename: banyan-systems-enriched-data-merchant-service-provider-api-openapi.yml
  format: yaml
  label: Banyan Systems Enriched Data - Merchant Service Provider API
  slug: banyan-systems-enriched-data-merchant-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-enriched-data-merchant-service-provider-api-openapi.yml
- filename: banyan-systems-history-api-openapi.yml
  format: yaml
  label: Banyan Systems History API
  slug: banyan-systems-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-history-api-openapi.yml
- filename: banyan-systems-receipt-api-openapi.yml
  format: yaml
  label: Banyan Systems Receipt API
  slug: banyan-systems-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-receipt-api-openapi.yml
- filename: banyan-systems-tag-counter-api-openapi.yml
  format: yaml
  label: Banyan Systems Tag Counter API
  slug: banyan-systems-tag-counter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-tag-counter-api-openapi.yml
- filename: banyan-systems-transaction-api-openapi.yml
  format: yaml
  label: Banyan Systems Transaction API
  slug: banyan-systems-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-transaction-api-openapi.yml
- filename: banyan-systems-webhook-api-openapi.yml
  format: yaml
  label: Banyan Systems Webhook API
  slug: banyan-systems-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-webhook-api-openapi.yml
consequence_counts:
  read: 23
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Banyan Systems Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'Banyan Systems exposes 40 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Banyan Systems
provider_slug: banyan-systems
slug: banyan-systems-agentic-access
source_filename: banyan-systems-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/banyan-systems-rest-api-openapi.yml, openapi/banyan-systems-sensitive-data-vault-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    acting: 17\n    connected: 23\n  by_consequence:\n    write: 17\n    read: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: oauth-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaign\n  method: get\n  operationId: retrieve-all-campaigns\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaign\n  method: post\n  operationId: submit-a-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaign/{id}\n  method: get\n  operationId: retrieve-a-campaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaign/{id}\n  method: patch\n  operationId: update-a-campaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaign/{id}/offers\n  method: get\n  operationId: retrieve-all-offers-under-a-campaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/history\n  method: post\n  operationId: retrieve-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offer\n  method: get\n  operationId: search-offer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offer\n  method: post\n  operationId: submit-an-offer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offer/activation\n  method: post\n  operationId: submit-an-offer-activation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offer/activation/search\n  method: get\n  operationId: search-offer-activations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offer/activation/{id}\n  method: get\n  operationId: retrieve-an-offer-activation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offer/activation/{id}\n  method: patch\n  operationId:\
  \ update-an-offer-activation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offer/{id}\n  method: get\n  operationId: retrieve-an-offer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offer/{id}\n  method: patch\n  operationId: update-an-offer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offer/{id}/activations\n  method: get\n  operationId: retrieve-offer-activations-for-offer-id\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receipt\n  method: post\n  operationId: submit-hotel-receipts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/receipt/retail\n  method: post\n  operationId: submit-retail-receipts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/receipt/search\n  method: post\n  operationId: receipt-search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receipt/{byn_receipt_id}\n  method: get\n  operationId: retrieve-a-receipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tagcounter/query\n  method: post\n  operationId: execute-tag-counter-query\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transaction\n  method: post\n  operationId: submit-one-or-more-transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/transaction/{byn_transaction_id}\n  method: get\n  operationId: fetch-a-transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transaction/{byn_transaction_id}/enriched\n  method: get\n  operationId: retrieve-match\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transaction/{byn_transaction_id}/enriched-merchant\n  method: get\n  operationId: retrieve-match-merchant-service-provider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transaction/{byn_transaction_id}/redemption\n  method: get\n  operationId: retrieve-offer-redemption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/transaction/{byn_transaction_id}/redemption/history\n  method: get\n  operationId: retrieve-offer-redemption-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/version\n  method: get\n  operationId: version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook\n  method: post\n  operationId: create-webhook-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/endpoint\n  method: get\n  operationId: get-webhook-endpoints-all\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/endpoint\n  method: post\n  operationId: create-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/endpoint/{endpoint_id}\n  method: delete\n  operationId: delete-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/endpoint/{endpoint_id}\n  method: get\n  operationId: retrieve-webhook-endpoint\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/endpoint/{endpoint_id}\n  method: put\n  operationId: update-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/events\n  method: get\n  operationId: get-webhook-event-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/{application_id}\n  method: delete\n  operationId: delete-webhook-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/{application_id}\n  method: get\n  operationId: retrieve-webhook-application\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/consent/\n  method: post\n  operationId: create-consent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/consent/search\n  method: post\n  operationId: search-consent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/consent/{byn_consent_id}\n  method: get\n  operationId: get-consent\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/agentic-access/banyan-systems-agentic-access.yml
summary_line: 40 operations · 17 acting
tags:
- Company
- Receipt Data
- Transaction Enrichment
- Item-Level Data
- Card-Linked Offers
- Fintech
- Payments
- Data Collaboration
- Webhook
- Data Enrichment
---
