---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 16
api_specs:
- filename: paylocity-openapi.yml
  format: yaml
  label: Paylocity Integrations REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paylocity/refs/heads/main/openapi/paylocity-openapi.yml
consequence_counts:
  physical: 2
  read: 16
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Paylocity Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /compliance/backgroundcheck/candidatescreeningorders/subscription
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /compliance/backgroundcheck/candidatescreeningorders/subscription
operation_count: 29
overview: 'Paylocity exposes 29 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 11 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paylocity
provider_slug: paylocity
slug: paylocity-agentic-access
source_filename: paylocity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/paylocity-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 16\n    acting: 13\n  by_consequence:\n    read: 16\n    write: 11\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/companies/{companyId}/employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/companies/{companyId}/employees\n  method: post\n  operationId: addEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/companies/{companyId}/employees/{employeeId}\n  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/companies/{companyId}/employees/{employeeId}\n  method: patch\n  operationId: updateEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/onboarding\n  method: post\n  operationId: onboardEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/earnings\n  method: get\n  operationId: listEarnings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/earnings\n  method: post\n  operationId: upsertEarning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}/{startDate}\n  method: get\n  operationId: getEarning\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}/{startDate}\n  method: delete\n  operationId: deleteEarning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/deductions\n  method: get\n  operationId: listDeductions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/deductions\n  method: post\n  operationId: upsertDeduction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/localtax\n  method: get\n  operationId: listLocalTaxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/localtax\n  method: post\n  operationId: addLocalTax\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/companies/{companyId}/employees/{employeeId}/statetax/primary\n  method: post\n  operationId: upsertPrimaryStateTax\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apihub/time/v2/companies/{companyId}/punchdetails\n  method: post\n  operationId: createPunchDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apihub/time/v2/companies/{companyId}/employees/{employeeId}/punchdetails\n  method: get\n  operationId: getEmployeePunchDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apihub/scheduling/v1/companies/{companyId}/shifts\n  method: get\n\
  \  operationId: listShifts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apihub/scheduling/v1/companies/{companyId}/employees/{employeeId}/shifts\n  method: get\n  operationId: listEmployeeShifts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apihub/scheduling/v1/companies/{companyId}/openshifts\n  method: get\n  operationId: listOpenShifts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apihub/learningmanagementsystem/v1/companies/{companyId}/contents\n  method: get\n  operationId: listLmsContents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apihub/learningmanagementsystem/v1/companies/{companyId}/contents\n\
  \  method: post\n  operationId: createLmsContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payentry/v2/payentryimport\n  method: post\n  operationId: createPayrollBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payentry/v2/payentryimport/{timeImportFileTrackingId}\n  method: get\n  operationId: getPayrollBatchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apihub/payrollhistory/v1/companies/{companyId}/employees/{employeeId}/paystatements\n\
  \  method: get\n  operationId: listPayStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/companies/{companyId}/codes\n  method: get\n  operationId: listCompanyCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/companies/{companyId}/openapi\n  method: get\n  operationId: getCompanyOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compliance/backgroundcheck/screeningpackages\n  method: get\n  operationId: listScreeningPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compliance/backgroundcheck/candidatescreeningorders/subscription\n\
  \  method: post\n  operationId: createBackgroundCheckSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compliance/backgroundcheck/candidatescreeningorders/subscription\n  method: delete\n  operationId: deleteBackgroundCheckSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paylocity/refs/heads/main/agentic-access/paylocity-agentic-access.yml
summary_line: 29 operations · 13 acting
tags:
- HR
- Payroll
- HCM
- Benefits
- Workforce Management
- Time Tracking
---
