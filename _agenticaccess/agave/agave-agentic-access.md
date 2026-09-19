---
acting_count: 226
action_class_counts:
  acting: 226
  connected: 212
api_specs:
- filename: agave-budgets-api-openapi.yml
  format: yaml
  label: Agave Budgets API
  slug: agave-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-budgets-api-openapi.yml
- filename: agave-contracts-api-openapi.yml
  format: yaml
  label: Agave Contracts API
  slug: agave-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-contracts-api-openapi.yml
- filename: agave-cost-codes-api-openapi.yml
  format: yaml
  label: Agave Cost Codes API
  slug: agave-cost-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-cost-codes-api-openapi.yml
- filename: agave-employees-api-openapi.yml
  format: yaml
  label: Agave Employees API
  slug: agave-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-employees-api-openapi.yml
- filename: agave-invoices-api-openapi.yml
  format: yaml
  label: Agave Invoices API
  slug: agave-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-invoices-api-openapi.yml
- filename: agave-link-sessions-api-openapi.yml
  format: yaml
  label: Agave Link Sessions API
  slug: agave-link-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-link-sessions-api-openapi.yml
- filename: agave-projects-api-openapi.yml
  format: yaml
  label: Agave Projects API
  slug: agave-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-projects-api-openapi.yml
- filename: agave-timesheets-api-openapi.yml
  format: yaml
  label: Agave Timesheets API
  slug: agave-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-timesheets-api-openapi.yml
- filename: agave-vendors-api-openapi.yml
  format: yaml
  label: Agave Vendors API
  slug: agave-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-vendors-api-openapi.yml
- filename: agave-common-api-openapi.yml
  format: yaml
  label: Agave Common API
  slug: agave-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-common-api-openapi.yml
- filename: agave-customer-management-api-openapi.yml
  format: yaml
  label: Agave Customer Management API
  slug: agave-customer-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-customer-management-api-openapi.yml
- filename: agave-file-management-api-openapi.yml
  format: yaml
  label: Agave File Management API
  slug: agave-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-file-management-api-openapi.yml
- filename: agave-financials-management-api-openapi.yml
  format: yaml
  label: Agave Financials Management API
  slug: agave-financials-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-financials-management-api-openapi.yml
- filename: agave-project-management-api-openapi.yml
  format: yaml
  label: Agave Project Management API
  slug: agave-project-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-project-management-api-openapi.yml
- filename: agave-service-management-api-openapi.yml
  format: yaml
  label: Agave Service Management API
  slug: agave-service-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-service-management-api-openapi.yml
- filename: agave-webhooks-api-openapi.yml
  format: yaml
  label: Agave Webhooks API
  slug: agave-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/openapi/agave-webhooks-api-openapi.yml
consequence_counts:
  physical: 49
  read: 212
  safety-critical: 3
  write: 174
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Agave Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/accounts/{id}/revoke-tokens
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /link/revoke-tokens
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /opportunities
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ap-invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ap-invoices/{ap_invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /ap-invoices/{ap_invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ap-invoices/{ap_invoice_id}/line-items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ap-invoices/{ap_invoice_id}/line-items/{ap_invoice_line_item_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /ap-invoices/{ap_invoice_id}/line-items/{ap_invoice_line_item_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ap-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ap-payments/{ap_payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /ap-payments/{ap_payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ap-payments/{ap_payment_id}/line-items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ap-payments/{ap_payment_id}/line-items/{ap_payment_line_item_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /ap-payments/{ap_payment_id}/line-items/{ap_payment_line_item_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ar-invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ar-invoices/{ar_invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /ar-invoices/{ar_invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ar-invoices/{ar_invoice_id}/line-items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ar-invoices/{ar_invoice_id}/line-items/{ar_invoice_line_item_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /ar-invoices/{ar_invoice_id}/line-items/{ar_invoice_line_item_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ar-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ar-payments/{ar_payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /ar-payments/{ar_payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ar-payments/{ar_payment_id}/line-items
operation_count: 438
overview: 'Agave exposes 438 API operations that an AI agent could call, of which 226 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 212 read, 174 write, 49 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agave
provider_slug: agave
slug: agave-agentic-access
source_filename: agave-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/agave-budgets-api-openapi.yml, openapi/agave-common-api-openapi.yml, openapi/agave-contracts-api-openapi.yml,\n  openapi/agave-cost-codes-api-openapi.yml, openapi/agave-customer-management-api-openapi.yml,\n  openapi/agave-employees-api-openapi.yml, openapi/agave-file-management-api-openapi.yml, openapi/agave-financials-management-api-openapi.yml,\n  openapi/agave-invoices-api-openapi.yml, openapi/agave-link-sessions-api-openapi.yml, openapi/agave-project-management-api-openapi.yml,\n  openapi/agave-projects-api-openapi.yml, openapi/agave-service-management-api-openapi.yml,\n  openapi/agave-timesheets-api-openapi.yml, openapi/agave-vendors-api-openapi.yml, openapi/agave-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 438\n  by_action_class:\n    connected: 212\n    acting: 226\n  by_consequence:\n    read: 212\n    write: 174\n    safety-critical: 3\n    physical: 49\n  human_in_the_loop_required: 3\noperations:\n- path: /budgets\n  method: get\n  operationId: listBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: getPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/token/create\n  method: post\n  operationId: postLinkTokenCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link/token/exchange\n\
  \  method: post\n  operationId: postLinkTokenExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link/sessions\n  method: post\n  operationId: postLinkSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link/sessions\n  method: get\n  operationId: getLinkSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/sessions/xxx/extend\n  method: post\n  operationId: postLinkSessionsXxxExtend\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link/sessions/xxx/expire\n  method: post\n  operationId: postLinkSessionsXxxExpire\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link/account\n  method: get\n  operationId: getLinkAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/edit\n  method: post\n  operationId: postLinkEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link/source-system\n  method: get\n  operationId: getLinkSourceSystem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/source-systems\n  method: get\n  operationId: getLinkSourceSystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/connection\n  method: get\n  operationId: getLinkConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/rate-limits\n  method: get\n  operationId: getLinkRateLimits\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/company\n  method: get\n  operationId: getLinkCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/companies\n  method: get\n  operationId: getLinkCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/user\n  method: get\n  operationId: getLinkUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/account/create\n  method: post\n  operationId: postLinkAccountCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link/debug/session\n  method: post\n  operationId: postLinkDebugSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link/revoke-tokens\n  method: post\n  operationId: postLinkRevokeTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /async-requests/{async_request_id}\n  method: get\n  operationId: getAsyncRequestsByAsyncRequestId\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/accounts/{id}\n  method: get\n  operationId: getAdminAccountsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/accounts/{id}/sessions\n  method: get\n  operationId: getAdminAccountsByIdSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/accounts/{id}/events\n  method: get\n  operationId: getAdminAccountsByIdEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/accounts/{id}/requests\n  method: get\n  operationId: getAdminAccountsByIdRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /admin/accounts\n  method: get\n  operationId: getAdminAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/link-tokens\n  method: get\n  operationId: getAdminLinkTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/accounts/{id}/revoke-tokens\n  method: post\n  operationId: postAdminAccountsByIdRevokeTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cache/repopulate\n  method: post\n  operationId: postCacheRepopulate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cache/{cache_id}\n  method: get\n  operationId: getCacheByCacheId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cache/repopulate/latest\n  method: get\n  operationId: getCacheRepopulateLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: get\n  operationId: listContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-codes\n  method: get\n  operationId: listCostCodes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities\n  method: get\n  operationId: getActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities\n  method: post\n  operationId: postActivities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activities/{activity_id}\n  method: get\n  operationId: getActivitiesByActivityId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities/{activity_id}\n  method: put\n  operationId: putActivitiesByActivityId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activities/{activity_id}\n  method: delete\n  operationId: deleteActivitiesByActivityId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activities/{activity_id}/attachments\n  method: post\n  operationId: postActivitiesByActivityIdAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /appointments\n  method: get\n  operationId: getAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments/{appointment_id}\n  method: get\n  operationId: getAppointmentsByAppointmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: postCustomers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}\n  method: get\n  operationId: getCustomersByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}\n  method: put\n  operationId: putCustomersByCustomerId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}\n  method: delete\n  operationId: deleteCustomersByCustomerId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /leads\n  method: get\n  operationId: getLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/{lead_id}\n  method: get\n  operationId: getLeadsByLeadId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities\n  method: get\n  operationId: getOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities\n  method: post\n  operationId: postOpportunities\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /opportunities/{opportunity_id}\n  method: get\n  operationId: getOpportunitiesByOpportunityId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{opportunity_id}\n  method: put\n  operationId: putOpportunitiesByOpportunityId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{opportunity_id}\n  method: delete\n  operationId: deleteOpportunitiesByOpportunityId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /root-folder\n  method: get\n  operationId: getRootFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders/{folder_id}\n  method: get\n  operationId: getFoldersByFolderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders/{folder_id}\n  method: put\n  operationId: putFoldersByFolderId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders/{folder_id}\n  method: delete\n  operationId: deleteFoldersByFolderId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders\n  method: post\n  operationId: postFolders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders/{folder_id}/files\n  method: get\n  operationId: getFoldersByFolderIdFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /folders/{folder_id}/files\n  method: post\n  operationId: postFoldersByFolderIdFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}\n  method: get\n  operationId: getFilesByFileId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}\n  method: put\n  operationId: putFilesByFileId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}\n  method: delete\n\
  \  operationId: deleteFilesByFileId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders/{folder_id}/transfer\n  method: post\n  operationId: postFoldersByFolderIdTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}/transfer\n  method: post\n  operationId: postFilesByFileIdTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file-transfers/{file_transfer_id}\n  method: get\n  operationId: getFileTransfersByFileTransferId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}/versions\n  method: get\n  operationId: getFilesByFileIdVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}/versions\n  method: post\n  operationId: postFilesByFileIdVersions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /files/{file_id}/versions/{file_version_id}\n  method: get\n  operationId: getFilesByFileIdVersionsByFileVersionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /photos\n  method: get\n  operationId: getPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /photos\n  method: post\n  operationId: postPhotos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /photos/{photo_id}\n  method: get\n  operationId: getPhotosByPhotoId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /photos/{photo_id}\n  method: put\n  operationId: putPhotosByPhotoId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /photos/{photo_id}\n  method: delete\n  operationId: deletePhotosByPhotoId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets\n  method: post\n\
  \  operationId: postAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{asset_id}\n  method: get\n  operationId: getAssetsByAssetId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{asset_id}\n  method: put\n  operationId: putAssetsByAssetId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-invoices\n  method: get\n  operationId: getApInvoices\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap-invoices\n  method: post\n  operationId: postApInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-invoices/{ap_invoice_id}\n  method: get\n  operationId: getApInvoicesByApInvoiceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap-invoices/{ap_invoice_id}\n  method: put\n  operationId: putApInvoicesByApInvoiceId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-invoices/{ap_invoice_id}\n  method: delete\n  operationId: deleteApInvoicesByApInvoiceId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-invoices/{ap_invoice_id}/line-items\n  method: get\n  operationId: getApInvoicesByApInvoiceIdLineItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap-invoices/{ap_invoice_id}/line-items\n  method: post\n  operationId: postApInvoicesByApInvoiceIdLineItems\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-invoices/{ap_invoice_id}/line-items/{ap_invoice_line_item_id}\n  method: get\n  operationId: getApInvoicesByApInvoiceIdLineItemsByApInvoiceLineItemId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap-invoices/{ap_invoice_id}/line-items/{ap_invoice_line_item_id}\n  method: put\n  operationId: putApInvoicesByApInvoiceIdLineItemsByApInvoiceLineItemId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-invoices/{ap_invoice_id}/line-items/{ap_invoice_line_item_id}\n  method: delete\n  operationId: deleteApInvoicesByApInvoiceIdLineItemsByApInvoiceLineItemId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-payments\n  method: get\n  operationId: getApPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap-payments\n  method: post\n  operationId: postApPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-payments/{ap_payment_id}\n  method: get\n  operationId: getApPaymentsByApPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap-payments/{ap_payment_id}\n  method: put\n  operationId: putApPaymentsByApPaymentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-payments/{ap_payment_id}\n  method: delete\n  operationId: deleteApPaymentsByApPaymentId\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-payments/{ap_payment_id}/line-items\n  method: get\n  operationId: getApPaymentsByApPaymentIdLineItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap-payments/{ap_payment_id}/line-items\n  method: post\n  operationId: postApPaymentsByApPaymentIdLineItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /ap-payments/{ap_payment_id}/line-items/{ap_payment_line_item_id}\n  method: get\n  operationId: getApPaymentsByApPaymentIdLineItemsByApPaymentLineItemId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap-payments/{ap_payment_id}/line-items/{ap_payment_line_item_id}\n  method: put\n  operationId: putApPaymentsByApPaymentIdLineItemsByApPaymentLineItemId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap-payments/{ap_payment_id}/line-items/{ap_payment_line_item_id}\n  method: delete\n  operationId: deleteApPaymentsByApPaymentIdLineItemsByApPaymentLineItemId\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ar-invoices\n  method: get\n  operationId: getArInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ar-invoices\n  method: post\n  operationId: postArInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ar-invoices/{ar_invoice_id}\n  method: get\n  operationId: getArInvoicesByArInvoiceId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ar-invoices/{ar_invoice_id}\n  method: put\n  operationId: putArInvoicesByArInvoiceId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ar-invoices/{ar_invoice_id}\n  method: delete\n  operationId: deleteArInvoicesByArInvoiceId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /ar-invoices/{ar_invoice_id}/line-items\n  method: get\n  operationId: getArInvoicesByArInvoiceIdLineItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ar-invoices/{ar_invoice_id}/line-items\n  method: post\n  operationId: postArInvoicesByArInvoiceIdLineItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ar-invoices/{ar_invoice_id}/line-items/{ar_invoice_line_item_id}\n  method: get\n  operationId: getArInvoicesByArInvoiceIdLineItemsByArInvoiceLineItemId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \n\n# --- truncated\
  \ at 32 KB (134 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/agentic-access/agave-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/agentic-access/agave-agentic-access.yml
summary_line: 438 operations · 226 acting · 3 human-in-the-loop
tags:
- Accounting
- Construction
- Integration
- ERP
- Project Management
- Unified-API
- iPaaS
- Webhook
- Field Service
- Invoicing
---
