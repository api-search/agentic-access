---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 17
api_specs:
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Companies API
  slug: zeal-hq-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Employees API
  slug: zeal-hq-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Contractors API
  slug: zeal-hq-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Employee Check (Payroll Run) API
  slug: zeal-hq-employee-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Contractor Payments API
  slug: zeal-hq-contractor-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Pay Schedules API
  slug: zeal-hq-pay-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Worker Onboarding API
  slug: zeal-hq-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Tax and Compliance API
  slug: zeal-hq-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Reports API
  slug: zeal-hq-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Funding and Journal API
  slug: zeal-hq-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
- filename: zeal-hq-openapi.yml
  format: yaml
  label: Zeal Webhooks and Events API
  slug: zeal-hq-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/openapi/zeal-hq-openapi.yml
consequence_counts:
  physical: 4
  read: 17
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zeal Hq Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contractorPayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /contractorPayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /contractorPayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contractorPayments/disburse
operation_count: 36
overview: 'Zeal exposes 36 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 15 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zeal
provider_slug: zeal-hq
slug: zeal-hq-agentic-access
source_filename: zeal-hq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zeal-hq-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 19\n    connected: 17\n  by_consequence:\n    write: 15\n    read: 17\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /companies\n  method: post\n  operationId: createCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies\n  method: get\n  operationId: getCompanyInformation\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies\n  method: put\n  operationId: updateCompanyInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/onboard\n  method: get\n  operationId: getCompanyOnboardingLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bankAccount\n  method: post\n  operationId: createCompanyBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /employees\n  method: post\n  operationId: createEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees\n  method: get\n  operationId: getEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees\n  method: put\n  operationId: updateEmployeeInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/onboarding\n  method: get\n  operationId:\
  \ generateEmployeeOnboardingLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /taxes/employee/setup\n  method: post\n  operationId: setEmployeeTaxParameters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /taxes/employee/definitions\n  method: get\n  operationId: getEmployeeTaxParameterDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contractors\n  method: post\n  operationId: createContractor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contractors\n  method: get\n  operationId: getContractors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contractors\n  method: put\n  operationId: updateContractorInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contractors/onboard\n  method: get\n  operationId: getContractorOnboardingLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employeeCheck\n  method: post\n  operationId:\
  \ createEmployeeCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employeeCheck\n  method: get\n  operationId: getEmployeeChecksByEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employeeCheck\n  method: put\n  operationId: updateEmployeeCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employeeCheck\n  method: delete\n  operationId: deleteEmployeeCheck\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employeeCheck/bulk\n  method: post\n  operationId: createBulkEmployeeChecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paystub\n  method: get\n  operationId: downloadPaystubPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contractorPayments\n  method: post\n  operationId: createContractorPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contractorPayments\n  method: get\n  operationId: getContractorPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contractorPayments\n  method: put\n  operationId: updateContractorPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contractorPayments\n  method: delete\n  operationId: deleteContractorPayment\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contractorPayments/disburse\n  method: post\n  operationId: triggerContractorDisbursement\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reportingPeriods\n  method: get\n  operationId: getAllReportingPeriods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reportingPeriods/upcoming\n  method: get\n  operationId:\
  \ getUpcomingRegularPayroll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkDate\n  method: get\n  operationId: getNextAvailableCheckDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /taxes/location\n  method: post\n  operationId: resolveTaxableLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /minimumWage\n  method: get\n  operationId: getMinimumWageRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/payrollJournal\n\
  \  method: post\n  operationId: createPayrollJournalReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/cashRequirements\n  method: post\n  operationId: createCashRequirementsReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/status\n  method: get\n  operationId: getReportJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/download\n  method: get\n  operationId: retrieveReportDownload\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reserve/balance\n  method: get\n  operationId: getReserveBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeal-hq/refs/heads/main/agentic-access/zeal-hq-agentic-access.yml
summary_line: 36 operations · 19 acting
tags:
- Payroll
- Embedded Finance
- Fintech
- Tax Compliance
- Contractors
- Human Resources
---
