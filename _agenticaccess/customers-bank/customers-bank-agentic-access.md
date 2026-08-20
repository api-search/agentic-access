---
acting_count: 84
action_class_counts:
  acting: 84
  connected: 127
api_specs:
- filename: customers-bank-accounts-openapi.json
  format: json
  label: Customers Bank Accounts API
  slug: customers-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-accounts-openapi.json
- filename: customers-bank-ach-openapi.json
  format: json
  label: Customers Bank ACH API
  slug: customers-bank-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-ach-openapi.json
- filename: customers-bank-consumerlending-openapi.json
  format: json
  label: Customers Bank Consumer Lending API
  slug: customers-bank-consumer-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-consumerlending-openapi.json
- filename: customers-bank-instantpayments-openapi.json
  format: json
  label: Customers Bank Instant Payments API
  slug: customers-bank-instant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-instantpayments-openapi.json
- filename: customers-bank-itoperations-openapi.json
  format: json
  label: Customers Bank IT Operations API
  slug: customers-bank-it-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-itoperations-openapi.json
- filename: customers-bank-partners-openapi.json
  format: json
  label: Customers Bank Partners API
  slug: customers-bank-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-partners-openapi.json
- filename: customers-bank-security-openapi.json
  format: json
  label: Customers Bank Security API
  slug: customers-bank-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-security-openapi.json
- filename: customers-bank-transfers-openapi.json
  format: json
  label: Customers Bank Transfers API
  slug: customers-bank-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-transfers-openapi.json
- filename: customers-bank-webhooks-openapi.json
  format: json
  label: Customers Bank Webhooks API
  slug: customers-bank-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-webhooks-openapi.json
- filename: customers-bank-wires-openapi.json
  format: json
  label: Customers Bank Wires API
  slug: customers-bank-wires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-wires-openapi.json
consequence_counts:
  physical: 21
  read: 127
  safety-critical: 4
  write: 59
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Customers Bank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /ControlType/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /ControlType/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /ControlType/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /notification-email/send-code
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/bulk-approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/bulk-decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/fednow
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/fednow/{id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/fednow/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/fednow/{id}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/rtp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/rtp/{id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/rtp/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/rtp/{id}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/{id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /outgoing/{id}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{accountId}/InterestPayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{id}/decline
operation_count: 211
overview: 'Customers Bank exposes 211 API operations that an AI agent could call, of which 84 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 127 read, 59 write, 21 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Customers Bank
provider_slug: customers-bank
slug: customers-bank-agentic-access
source_filename: customers-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/customers-bank-accounts-openapi.json, openapi/customers-bank-ach-openapi.json,\n  openapi/customers-bank-consumerlending-openapi.json, openapi/customers-bank-instantpayments-openapi.json,\n  openapi/customers-bank-itoperations-openapi.json, openapi/customers-bank-partners-openapi.json,\n  openapi/customers-bank-security-openapi.json, openapi/customers-bank-transfers-openapi.json,\n  openapi/customers-bank-webhooks-openapi.json, openapi/customers-bank-wires-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 211\n  by_action_class:\n    acting: 84\n    connected: 127\n  by_consequence:\n    write: 59\n    read: 127\n    physical: 21\n    safety-critical: 4\n  human_in_the_loop_required:\
  \ 4\noperations:\n- path: /{accountId}\n  method: put\n  operationId: put-accountid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{accountId}\n  method: get\n  operationId: get-accountid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{accountId}/transactions\n  method: get\n  operationId: get-accountid-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /download\n  method: get\n  operationId: get-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{accountId}/InterestPayments\n  method: post\n  operationId: post-accountid-interestpayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{accountId}/InterestPayments\n  method: get\n  operationId: get-accountid-interestpayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{accountId}/InterestPayments/{interestPaymentId}\n  method: get\n  operationId: get-accountid-interestpayments-interestpaymentid\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{accountId}/searchable\n  method: put\n  operationId: put-accountid-searchable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Customers\n  method: get\n  operationId: get-customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Customers\n  method: post\n  operationId: post-customers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /Subaccounts\n  method: get\n  operationId: get-subaccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Subaccounts\n  method: post\n  operationId: post-subaccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Customers/{id}\n  method: get\n  operationId: get-customers-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Customers/{id}\n  method: put\n  operationId: put-customers-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Customers/{id}\n  method: delete\n  operationId: delete-customers-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference-data\n  method: get\n  operationId: get-reference-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Subaccounts/{id}\n  method: get\n  operationId: get-subaccounts-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Subaccounts/{id}\n\
  \  method: put\n  operationId: put-subaccounts-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Subaccounts/{id}\n  method: delete\n  operationId: delete-subaccounts-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Subaccounts/{id}/freeze\n  method: post\n  operationId: post-subaccounts-id-freeze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /Subaccounts/{id}/unfreeze\n  method: post\n  operationId: post-subaccounts-id-unfreeze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Subaccounts/{id}/tags/{tagId}\n  method: post\n  operationId: post-subaccounts-id-tags-tagid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Subaccounts/{id}/tags/{tagId}\n  method: delete\n  operationId: delete-subaccounts-id-tags-tagid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Tags\n  method: get\n  operationId: get-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Tags\n  method: post\n  operationId: post-tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Tags/{id}\n  method: get\n  operationId: get-tags-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Tags/{id}\n  method: put\n  operationId: put-tags-id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Tags/{id}\n  method: delete\n  operationId: delete-tags-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /programs/{id}\n  method: get\n  operationId: get-programs-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs\n  method: get\n  operationId: get-programs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /programs/download\n  method: get\n  operationId: get-programs-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/{id}\n  method: get\n  operationId: get-outgoing-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing\n  method: get\n  operationId: get-outgoing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/download\n  method: get\n  operationId: get-outgoing-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/credit\n  method: post\n  operationId: post-outgoing-credit\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing/debit\n  method: post\n  operationId: post-outgoing-debit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing/{id}/reverse\n  method: post\n  operationId: post-outgoing-id-reverse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /outgoing/{id}/cancel\n  method: post\n  operationId: post-outgoing-id-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incoming/{id}\n  method: get\n  operationId: get-incoming-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incoming\n  method: get\n  operationId: get-incoming\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incoming/download\n  method: get\n  operationId: get-incoming-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /ControlType\n  method: get\n  operationId: get-controltype\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ControlType/{id}\n  method: get\n  operationId: get-controltype-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ControlType/{id}\n  method: put\n  operationId: put-controltype-id\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /outgoing/{id}/approve\n  method: post\n  operationId: post-outgoing-id-approve\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing/{id}/decline\n  method: post\n  operationId: post-outgoing-id-decline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reference-data\n  method: get\n  operationId: get-reference-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountAccess/{id}\n  method: get\n  operationId: get-accountaccess-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /application\n  method: post\n  operationId: post-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /application\n  method: get\n  operationId: get-application\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /application/{id}\n  method: get\n  operationId: get-application-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /program/{id}\n  method: get\n  operationId: get-program-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /program\n  method: get\n  operationId: get-program\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loan/{id}\n  method: get\n  operationId: get-loan-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loan/{id}/funding\n  method: post\n  operationId: post-loan-id-funding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loan/{id}/funding\n  method: get\n  operationId: get-loan-id-funding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /loan/{id}/funding/{fundingInstructionId}\n  method: get\n  operationId: get-loan-id-funding-fundinginstructionid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loan\n  method: get\n  operationId: get-loan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loan/{id}/complete\n  method: post\n  operationId: post-loan-id-complete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loan/{id}/cancel\n  method: post\n  operationId: post-loan-id-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incoming/{id}\n  method: get\n  operationId: get-incoming-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incoming/fednow/{id}\n  method: get\n  operationId: get-incoming-fednow-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incoming/rtp/{id}\n  method: get\n  operationId: get-incoming-rtp-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incoming\n  method: get\n  operationId: get-incoming\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incoming/rtp\n  method: get\n  operationId: get-incoming-rtp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incoming/fednow\n  method: get\n  operationId: get-incoming-fednow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing\n  method: post\n  operationId: post-outgoing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing\n  method: get\n  operationId: get-outgoing\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/rtp\n  method: post\n  operationId: post-outgoing-rtp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing/rtp\n  method: get\n  operationId: get-outgoing-rtp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/fednow\n  method: post\n  operationId: post-outgoing-fednow\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n \
  \     purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing/fednow\n  method: get\n  operationId: get-outgoing-fednow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/{id}\n  method: get\n  operationId: get-outgoing-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/{id}/cancel\n  method: post\n  operationId: post-outgoing-id-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /outgoing/rtp/{id}\n  method: get\n  operationId: get-outgoing-rtp-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/rtp/{id}/cancel\n  method: post\n  operationId: post-outgoing-rtp-id-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing/fednow/{id}\n  method: get\n  operationId: get-outgoing-fednow-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/fednow/{id}/cancel\n  method: post\n  operationId: post-outgoing-fednow-id-cancel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ControlType\n  method: get\n  operationId: get-controltype\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ControlType/{id}\n  method: get\n  operationId: get-controltype-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ControlType/{id}\n  method: put\n  operationId: put-controltype-id\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /incoming/fednow/download\n  method: get\n  operationId: get-incoming-fednow-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incoming/rtp/download\n  method: get\n  operationId: get-incoming-rtp-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/rtp/download\n  method: get\n  operationId: get-outgoing-rtp-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/fednow/download\n  method: get\n  operationId: get-outgoing-fednow-download\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outgoing/rtp/{id}/approve\n  method: post\n  operationId: post-outgoing-rtp-id-approve\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing/fednow/{id}/approve\n  method: post\n  operationId: post-outgoing-fednow-id-approve\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing/rtp/{id}/decline\n\
  \  method: post\n  operationId: post-outgoing-rtp-id-decline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outgoing/fednow/{id}/decline\n  method: post\n  operationId: post-outgoing-fednow-id-decline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accountaccess/fednow/{accountId}\n  method: get\n  operationId: get-accountaccess-fednow-accountid\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountaccess/rtp/{accountId}\n  method: get\n  operationId: get-accountaccess-rtp-accountid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Banks\n  method: get\n  operationId: get-banks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Banks/{id}\n  method: get\n  operationId: get-banks-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Banks/aba/{abaNumber}\n  method: get\n  operationId: get-banks-aba-abanumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Banks/bic/{bic}\n\
  \  method: get\n  operationId: get-banks-bic-bic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CorrespondentInstructions\n  method: get\n  operationId: get-correspondentinstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Banks/aba\n  method: get\n  operationId: get-banks-aba\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Banks/bic\n  method: get\n  operationId: get-banks-bic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CorrespondentInstructions/download\n  method: get\n  operationId: get-correspondentinstructions-download-rail-rail\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /WebPubSub/client-access-uri\n  method: get\n  operationId: get-webpubsub-client-access-uri\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apiAccess\n  method: get\n  operationId: get-apiaccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Messages\n  method: get\n  operationId: get-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials\n\
  \  method: get\n  operationId: get-credentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials\n  method: post\n  operationId: post-credentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credentials/{id}\n  method: delete\n  operationId: delete-credentials-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Users\n  method: post\n  operationId: post-users\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Users\n  method: get\n  operationId: get-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users\n  method: put\n  operationId: put-users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Users/{userId}\n  method: delete\n  operationId: delete-users-userid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me\n  method: get\n  operationId: get-users-me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Messages/download\n  method: get\n  operationId: get-messages-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users/download\n  method: get\n  operationId: get-users-download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users/{id}\n  method: get\n  operationId: get-users-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /users/me/logout\n  method: post\n  operationId: post-users-me-logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Users/email\n  method: get\n  operationId: get-users-email\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-settings/{settingName}\n  method: get\n  operationId: get-user-settings-settingname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-settings/{settingName}\n  method: put\n  operationId: put-user-settings-settingname\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \n\n# --- truncated at 32 KB (57 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/agentic-access/customers-bank-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/agentic-access/customers-bank-agentic-access.yml
summary_line: 211 operations · 84 acting · 4 human-in-the-loop
tags:
- Financial-Services
- Banking
- United States
- Banking as a Service
- Embedded Finance
- Payments
- Commercial Banking
---
