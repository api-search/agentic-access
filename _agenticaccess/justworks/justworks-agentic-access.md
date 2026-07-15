---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 18
api_specs:
- filename: justworks-members-api-openapi.yml
  format: yaml
  label: Justworks Members API
  slug: justworks-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-members-api-openapi.yml
- filename: justworks-company-api-openapi.yml
  format: yaml
  label: Justworks Company API
  slug: justworks-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-company-api-openapi.yml
- filename: justworks-payroll-api-openapi.yml
  format: yaml
  label: Justworks Payroll API
  slug: justworks-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-payroll-api-openapi.yml
- filename: justworks-deductions-api-openapi.yml
  format: yaml
  label: Justworks Deductions API
  slug: justworks-deductions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-deductions-api-openapi.yml
- filename: justworks-time-off-api-openapi.yml
  format: yaml
  label: Justworks Time Off API
  slug: justworks-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-time-off-api-openapi.yml
- filename: justworks-webhooks-api-openapi.yml
  format: yaml
  label: Justworks Webhooks API
  slug: justworks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-webhooks-api-openapi.yml
- filename: justworks-oauth-api-openapi.yml
  format: yaml
  label: Justworks OAuth API
  slug: justworks-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-oauth-api-openapi.yml
consequence_counts:
  read: 18
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Justworks Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/oauth/revoke
operation_count: 27
overview: 'Justworks exposes 27 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 8 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Justworks
provider_slug: justworks
slug: justworks-agentic-access
source_filename: justworks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/justworks-company-api-openapi.yml, openapi/justworks-deductions-api-openapi.yml,\n  openapi/justworks-members-api-openapi.yml, openapi/justworks-oauth-api-openapi.yml, openapi/justworks-payroll-api-openapi.yml,\n  openapi/justworks-time-off-api-openapi.yml, openapi/justworks-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 18\n    acting: 9\n  by_consequence:\n    read: 18\n    write: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/company\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/company/bank-account\n  method: get\n  operationId: getCompanyBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/business-info\n  method: get\n  operationId: getCompanyBusinessInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/custom-fields\n  method: get\n  operationId: listCompanyCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/jurisdictions\n  method: get\n  operationId: listCompanyJurisdictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deduction-types\n\
  \  method: get\n  operationId: listDeductionTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deductions\n  method: get\n  operationId: listDeductions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deductions\n  method: post\n  operationId: createDeductions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deductions\n  method: put\n  operationId: updateDeductions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deductions/cancel\n  method: patch\n  operationId: cancelDeductions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/members\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/members/{member_id}\n  method: get\n  operationId: getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/members/{member_id}/custom-field-values\n  method: get\n  operationId: listMemberCustomFieldValues\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/members/{member_id}/tax-id\n  method: get\n  operationId: getMemberTaxId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: obtainOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/oauth/revoke\n  method: post\n  operationId: revokeOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/payrolls\n  method: get\n  operationId: listPayrolls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payrolls/{payroll_id}/fees\n  method: get\n  operationId: listPayrollFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payrolls/{payroll_id}/paystubs\n  method: get\n  operationId: listPaystubsForPayroll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/paystubs/{paystub_id}\n  method: get\n  operationId: getPaystub\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/time-off/balances\n  method: post\n  operationId: createTimeOffBalancesReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/time-off/balances/{report_id}\n  method: get\n  operationId: getTimeOffBalancesReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/time-off/policies\n  method: get\n  operationId: listTimeOffPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/time-off/requests\n  method: get\n  operationId: listTimeOffRequests\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/get\n  method: post\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhook_id}/resume\n  method: post\n  operationId: resumeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhook_id}/simulate\n  method: post\n  operationId: simulateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/agentic-access/justworks-agentic-access.yml
summary_line: 27 operations · 9 acting · 1 human-in-the-loop
tags:
- PEO
- Payroll
- HR
- Human Resources
- Benefits
- Health Insurance
- 401(k)
- Time Off
- Compliance
- Small Business
- Employer of Record
- HRIS
---
