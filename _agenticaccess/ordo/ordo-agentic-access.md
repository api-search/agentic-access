---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 29
api_specs:
- filename: ordo-single-payments.yml
  format: yaml
  label: Ordo Single Payments API
  slug: ordo-single-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-single-payments.yml
- filename: ordo-smart-request-manager.yml
  format: yaml
  label: Ordo Smart Request Manager API
  slug: ordo-smart-request-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-smart-request-manager.yml
- filename: ordo-recurring-payment-mandates.yml
  format: yaml
  label: Ordo Recurring Payment Mandates (VRP) API
  slug: ordo-recurring-payment-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-recurring-payment-mandates.yml
- filename: ordo-account-data-ordo-hosted.yml
  format: yaml
  label: Ordo Account Data (Ordo Hosted) API
  slug: ordo-account-data-ordo-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-data-ordo-hosted.yml
- filename: ordo-account-data-client-hosted.yml
  format: yaml
  label: Ordo Account Data (Client Hosted) API
  slug: ordo-account-data-client-hosted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-account-data-client-hosted.yml
- filename: ordo-registry-manager.yml
  format: yaml
  label: Ordo Registry Manager API
  slug: ordo-registry-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/openapi/ordo-registry-manager.yml
consequence_counts:
  physical: 7
  read: 29
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ordo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /smartRequests/newSmartRequestBDRLink
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /smartRequests/newSmartRequestMessage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /smartRequests/withdrawSmartRequestMessage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /smartRequests/withdrawSmartRequestMessageBDR
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdraw
operation_count: 54
overview: 'Ordo exposes 54 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 18 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ordo
provider_slug: ordo
slug: ordo-agentic-access
source_filename: ordo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/ordo-account-data-client-hosted.yml, openapi/ordo-account-data-ordo-hosted.yml,\n  openapi/ordo-recurring-payment-mandates.yml, openapi/ordo-registry-manager.yml, openapi/ordo-single-payments.yml,\n  openapi/ordo-smart-request-manager.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    connected: 29\n    acting: 25\n  by_consequence:\n    read: 29\n    write: 18\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /account/information/institutions\n  method: get\n  operationId: get-account-information-institutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /account/information/create\n  method: post\n  operationId: post-account-information-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/information/data\n  method: post\n  operationId: post-account-information-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/information/data\n  method: get\n  operationId: get-account-information-data-aisdatarequestid-aisdatarequestid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/consent/{aisConsentId}\n  method: get\n  operationId: get-account-information-consent-aisconsentid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/consents\n  method: get\n  operationId: get-account-information-consents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/cancel\n  method: post\n  operationId: post-account-information-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/information/data/request/{aisDataRequestId}\n\
  \  method: get\n  operationId: get-account-information-data-request-aisdatarequestid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/data/requests/{aisConsentId}\n  method: get\n  operationId: get-account-information-data-requests-aisconsentid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/initiate\n  method: post\n  operationId: post-account-information-clienthostedinitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/verification/create\n  method: post\n  operationId: post-account-verification-create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/verification/initiate\n  method: post\n  operationId: post-account-verification-clienthostedinitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/verification/institutions\n  method: get\n  operationId: get-account-verification-institutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/verification/{avId}\n  method: get\n  operationId:\
  \ get-account-verification-avid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/verification/account\n  method: get\n  operationId: get-account-verification-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/verification/account/{avId}\n  method: get\n  operationId: get-account-verification-account-avid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/create\n  method: post\n  operationId: post-account-information-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /account/information/data\n  method: post\n  operationId: post-account-information-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/information/data\n  method: get\n  operationId: get-account-information-data-aisdatarequestid-aisdatarequestid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/consent/{aisConsentId}\n  method: get\n  operationId: get-account-information-consent-aisconsentid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/consents\n\
  \  method: get\n  operationId: get-account-information-consents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/cancel\n  method: post\n  operationId: post-account-information-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/information/data/request/{aisDataRequestId}\n  method: get\n  operationId: get-account-information-data-request-aisdatarequestid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/information/data/requests/{aisConsentId}\n  method: get\n  operationId: get-account-information-data-requests-aisconsentid\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/verification/create\n  method: post\n  operationId: post-account-verification-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/verification/initiate\n  method: post\n  operationId: post-account-verification-initiate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/verification/institutions\n  method: get\n  operationId: get-account-verification-institutions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/verification/{avId}\n  method: get\n  operationId: get-account-verification-avid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/verification/account\n  method: get\n  operationId: get-account-verification-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/verification/account/{avId}\n  method: get\n  operationId: get-account-verification-account-avid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /VRPMandate/sweeping\n  method: post\n  operationId: post-vrpmandate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /VRPMandate/{mandateId}\n  method: get\n  operationId: get-vrpmandate-mandateid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /VRPMandates\n  method: get\n  operationId: get-vrpmandates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /VRPTransaction/{vrpTransactionId}\n  method: get\n  operationId: get-vrptransaction-vrptransactionid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /VRPTransactions/{vrpMandateId}\n\
  \  method: get\n  operationId: get-vrptransactions-vrpmandateid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /VRPMandate/nonsweeping\n  method: post\n  operationId: 63e10df05af59030f7e5fa4b\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Registry/{billerAccountId}\n  method: get\n  operationId: GetBillerAccountDetailsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Registry/{billerAccountId}\n  method: delete\n  operationId: DeleteBillerAccountAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Registry\n  method: put\n  operationId: PutBillerAccountAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Registry\n  method: post\n  operationId: PostBillerAccountAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Registry\n  method: get\n  operationId: GetBillerAccountsAsync\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Registry/BillerAccountId\n  method: get\n  operationId: GetBillerAccountIdAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /institutions\n  method: get\n  operationId: get-institutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /create\n  method: post\n  operationId: postsmartrequestbdrasync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /initiate\n  method: post\n\
  \  operationId: post-initiatepayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdraw\n  method: post\n  operationId: postwithdrawsmartrequestbdrasync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smartRequests/newSmartRequestBDRLink\n  method: post\n  operationId: PostSmartRequestBDRAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smartRequests/{smartRequestId}\n  method: get\n  operationId: GetSmartRequestAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smartRequests/smartRequestMessages\n  method: get\n  operationId: GetSmartRequestsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smartRequests/withdrawSmartRequestMessageBDR\n  method: post\n  operationId: PostWithdrawSmartRequestBDRAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smartRequests/newSmartRequestMessage\n  method: post\n  operationId: PostSmartRequestAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smartRequests/withdrawSmartRequestMessage\n  method: post\n  operationId: PostWithdrawSmartRequestAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /smartRequests/grantExtensionMessage\n  method: post\n  operationId: PostSmartRequestMessagesGrantDueDateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smartRequests/declineExtensionMessage\n  method: post\n  operationId: PostSmartRequestMessagesDeclineDueDateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordo/refs/heads/main/agentic-access/ordo-agentic-access.yml
summary_line: 54 operations · 25 acting
tags:
- Payments
- United Kingdom
- Open Banking
- Account-to-Account
- Payment Initiation
- Variable Recurring Payments
- Request to Pay
- Real-Time Payments
- Faster Payments
- PSD2
- Account Information
---
