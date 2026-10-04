---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 17
api_specs:
- filename: workday-advanced-compensation-bonus-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Bonus Plans API
  slug: workday-advanced-compensation-bonus-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-bonus-plans-api-openapi.yml
- filename: workday-advanced-compensation-compensation-budgets-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Budgets API
  slug: workday-advanced-compensation-compensation-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-budgets-api-openapi.yml
- filename: workday-advanced-compensation-compensation-grades-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Grades API
  slug: workday-advanced-compensation-compensation-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-grades-api-openapi.yml
- filename: workday-advanced-compensation-compensation-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Plans API
  slug: workday-advanced-compensation-compensation-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-plans-api-openapi.yml
- filename: workday-advanced-compensation-compensation-reviews-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Reviews API
  slug: workday-advanced-compensation-compensation-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-reviews-api-openapi.yml
- filename: workday-advanced-compensation-employee-compensation-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Employee Compensation API
  slug: workday-advanced-compensation-employee-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-employee-compensation-api-openapi.yml
- filename: workday-advanced-compensation-merit-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Merit Plans API
  slug: workday-advanced-compensation-merit-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-merit-plans-api-openapi.yml
- filename: workday-advanced-compensation-stock-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Stock Plans API
  slug: workday-advanced-compensation-stock-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-stock-plans-api-openapi.yml
- filename: workday-advanced-compensation-prompt-values-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Prompt Values API
  slug: workday-advanced-compensation-prompt-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-prompt-values-api-openapi.yml
- filename: workday-advanced-compensation-scorecardresults-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Scorecard Results API
  slug: workday-advanced-compensation-scorecardresults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-scorecardresults-api-openapi.yml
- filename: workday-advanced-compensation-scorecards-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Scorecards API
  slug: workday-advanced-compensation-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-scorecards-api-openapi.yml
- filename: workday-advanced-compensation-workers-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Workers API
  slug: workday-advanced-compensation-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-workers-api-openapi.yml
consequence_counts:
  physical: 1
  read: 17
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Workday Advanced Compensation Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workers/{ID}/requestOneTimePayment
operation_count: 25
overview: 'Workday Advanced Compensation exposes 25 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 7 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Workday Advanced Compensation
provider_slug: workday-advanced-compensation
slug: workday-advanced-compensation-agentic-access
source_filename: workday-advanced-compensation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: generated\nsource: openapi/workday-advanced-compensation-bonus-plans-api-openapi.yml, openapi/workday-advanced-compensation-compensation-budgets-api-openapi.yml,\n  openapi/workday-advanced-compensation-compensation-grades-api-openapi.yml, openapi/workday-advanced-compensation-compensation-plans-api-openapi.yml,\n  openapi/workday-advanced-compensation-compensation-reviews-api-openapi.yml, openapi/workday-advanced-compensation-employee-compensation-api-openapi.yml,\n  openapi/workday-advanced-compensation-merit-plans-api-openapi.yml, openapi/workday-advanced-compensation-prompt-values-api-openapi.yml,\n  openapi/workday-advanced-compensation-scorecardresults-api-openapi.yml, openapi/workday-advanced-compensation-scorecards-api-openapi.yml,\n  openapi/workday-advanced-compensation-stock-plans-api-openapi.yml, openapi/workday-advanced-compensation-workers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified\
  \ heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 17\n    acting: 8\n  by_consequence:\n    read: 17\n    write: 7\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /bonusPlans\n  method: get\n  operationId: listBonusPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compensationBudgets\n  method: get\n  operationId: listCompensationBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compensationGrades\n  method: get\n  operationId: listCompensationGrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /compensationGrades/{gradeId}\n  method: get\n  operationId: getCompensationGrade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compensationPlans\n  method: get\n  operationId: listCompensationPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compensationPlans/{planId}\n  method: get\n  operationId: getCompensationPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compensationReviews\n  method: get\n  operationId: listCompensationReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}/compensation\n\
  \  method: get\n  operationId: getEmployeeCompensation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}/compensation\n  method: post\n  operationId: submitCompensationChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meritPlans\n  method: get\n  operationId: listMeritPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /values/oneTimePaymentPlanGroup/oneTimePaymentPlan/\n  method: get\n  operationId: getValuesOneTimePaymentPlanGroupOneTimePaymentPlan\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecardResults\n  method: get\n  operationId: getScorecardResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecardResults\n  method: post\n  operationId: postScorecardResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scorecardResults/{ID}/scores/{subresourceID}\n  method: patch\n  operationId: patchScorecardResultsByIDScoresBySubresourceID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scorecardResults/{ID}\n  method: get\n  operationId: getScorecardResultsByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecardResults/{ID}\n  method: delete\n  operationId: deleteScorecardResultsByID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scorecards\n  method: get\n  operationId: getScorecards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards\n  method: post\n  operationId: postScorecards\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scorecards/{ID}\n  method: get\n  operationId: getScorecardsByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards/{ID}\n  method: put\n  operationId: putScorecardsByID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scorecards/{ID}\n  method: delete\n  operationId: deleteScorecardsByID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stockPlans\n  method: get\n  operationId: listStockPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers\n  method: get\n  operationId: getWorkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{ID}/requestOneTimePayment\n  method: post\n  operationId: postWorkersByIDRequestOneTimePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /workers/{ID}\n  method: get\n  operationId: getWorkersByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/agentic-access/workday-advanced-compensation-agentic-access.yml
summary_line: 25 operations · 8 acting
tags:
- Compensation
- Human Resources
- Payroll
- HCM
- Enterprise Software
- Total Rewards
- Bonus
- Merit
- Stock Compensation
- SOAP
- Software-as-a-Service
---
