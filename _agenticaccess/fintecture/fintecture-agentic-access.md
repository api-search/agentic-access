---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 36
api_specs:
- filename: fintecture-pis-api-openapi.yml
  format: yaml
  label: Fintecture Payment Initiation Services API
  slug: fintecture-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-pis-api-openapi.yml
- filename: fintecture-ais-api-openapi.yml
  format: yaml
  label: Fintecture Account Information Services API
  slug: fintecture-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-ais-api-openapi.yml
- filename: fintecture-customers-api-openapi.yml
  format: yaml
  label: Fintecture Customers API
  slug: fintecture-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-customers-api-openapi.yml
- filename: fintecture-emandates-api-openapi.yml
  format: yaml
  label: Fintecture E-Mandates API
  slug: fintecture-emandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-emandates-api-openapi.yml
- filename: fintecture-oauth-api-openapi.yml
  format: yaml
  label: Fintecture OAuth and Tokens API
  slug: fintecture-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-oauth-api-openapi.yml
- filename: fintecture-resources-api-openapi.yml
  format: yaml
  label: Fintecture Resources API
  slug: fintecture-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-resources-api-openapi.yml
- filename: fintecture-oac-api-openapi.yml
  format: yaml
  label: Fintecture Organisation Access Credentials API
  slug: fintecture-oac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-oac-api-openapi.yml
- filename: fintecture-transactions-api-openapi.yml
  format: yaml
  label: Fintecture Transactions and Settlements API
  slug: fintecture-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-transactions-api-openapi.yml
consequence_counts:
  physical: 7
  read: 36
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fintecture Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pis/v2/connect
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /pis/v2/payments/{payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pis/v2/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pis/v2/request-for-payout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/memberships/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/memberships/{membership_id}
operation_count: 69
overview: 'Fintecture exposes 69 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read, 26 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fintecture
provider_slug: fintecture
slug: fintecture-agentic-access
source_filename: fintecture-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fintecture-ais-api-openapi.yml, openapi/fintecture-customers-api-openapi.yml,\n  openapi/fintecture-emandates-api-openapi.yml, openapi/fintecture-oac-api-openapi.yml, openapi/fintecture-oauth-api-openapi.yml,\n  openapi/fintecture-pis-api-openapi.yml, openapi/fintecture-resources-api-openapi.yml, openapi/fintecture-transactions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    connected: 36\n    acting: 33\n  by_consequence:\n    read: 36\n    write: 26\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /ais/v1/provider/{provider_id}/authorize\n  method: get\n  operationId: getAisV1ProviderAuthorization\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ais/v1/provider/{provider_id}/authorize/decoupled\n  method: get\n  operationId: getAisV1ProviderAuthorizationDecoupled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ais/v2/connect\n  method: get\n  operationId: getAisV2Connect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ais/v1/customer/{customer_id}\n  method: delete\n  operationId: deleteAisV1Customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ais/v1/customer/{customer_id}/accounts\n\
  \  method: get\n  operationId: getAisV1CustomerAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ais/v1/customer/{customer_id}/account/{account_id}\n  method: get\n  operationId: getAisV1CustomerAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ais/v1/customer/{customer_id}/account/{account_id}/holders\n  method: get\n  operationId: getAisV1CustomerAccountHolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ais/v1/customer/{customer_id}/account/{account_id}/transactions\n  method: get\n  operationId: getAisV1CustomerAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /ais/v1/verification\n  method: post\n  operationId: createAisV1Verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers\n  method: get\n  operationId: listAllCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}\n  method: get\n\
  \  operationId: getCustomerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/bank-accounts\n  method: get\n  operationId: listAllCustomerBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/bank-accounts\n  method: post\n  operationId: createCustomerBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/bank-accounts/{account_id}\n  method: get\n  operationId: getBankAccountById\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/verification\n  method: post\n  operationId: initiateCustomerVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/verifications\n  method: get\n  operationId: listAllCustomerVerifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/verification/{verification_id}\n  method: get\n  operationId: getCustomerVerificationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/e-mandates\n  method: get\n  operationId: listAllEmandates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/e-mandates\n  method: post\n  operationId: createEmandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/e-mandates/{mandate_id}\n  method: get\n  operationId: getEmandateById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/e-mandates/{mandate_id}\n  method: patch\n  operationId: patchEmandateById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications\n  method: get\n  operationId: getApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications\n  method: post\n  operationId: postApplications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/current\n  method: get\n  operationId: getResV1Applications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{app_id}\n\
  \  method: get\n  operationId: getApplicationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{app_id}\n  method: patch\n  operationId: patchApplicationById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/{app_id}\n  method: delete\n  operationId: deleteApplicationById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bank-accounts\n  method: get\n  operationId: getBankAccounts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bank-accounts\n  method: post\n  operationId: postBankAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bank-accounts/{bank_account_id}\n  method: patch\n  operationId: patchBankAccountById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bank-accounts/{bank_account_id}\n  method: delete\n  operationId: deleteBankAccountById\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies\n  method: get\n  operationId: getCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies\n  method: post\n  operationId: postCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company_id}\n  method: get\n  operationId: getCompanyById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company_id}\n  method: patch\n  operationId: patchCompanyById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{company_id}\n  method: delete\n  operationId: deleteCompanyById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organisation-nodes\n  method: post\n  operationId: postOrganisationNodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organisation-nodes/{organisation_node_id}\n  method: get\n  operationId: getOrganisationNodeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organisation-nodes/{organisation_node_id}\n  method: patch\n  operationId: patchOrganisationNodeById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organisation-nodes/{organisation_node_id}\n  method: delete\n  operationId: deleteOrganisationNodeById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organisation-nodes/{organisation_node_id}/tree\n  method: get\n  operationId: getOrganisationNodeTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organisation-nodes/{organisation_node_id}/companies\n  method: get\n  operationId: getOrganisationNodeCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/memberships\n  method: post\n  operationId: postMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/memberships/{membership_id}\n  method: patch\n  operationId: patchMembershipById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/memberships/{membership_id}\n  method: delete\n  operationId: deleteMembershipById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users\n  method: post\n\
  \  operationId: postUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{user_id}\n  method: get\n  operationId: getUserById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{user_id}\n  method: patch\n  operationId: patchUserById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{user_id}\n  method: delete\n  operationId: deleteUserById\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/accesstoken\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/refreshtoken\n  method: post\n  operationId: createRefreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pis/v2/connect\n  method: post\n  operationId: createPisV2Connect\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pis/v2/payments\n  method: get\n  operationId: getPisV2Payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pis/v2/payments/{payment_id}\n  method: get\n  operationId: getPaymentSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pis/v2/payments/{payment_id}\n  method: patch\n  operationId: patchPisV2PaymentSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pis/v2/payments/{payment_id}/refunds\n  method: get\n  operationId: getPisV2PaymentRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pis/v2/refund\n  method: post\n  operationId: createPisV2Refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pis/v2/request-to-pay\n  method: post\n  operationId: createPisV2RequestToPay\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pis/v2/request-for-payout\n  method: post\n  operationId: createPisV2RequestForPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pis/v2/settlements\n  method: get\n  operationId: getPisV2Settlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pis/v2/settlements/{settlement_id}\n  method: get\n  operationId: getSettlementById\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /res/v1/providers\n  method: get\n  operationId: getResV1Providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /res/v1/providers/{provider_id}\n  method: get\n  operationId: getResV1Provider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /res/v1/test-accounts\n  method: get\n  operationId: getResV1TestAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /res/v1/test-accounts/{account_id}\n  method: get\n  operationId: getResV1TestAccountById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions\n  method: get\n  operationId: listAllTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transaction_id}\n  method: get\n  operationId: getTransactionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/simulate\n  method: post\n  operationId: simulateTransactionEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/agentic-access/fintecture-agentic-access.yml
summary_line: 69 operations · 33 acting
tags:
- Open Banking
- Payments
- PSD2
- France
- Account Information
- Payment Initiation
- Instant Payments
- SEPA
- Smart Transfer
- Request To Pay
- Buy Now Pay Later
- E-Mandates
- Account-to-Account
- KYC
---
