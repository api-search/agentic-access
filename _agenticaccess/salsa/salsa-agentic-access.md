---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 17
api_specs:
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Companies API
  slug: salsa-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Workers API
  slug: salsa-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Pay Schedules API
  slug: salsa-pay-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Payrolls API
  slug: salsa-payrolls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Payments API
  slug: salsa-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Onboarding & Sessions API
  slug: salsa-onboarding-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Tax API
  slug: salsa-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
- filename: salsa-openapi.yml
  format: yaml
  label: Salsa Webhooks API
  slug: salsa-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/openapi/salsa-openapi.yml
consequence_counts:
  physical: 3
  read: 17
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Salsa Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /employers/{employerId}/workers/{workerId}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /employers/{employerId}/workers/{workerId}/payments/{paymentId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /employers/{employerId}/workers/{workerId}/payments/{paymentId}/deductions
operation_count: 42
overview: 'Salsa exposes 42 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 22 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Salsa
provider_slug: salsa
slug: salsa-agentic-access
source_filename: salsa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/salsa-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 25\n    connected: 17\n  by_consequence:\n    write: 22\n    read: 17\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /employers\n  method: post\n  operationId: createEmployer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers\n  method: get\n  operationId: listEmployers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}\n  method: get\n  operationId: getEmployer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}\n  method: patch\n  operationId: updateEmployer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}\n  method: delete\n  operationId: deleteEmployer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /employers/{employerId}/pay-types\n  method: get\n  operationId: listPayTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/pay-types\n  method: post\n  operationId: createPayType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/bank-accounts\n  method: get\n  operationId: listEmployerBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/bank-accounts\n  method: post\n  operationId: createEmployerBankAccount\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/workers\n  method: post\n  operationId: createWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/workers\n  method: get\n  operationId: listWorkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/workers/{workerId}\n  method: get\n  operationId: getWorker\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/workers/{workerId}\n  method: patch\n  operationId: updateWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/workers/{workerId}\n  method: delete\n  operationId: deleteWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/workers/{workerId}/contracts\n  method: get\n  operationId: listWorkerContracts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/workers/{workerId}/contracts\n  method: post\n  operationId: createWorkerContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/workers/{workerId}/bank-accounts\n  method: get\n  operationId: listWorkerBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/workers/{workerId}/bank-accounts\n  method: post\n  operationId: createWorkerBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/worker-pay-groups\n  method: get\n  operationId: listWorkerPayGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/worker-pay-groups\n  method: post\n  operationId: createWorkerPayGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/work-weeks\n  method: get\n  operationId: listWorkWeeks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /employers/{employerId}/work-weeks\n  method: post\n  operationId: createWorkWeek\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/payroll-runs\n  method: post\n  operationId: createPayrollRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/payroll-runs\n  method: get\n  operationId: listPayrollRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/payroll-runs/{payrollRunId}\n\
  \  method: get\n  operationId: getPayrollRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/payroll-runs/{payrollRunId}\n  method: delete\n  operationId: deletePayrollRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/payroll-runs/{payrollRunId}/preview\n  method: post\n  operationId: previewPayrollRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/payroll-runs/{payrollRunId}/confirm\n\
  \  method: post\n  operationId: confirmPayrollRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/reports/payroll-journal\n  method: get\n  operationId: getPayrollJournalReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/workers/{workerId}/payments\n  method: post\n  operationId: createWorkerPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /employers/{employerId}/workers/{workerId}/payments\n  method: get\n  operationId: listWorkerPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employers/{employerId}/workers/{workerId}/payments/{paymentId}/confirm\n  method: post\n  operationId: confirmWorkerPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/workers/{workerId}/payments/{paymentId}/deductions\n  method: post\n  operationId: createPaymentDeduction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-tokens\n  method: post\n  operationId: createUserToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/hosted-onboardings\n  method: post\n  operationId: createHostedEmployerOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/mock-onboard\n\
  \  method: post\n  operationId: mockOnboardEmployer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/workers/mock-onboard\n  method: post\n  operationId: mockOnboardWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employers/{employerId}/taxes-setup\n  method: get\n  operationId: getEmployerTaxSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-endpoints\n  method: post\n  operationId:\
  \ createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-endpoints/{webhookEndpointId}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-endpoints/{webhookEndpointId}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salsa/refs/heads/main/agentic-access/salsa-agentic-access.yml
summary_line: 42 operations · 25 acting
tags:
- Payroll
- Embedded Finance
- Payroll as a Service
- Fintech
- Payments
- HR
- Tax
- Multi-Country
---
