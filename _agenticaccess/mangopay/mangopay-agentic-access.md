---
acting_count: 116
action_class_counts:
  acting: 116
  connected: 99
api_specs:
- filename: openapi.json
  format: json
  label: Mangopay REST API
  slug: mangopay-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mangopay/refs/heads/main/openapi/openapi.json
consequence_counts:
  physical: 49
  read: 99
  write: 67
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mangopay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /bankingaliases/{bankingaliasid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cardregistrations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /cardregistrations/{cardregistrationid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /cards/{cardchallengeflowid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cards/{cardchallengeflowid}/validation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deposit-preauthorizations/card/direct
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /deposit-preauthorizations/{depositid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mandates/directdebit/web
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /mandates/{mandateId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/bankwire/direct
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/card/direct
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/card/web
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/deposit-preauthorized/direct/full-capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/directdebit/direct
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/bancontact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/bizum
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/blik
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/ideal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/klarna
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/mbway
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/multibanco
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/openbanking
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/payconiq
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/paypal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payins/payment-methods/paypal/data-collection
operation_count: 215
overview: 'Mangopay exposes 215 API operations that an AI agent could call, of which 116 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 99 read, 67 write, and 49 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mangopay
provider_slug: mangopay
slug: mangopay-agentic-access
source_filename: mangopay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 215\n  by_action_class:\n    acting: 116\n    connected: 99\n  by_consequence:\n    write: 67\n    read: 99\n    physical: 49\n  human_in_the_loop_required: 0\noperations:\n- path: /sca/users/natural\n  method: post\n  operationId: post_sca_users_natural\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sca/users/natural/{userId}/category\n  method: put\n  operationId: put_sca_users_natural_userId_category\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sca/users/natural/{userId}\n  method: put\n  operationId: put_sca_users_natural_userId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sca/users/legal\n  method: post\n  operationId: post_sca_users_legal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /sca/users/legal/{userId}/category\n  method: put\n  operationId: put_sca_users_legal_userId_category\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sca/users/legal/{userId}\n  method: put\n  operationId: put_sca_users_legal_userId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sca/users/{userId}/enrollment\n  method: post\n  operationId: post_sca_users_userId_enrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sca/users/{userId}/consent\n  method: post\n  operationId: post_sca_users_userId_consent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sca/users/{userId}/sca-status\n  method: get\n  operationId: get_sca_users_userId_sca_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sca/users/{userId}\n  method: get\n  operationId: get_sca_users_userId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/natural\n\
  \  method: post\n  operationId: post_users_natural\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/natural/{userId}\n  method: put\n  operationId: put_users_natural_userId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/natural/{userId}\n  method: delete\n  operationId: delete_users_natural_userId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /users/legal\n  method: post\n  operationId: post_users_legal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/legal/{userId}\n  method: put\n  operationId: put_users_legal_userId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/legal/{userId}\n  method: delete\n  operationId: delete_users_legal_userId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}\n  method: get\n  operationId: get_users_userId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: get_users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets\n  method: post\n  operationId: post_wallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets/{walletId}\n  method: put\n  operationId: put_wallets_walletId\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets/{walletId}\n  method: get\n  operationId: get_wallets_walletId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{usernaturalpayerwalletid}\n  method: put\n  operationId: put_wallets_usernaturalpayerwalletid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets/{usernaturalpayerwalletid}\n  method: get\n  operationId: get_wallets_usernaturalpayerwalletid\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{usernaturalownerwalletid}\n  method: put\n  operationId: put_wallets_usernaturalownerwalletid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets/{usernaturalownerwalletid}\n  method: get\n  operationId: get_wallets_usernaturalownerwalletid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{userlegalownerwalletid}\n  method: put\n  operationId: put_wallets_userlegalownerwalletid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets/{userlegalownerwalletid}\n  method: get\n  operationId: get_wallets_userlegalownerwalletid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/wallets\n  method: get\n  operationId: get_users_userId_wallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{usernaturalpayerwalletid}/transactions\n  method: get\n  operationId: get_wallets_usernaturalpayerwalletid_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{usernaturalownerwalletid}/transactions\n  method:\
  \ get\n  operationId: get_wallets_usernaturalownerwalletid_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{userlegalownerwalletid}/transactions\n  method: get\n  operationId: get_wallets_userlegalownerwalletid_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardregistrations\n  method: post\n  operationId: post_cardregistrations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '{cardregistrationurl}'\n  method: post\n  operationId: post_cardregistrationurl\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardregistrations/{cardregistrationid}\n  method: put\n  operationId: put_cardregistrations_cardregistrationid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardregistrations/{cardregistrationid}\n  method: get\n  operationId: get_cardregistrations_cardregistrationid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardchallengeflowid}\n  method: put\n  operationId: put_cards_cardchallengeflowid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardchallengeflowid}\n  method: get\n  operationId: get_cards_cardchallengeflowid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/cards\n  method: get\n  operationId: get_users_userId_cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/fingerprints/{cardfingerprint}\n\
  \  method: get\n  operationId: get_cards_fingerprints_cardfingerprint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/fingerprints/{cardfingerprint}/transactions\n  method: get\n  operationId: get_cards_fingerprints_cardfingerprint_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardchallengeflowid}/validation\n  method: post\n  operationId: post_cards_cardchallengeflowid_validation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cards/{cardchallengeflowid}/validation/{cardvalidationid}\n\
  \  method: get\n  operationId: get_cards_cardchallengeflowid_validation_cardvalidationid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payins/card/direct\n  method: post\n  operationId: post_payins_card_direct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/{payinId}\n  method: get\n  operationId: get_payins_payinId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurringpayinregistrations\n  method: post\n  operationId: post_recurringpayinregistrations\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurringpayinregistrations/{recurringpayinregistrationid}\n  method: put\n  operationId: put_recurringpayinregistrations_recurringpayinregistrationid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurringpayinregistrations/{recurringpayinregistrationid}\n  method: get\n  operationId: get_recurringpayinregistrations_recurringpayinregistrationid\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payins/recurring/card/direct\n  method: post\n  operationId: post_payins_recurring_card_direct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /preauthorizations/card/direct\n  method: post\n  operationId: post_preauthorizations_card_direct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /preauthorizations/{preauthorizationid}\n\
  \  method: put\n  operationId: put_preauthorizations_preauthorizationid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /preauthorizations/{preauthorizationid}\n  method: get\n  operationId: get_preauthorizations_preauthorizationid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardchallengeflowid}/preauthorizations\n  method: get\n  operationId: get_cards_cardchallengeflowid_preauthorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/preauthorizations\n  method:\
  \ get\n  operationId: get_users_userId_preauthorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payins/preauthorized/direct\n  method: post\n  operationId: post_payins_preauthorized_direct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deposit-preauthorizations/card/direct\n  method: post\n  operationId: post_deposit_preauthorizations_card_direct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deposit-preauthorizations/{depositid}\n  method: put\n  operationId: put_deposit_preauthorizations_depositid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deposit-preauthorizations/{depositid}\n  method: get\n  operationId: get_deposit_preauthorizations_depositid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{cardchallengeflowid}/deposit-preauthorizations\n  method: get\n  operationId: get_cards_cardchallengeflowid_deposit_preauthorizations\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/deposit-preauthorizations\n  method: get\n  operationId: get_users_userId_deposit_preauthorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payins/deposit-preauthorized/direct/full-capture\n  method: post\n  operationId: post_payins_deposit_preauthorized_direct_full_capture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/card/web\n  method: post\n  operationId: post_payins_card_web\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/card/web/{webpayinid}/extended\n  method: get\n  operationId: get_payins_card_web_webpayinid_extended\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-methods/metadata\n  method: post\n  operationId: post_payment_methods_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virtual-accounts/availability\n  method:\
  \ get\n  operationId: get_virtual_accounts_availability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{walletId}/virtual-accounts\n  method: post\n  operationId: post_wallets_walletId_virtual_accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets/{usernaturalpayerwalletid}/virtual-accounts/{virtualaccountid}\n  method: put\n  operationId: put_wallets_usernaturalpayerwalletid_virtual_accounts_virtualaccountid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets/{walletId}/virtual-accounts/{virtualaccountid}\n  method: get\n  operationId: get_wallets_walletId_virtual_accounts_virtualaccountid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{usernaturalpayerwalletid}/virtual-accounts\n  method: get\n  operationId: get_wallets_usernaturalpayerwalletid_virtual_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{userlegalownerwalletid}/bankingaliases/iban\n  method: post\n  operationId: post_wallets_userlegalownerwalletid_bankingaliases_iban\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bankingaliases/{bankingaliasid}\n  method: put\n  operationId: put_bankingaliases_bankingaliasid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bankingaliases/{bankingaliasid}\n  method: get\n  operationId: get_bankingaliases_bankingaliasid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{userlegalownerwalletid}/bankingaliases\n  method: get\n\
  \  operationId: get_wallets_userlegalownerwalletid_bankingaliases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payins/bankwire/direct\n  method: post\n  operationId: post_payins_bankwire_direct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-methods/openbanking/metadata/supported-banks\n  method: get\n  operationId: get_payment_methods_openbanking_metadata_supported_banks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payins/payment-methods/openbanking\n  method: post\n  operationId:\
  \ post_payins_payment_methods_openbanking\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates/directdebit/web\n  method: post\n  operationId: post_mandates_directdebit_web\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates/{mandateId}\n  method: get\n  operationId: get_mandates_mandateId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /mandates/{mandateId}/cancel\n  method: put\n  operationId: put_mandates_mandateId_cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates\n  method: get\n  operationId: get_mandates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{legaluserbankaccountid}/mandates\n  method: get\n  operationId: get_users_legaluserbankaccountid_mandates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/mandates\n  method: get\n  operationId:\
  \ get_users_userId_mandates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payins/directdebit/direct\n  method: post\n  operationId: post_payins_directdebit_direct\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/bancontact\n  method: post\n  operationId: post_payins_payment_methods_bancontact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/bizum\n  method: post\n  operationId: post_payins_payment_methods_bizum\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/blik\n  method: post\n  operationId: post_payins_payment_methods_blik\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/ideal\n  method: post\n  operationId: post_payins_payment_methods_ideal\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/klarna\n  method: post\n  operationId: post_payins_payment_methods_klarna\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/mbway\n  method: post\n  operationId: post_payins_payment_methods_mbway\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/multibanco\n  method: post\n  operationId: post_payins_payment_methods_multibanco\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/payconiq\n  method: post\n  operationId: post_payins_payment_methods_payconiq\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/paypal/data-collection\n  method: post\n  operationId: post_payins_payment_methods_paypal_data_collection\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/paypal/data-collection/{datacollectionid}\n  method: get\n  operationId: get_payins_payment_methods_paypal_data_collection_datacollectionid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payins/payment-methods/paypal/recurring\n  method: post\n  operationId: post_payins_payment_methods_paypal_recurring\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/payment-methods/paypal\n  method: post\n  operationId: post_payins_payment_methods_paypal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payins/{paypalpayinid}/trackings\n  method: put\n  operationId: put_payins_paypalpayinid_trackings\n  x-agentic-access:\n    action-class: acting\n    consequence: \n\n# --- truncated at 32 KB (69 KB total) ---\n# Full\
  \ source: https://raw.githubusercontent.com/api-evangelist/mangopay/refs/heads/main/agentic-access/mangopay-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mangopay/refs/heads/main/agentic-access/mangopay-agentic-access.yml
summary_line: 215 operations · 116 acting
tags:
- Payments
- Marketplace Payments
- Digital Wallets
- KYC
- KYB
- Fund Transfers
- Currency Conversion
- Payment Cards
- Fintech
- European
---
