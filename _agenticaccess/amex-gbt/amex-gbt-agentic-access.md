---
acting_count: 97
action_class_counts:
  acting: 97
  connected: 74
api_specs:
- filename: amex-gbt-user-sync-api-openapi.json
  format: json
  label: Egencia User Sync API
  slug: egencia-user-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-user-sync-api-openapi.json
- filename: amex-gbt-sso-context-api-openapi.json
  format: json
  label: Egencia Context SSO API
  slug: egencia-context-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-sso-context-api-openapi.json
- filename: amex-gbt-company-info-api-openapi.json
  format: json
  label: Egencia Company Details API
  slug: egencia-company-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-company-info-api-openapi.json
- filename: amex-gbt-company-cdf-api-openapi.json
  format: json
  label: Egencia Company CDF API
  slug: egencia-company-cdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-company-cdf-api-openapi.json
- filename: amex-gbt-validation-spi-openapi.json
  format: json
  label: Egencia Validation SPI
  slug: egencia-validation-spi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-validation-spi-openapi.json
- filename: amex-gbt-expense-spi-openapi.json
  format: json
  label: Egencia Expense SPI
  slug: egencia-expense-spi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-expense-spi-openapi.json
- filename: amex-gbt-booking-api-openapi.json
  format: json
  label: Egencia Get Booking API
  slug: egencia-get-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-booking-api-openapi.json
- filename: amex-gbt-cancellation-deletion-api-openapi.json
  format: json
  label: Egencia Expense Cancellation and Deletion API
  slug: egencia-cancellation-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-cancellation-deletion-api-openapi.json
- filename: amex-gbt-approval-workflow-api-openapi.json
  format: json
  label: Egencia Approval Workflow API
  slug: egencia-approval-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-approval-workflow-api-openapi.json
- filename: amex-gbt-approval-customisation-spi-openapi.json
  format: json
  label: Egencia Approval Customisation SPI
  slug: egencia-approval-customisation-spi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-approval-customisation-spi-openapi.json
- filename: amex-gbt-receipt-api-openapi.json
  format: json
  label: Egencia Receipt API
  slug: egencia-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-receipt-api-openapi.json
- filename: amex-gbt-duty-of-care-api-openapi.json
  format: json
  label: Egencia Duty of Care API
  slug: egencia-duty-of-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-duty-of-care-api-openapi.json
- filename: amex-gbt-reporting-api-openapi.json
  format: json
  label: Egencia Reporting API (BI Transactions)
  slug: egencia-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-reporting-api-openapi.json
- filename: amex-gbt-service-bi-openapi.json
  format: json
  label: American Express Global Business Travel BI API
  slug: amex-gbt-service-bi-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-bi-openapi.json
- filename: amex-gbt-service-company-openapi.json
  format: json
  label: American Express Global Business Travel OpenAPI definition (Amex Gbt Service Company)
  slug: amex-gbt-service-company-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-company-openapi.json
- filename: amex-gbt-service-dutyofcare-openapi.json
  format: json
  label: American Express Global Business Travel Duty Of Care API
  slug: amex-gbt-service-dutyofcare-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-dutyofcare-openapi.json
- filename: amex-gbt-service-openconnect-openapi.json
  format: json
  label: American Express Global Business Travel OpenAPI definition (Amex Gbt Service Openconnect)
  slug: amex-gbt-service-openconnect-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/openapi/amex-gbt-service-openconnect-openapi.json
consequence_counts:
  read: 74
  safety-critical: 36
  write: 61
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 36
kind: agentic-access
layout: agentic-access
method: generated
name: Amex Gbt Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /base/version
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /gdpr
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /gdpr
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /gdpr
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /gdpr
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sensitive/audit/clean
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sensitive/audit/clean
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/transactions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/transactions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/transactions/air
operation_count: 171
overview: 'American Express Global Business Travel exposes 171 API operations that an AI agent could call, of which 97 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 74 read, 61 write, and 36 safety-critical.


  36 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: American Express Global Business Travel
provider_slug: amex-gbt
slug: amex-gbt-agentic-access
source_filename: amex-gbt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: generated\nsource: openapi/amex-gbt-approval-customisation-spi-openapi.json, openapi/amex-gbt-approval-workflow-api-openapi.json,\n  openapi/amex-gbt-booking-api-openapi.json, openapi/amex-gbt-cancellation-deletion-api-openapi.json,\n  openapi/amex-gbt-company-cdf-api-openapi.json, openapi/amex-gbt-company-info-api-openapi.json,\n  openapi/amex-gbt-duty-of-care-api-openapi.json, openapi/amex-gbt-expense-spi-openapi.json,\n  openapi/amex-gbt-receipt-api-openapi.json, openapi/amex-gbt-reporting-api-openapi.json, openapi/amex-gbt-service-bi-openapi.json,\n  openapi/amex-gbt-service-company-openapi.json, openapi/amex-gbt-service-dutyofcare-openapi.json,\n  openapi/amex-gbt-service-openconnect-openapi.json, openapi/amex-gbt-sso-context-api-openapi.json,\n  openapi/amex-gbt-user-sync-api-openapi.json, openapi/amex-gbt-validation-spi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI.\
  \ A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 171\n  by_action_class:\n    acting: 97\n    connected: 74\n  by_consequence:\n    write: 61\n    read: 74\n    safety-critical: 36\n  human_in_the_loop_required: 36\noperations:\n- path: /v1/custom-approval\n  method: post\n  operationId: getApprovalDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/approve\n  method: post\n  operationId: approveBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/deny\n  method: post\n  operationId: denyBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/items/{itemId}/approve\n  method: post\n  operationId: approveBookingItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/items/{itemId}/deny\n  method: post\n  operationId: denyBookingItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}\n  method: get\n  operationId: getBookingProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}/items/{itemId}\n  method: get\n  operationId: getBookingItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}/items/{itemId}/cancel\n  method: post\n  operationId: cancelBookingItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/items/{itemId}/delete\n  method: post\n  operationId: deleteBookingItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/items/{itemId}/receipts\n  method: get\n  operationId: getReceipt_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingId}/items/{itemId}/receipts\n  method: get\n  operationId: getReceiptsAsZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bookings/{bookingId}/items/{itemId}/receipts/{receiptId}\n  method:\
  \ get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings/{bookingId}/cancel\n  method: post\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{bookingId}/delete\n  method: post\n  operationId: deleteBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{companyId}/cdfs\n  method: get\n  operationId: getCdfDefinitions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{companyId}/cdfs/{definitionId}/values\n  method: get\n  operationId: getCdfValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{companyId}/cdfs/{definitionId}/values\n  method: post\n  operationId: createCdfValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{companyId}/cdfs/{definitionId}/values/{valueId}\n  method: delete\n  operationId: deleteCdfValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{companyId}/cdfs/{definitionId}/values/{valueId}\n  method: get\n  operationId: getCdfLinkedValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{companyId}/cdfs/{definitionId}/values/{valueId}\n  method: put\n  operationId: updateCdfValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/{companyId}/cdfs/{definitionId}/values/{valueId}/link\n  method: patch\n  operationId: patchCdfValue\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies\n  method: get\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company_id}\n  method: get\n  operationId: retrieveCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/ecommerce-settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/ecommerce-settings/audit\n  method: get\n  operationId: getAudit\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings\n  method: post\n  operationId: getDutyOfCareData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{resourceId}\n  method: get\n  operationId: getBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /some.base.path/some.path\n  method: post\n  operationId: pushExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /some.base.path/v1/subscriptions\n  method: post\n  operationId: pushSubscriptionNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/receipts/{itemId}\n  method: get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/egencia_iata\n  method: get\n  operationId: getIATACode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions\n  method: post\n  operationId: queryTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/air\n  method: post\n  operationId: queryTransactionsForAir\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/car\n  method: post\n  operationId: queryTransactionsForCar\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n   \
  \   human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/fees\n  method: post\n  operationId: queryTransactionsForFees\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/ground\n  method: post\n  operationId: queryTransactionsForGround\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/hotel\n  method: post\n  operationId: queryTransactionsForHotel\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/train\n  method: post\n  operationId: queryTransactionsForTrain\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/{reportId}\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/liveness\n  method: get\n  operationId: liveness\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/readiness\n  method: get\n  operationId: readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: delete\n  operationId: version_3\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: get\n  operationId: version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: head\n  operationId: version_5\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: options\n  operationId: version_6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: patch\n  operationId: version_4\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: post\n  operationId: version_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: put\n  operationId: version_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gdpr\n  method: delete\n  operationId: process\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gdpr\n  method: get\n  operationId: validate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/egencia_iata\n  method: get\n  operationId: getIATACode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sensitive/audit/clean\n  method: post\n  operationId: cleanup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions\n  method: post\n  operationId: queryTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n \
  \   audit: required\n- path: /v1/transactions/air\n  method: post\n  operationId: queryTransactionsForAir\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/car\n  method: post\n  operationId: queryTransactionsForCar\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/fees\n  method: post\n  operationId: queryTransactionsForFees\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/ground\n  method: post\n  operationId: queryTransactionsForGround\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/hotel\n  method: post\n  operationId: queryTransactionsForHotel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v1/transactions/train\n  method: post\n  operationId: queryTransactionsForTrain\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/transactions/{reportId}\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing-entity/thirdparty/response/gbt-customer\n  method: post\n  operationId: saveAcknowledgement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies\n  method: get\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company_id}\n  method: get\n  operationId: retrieveCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{company_id}/agent-assist-notes\n  method: get\n  operationId: getAgentAssistNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/ecommerce-settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/ecommerce-settings/audit\n\
  \  method: get\n  operationId: getAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gdpr\n  method: get\n  operationId: validate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gdpr\n  method: delete\n  operationId: process\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/readiness\n  method: get\n  operationId: readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/liveness\n  method:\
  \ get\n  operationId: liveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: get\n  operationId: version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: put\n  operationId: version_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: post\n  operationId: version_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: delete\n  operationId: version_3\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: options\n  operationId: version_6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: head\n  operationId: version_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: patch\n  operationId:\
  \ version_4\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/liveness\n  method: get\n  operationId: liveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/readiness\n  method: get\n  operationId: readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: delete\n  operationId: version_3\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n     \
  \ purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: get\n  operationId: version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: head\n  operationId: version_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: options\n  operationId: version_6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: patch\n  operationId: version_4\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: post\n  operationId: version_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: put\n  operationId: version_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gdpr\n  method: delete\n  operationId: process\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gdpr\n  method: get\n  operationId: validate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookings\n  method: post\n  operationId: getDutyOfCareData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookings/{resourceId}\n  method: get\n  operationId: getBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/sensitive/audit/clean\n  method: post\n  operationId: cleanup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/liveness\n  method: get\n  operationId: liveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/readiness\n  method: get\n  operationId: readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: delete\n  operationId: version_3\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: get\n  operationId: version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: head\n  operationId: version_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: options\n  operationId: version_6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base/version\n  method: patch\n  operationId: version_4\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: post\n  operationId: version_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /base/version\n  method: put\n  operationId: version_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gdpr\n\
  \  method: delete\n  operationId: process\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /gdpr\n  method: get\n  operationId: validate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v1/admin-users\n  method: get\n  operationId: getAllAdminUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v1/admin-users\n  method: post\n  operationId: createAdminUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v1/admin-users/search\n  method: post\n  operationId: searchAdminUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v1/admin-users/{userName}\n  method: patch\n  operationId: patchAdmin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v1/users\n  method: post\n  operationId: createUser_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    esc\n\n# --- truncated at 32 KB (50 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/agentic-access/amex-gbt-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amex-gbt/refs/heads/main/agentic-access/amex-gbt-agentic-access.yml
summary_line: 171 operations · 97 acting · 36 human-in-the-loop
tags:
- Travel
- United States
- Corporate Travel
- Travel Management
- Business Travel
- Distribution
- Booking
- Aviation
- Hotels
- Rail
- Car Rental
- Expense
- Duty of Care
- Reporting
---
