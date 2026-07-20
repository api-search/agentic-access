---
acting_count: 50
action_class_counts:
  acting: 50
  connected: 19
api_specs:
- filename: earnipay-e-invoicing-openapi-original.json
  format: json
  label: Earnipay Invoicing API
  slug: earnipay-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/openapi/earnipay-e-invoicing-openapi-original.json
consequence_counts:
  read: 19
  safety-critical: 50
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 50
kind: agentic-access
layout: agentic-access
method: generated
name: Earnipay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/api/v1/businesses/{businessId}/app/invoices/{invoiceId}/payment-status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/api/v1/businesses/{businessId}/app/invoices/{invoiceId}/submit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/forgot-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/login
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/refresh
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/resend-code
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/signup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/verify-email
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/banks/verify-account
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/businesses
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/businesses/upload
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/businesses/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/businesses/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/businesses/{id}/app-config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/businesses/{id}/app-provider
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/businesses/{id}/crypto-keys
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/businesses/{id}/firs-config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/businesses/{id}/interswitch-credentials
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/businesses/{id}/set-default
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/businesses/{id}/settings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/businesses/{id}/test-app-connection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/businesses/{id}/test-interswitch-connection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/customers
operation_count: 69
overview: 'Earnipay exposes 69 API operations that an AI agent could call, of which 50 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 50 safety-critical.


  50 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Earnipay
provider_slug: earnipay
slug: earnipay-agentic-access
source_filename: earnipay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/earnipay-e-invoicing-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    connected: 19\n    acting: 50\n  by_consequence:\n    read: 19\n    safety-critical: 50\n  human_in_the_loop_required: 50\noperations:\n- path: /v1\n  method: get\n  operationId: AppController_getHello_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/signup\n  method: post\n  operationId: AuthController_signup_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/verify-email\n  method: post\n  operationId: AuthController_verifyEmail_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/resend-code\n  method: post\n  operationId: AuthController_resendVerificationCode_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /v1/auth/login\n  method: post\n  operationId: AuthController_login_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/refresh\n  method: post\n  operationId: AuthController_refreshToken_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/logout\n  method: post\n  operationId: AuthController_logout_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/forgot-password\n  method: post\n  operationId: AuthController_forgotPassword_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/reset-password\n  method: post\n  operationId: AuthController_resetPassword_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /v1/users/me\n  method: get\n  operationId: UserController_getCurrentUser_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/me\n  method: patch\n  operationId: UserController_updateProfile_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/users/change-password\n  method: post\n  operationId: UserController_changePassword_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v1/users/me/completion\n  method: get\n  operationId: UserController_getProfileCompletion_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/upload\n  method: post\n  operationId: BusinessController_uploadFile_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses\n  method: post\n  operationId: BusinessController_createBusiness_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses\n  method: get\n  operationId: BusinessController_getUserBusinesses_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{id}\n  method: get\n  operationId: BusinessController_getBusinessById_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{id}\n  method: patch\n  operationId: BusinessController_updateBusiness_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /v1/businesses/{id}\n  method: delete\n  operationId: BusinessController_deleteBusiness_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/{id}/settings\n  method: patch\n  operationId: BusinessController_updateBusinessSettings_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/{id}/firs-config\n  method: patch\n  operationId: BusinessController_updateFirsConfig_v1\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/{id}/crypto-keys\n  method: patch\n  operationId: BusinessController_uploadCryptoKeys_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/{id}/app-config\n  method: patch\n  operationId: BusinessController_updateAppConfig_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/{id}/test-app-connection\n  method: post\n  operationId: BusinessController_testAppConnection_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/{id}/set-default\n  method: post\n  operationId: BusinessController_setDefaultBusiness_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/{id}/app-provider\n\
  \  method: patch\n  operationId: BusinessController_updateAppProvider_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/{id}/interswitch-credentials\n  method: patch\n  operationId: BusinessController_updateInterswitchCredentials_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/{id}/test-interswitch-connection\n  method: post\n  operationId: BusinessController_testInterswitchConnection_v1\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/businesses/providers/supported\n  method: get\n  operationId: BusinessController_getSupportedProviders_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/v1/businesses/{businessId}/app/connection-test\n  method: get\n  operationId: AppProviderController_testConnection_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/v1/businesses/{businessId}/app/invoices/{invoiceId}/submit\n  method: post\n  operationId: AppProviderController_submitInvoice_v1\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/api/v1/businesses/{businessId}/app/invoices/{invoiceId}/payment-status\n  method: patch\n  operationId: AppProviderController_updatePaymentStatus_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/api/v1/businesses/{businessId}/app/invoices/search\n  method: get\n  operationId: AppProviderController_searchInvoices_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: post\n  operationId: CustomerController_createCustomer_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/customers\n  method: get\n  operationId: CustomerController_getCustomers_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{id}\n  method: get\n  operationId: CustomerController_getCustomerById_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{id}\n  method: patch\n  operationId: CustomerController_updateCustomer_v1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/customers/{id}\n  method: delete\n  operationId: CustomerController_deleteCustomer_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/products\n  method: post\n  operationId: ProductController_createProduct_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n    \
  \  purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/products\n  method: get\n  operationId: ProductController_getProducts_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{id}\n  method: get\n  operationId: ProductController_getProductById_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{id}\n  method: patch\n  operationId: ProductController_updateProduct_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /v1/products/{id}\n  method: delete\n  operationId: ProductController_deleteProduct_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoices\n  method: post\n  operationId: InvoiceController_createInvoice_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoices\n  method: get\n  operationId: InvoiceController_getInvoices_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/{id}/approve\n  method: post\n  operationId: InvoiceController_approveInvoice_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoices/{id}/reject\n  method: post\n  operationId: InvoiceController_rejectInvoice_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoices/{id}\n  method: get\n  operationId: InvoiceController_getInvoiceById_v1\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/{id}\n  method: patch\n  operationId: InvoiceController_updateInvoice_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoices/{id}\n  method: delete\n  operationId: InvoiceController_cancelInvoice_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoices/{id}/generate-qr\n  method: post\n\
  \  operationId: InvoiceController_generateQrCode_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/invoices/{id}/pdf\n  method: get\n  operationId: InvoiceController_downloadPdf_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/{id}/submit-to-app\n  method: post\n  operationId: InvoiceController_submitToApp_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/invoices/validate\n  method: post\n  operationId: InvoiceController_validateInvoiceData_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/irn-generator/generate\n  method: post\n  operationId: IrnGeneratorController_generateIRN_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/qr-generator/generate\n  method: post\n  operationId: QrGeneratorController_generateQRCode_v1\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/payment-details\n  method: post\n  operationId: PaymentDetailController_create_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/payment-details\n  method: get\n  operationId: PaymentDetailController_findAll_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment-details/{id}\n  method: get\n  operationId: PaymentDetailController_findOne_v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment-details/{id}\n  method: patch\n  operationId: PaymentDetailController_update_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/payment-details/{id}\n  method: delete\n  operationId: PaymentDetailController_remove_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/team/invite\n\
  \  method: post\n  operationId: TeamController_inviteTeamMember_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/team\n  method: get\n  operationId: TeamController_getTeam_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/team/invitations/{token}/accept\n  method: post\n  operationId: TeamController_acceptInvitation_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/team/invitations/{id}\n  method: delete\n  operationId: TeamController_revokeInvitation_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/team/members/{id}/role\n  method: patch\n  operationId: TeamController_updateMemberRole_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/team/members/{id}\n  method: delete\n  operationId: TeamController_removeMember_v1\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/banks/list\n  method: get\n  operationId: BankController_getBankList_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/banks/verify-account\n  method: post\n  operationId: BankController_verifyBankAccount_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earnipay/refs/heads/main/agentic-access/earnipay-agentic-access.yml
summary_line: 69 operations · 50 acting · 50 human-in-the-loop
tags:
- Company
- E-Invoicing
- Invoicing
- FIRS
- NRS
- Tax
- Compliance
- Fintech
- Nigeria
- Payments
- Financial Services
---
