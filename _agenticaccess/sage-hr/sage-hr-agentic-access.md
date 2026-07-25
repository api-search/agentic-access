---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 28
api_specs:
- filename: sage-hr-documents-api-openapi.yml
  format: yaml
  label: Sage HR Documents API
  slug: sage-hr-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-documents-api-openapi.yml
- filename: sage-hr-employee-api-openapi.yml
  format: yaml
  label: Sage HR Employee API
  slug: sage-hr-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-employee-api-openapi.yml
- filename: sage-hr-integrations-api-openapi.yml
  format: yaml
  label: Sage HR Integrations API
  slug: sage-hr-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-integrations-api-openapi.yml
- filename: sage-hr-kit-days-api-openapi.yml
  format: yaml
  label: Sage HR KIT days API
  slug: sage-hr-kit-days-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-kit-days-api-openapi.yml
- filename: sage-hr-leave-management-api-openapi.yml
  format: yaml
  label: Sage HR Leave management API
  slug: sage-hr-leave-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-leave-management-api-openapi.yml
- filename: sage-hr-offboarding-api-openapi.yml
  format: yaml
  label: Sage HR Offboarding API
  slug: sage-hr-offboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-offboarding-api-openapi.yml
- filename: sage-hr-onboarding-api-openapi.yml
  format: yaml
  label: Sage HR Onboarding API
  slug: sage-hr-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-onboarding-api-openapi.yml
- filename: sage-hr-performance-api-openapi.yml
  format: yaml
  label: Sage HR Performance API
  slug: sage-hr-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-performance-api-openapi.yml
- filename: sage-hr-policies-api-openapi.yml
  format: yaml
  label: Sage HR Policies API
  slug: sage-hr-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-policies-api-openapi.yml
- filename: sage-hr-positions-api-openapi.yml
  format: yaml
  label: Sage HR Positions API
  slug: sage-hr-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-positions-api-openapi.yml
- filename: sage-hr-recruitment-api-openapi.yml
  format: yaml
  label: Sage HR Recruitment API
  slug: sage-hr-recruitment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-recruitment-api-openapi.yml
- filename: sage-hr-teams-api-openapi.yml
  format: yaml
  label: Sage HR Teams API
  slug: sage-hr-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-teams-api-openapi.yml
- filename: sage-hr-terminations-reasons-api-openapi.yml
  format: yaml
  label: Sage HR Terminations reasons API
  slug: sage-hr-terminations-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-terminations-reasons-api-openapi.yml
- filename: sage-hr-timesheets-api-openapi.yml
  format: yaml
  label: Sage HR Timesheets API
  slug: sage-hr-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-timesheets-api-openapi.yml
consequence_counts:
  physical: 10
  read: 28
  safety-critical: 2
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Sage Hr Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /employees/{id}/terminations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vikarina/terminated-employees
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/appointments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/bank-accounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/bonuses
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/contract-information
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/job-positions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/leave-types
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/organization-structure
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/salaries
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/timesheets
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vikarina/unused-days
operation_count: 53
overview: 'Sage HR exposes 53 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 13 write, 10 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sage HR
provider_slug: sage-hr
slug: sage-hr-agentic-access
source_filename: sage-hr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sage-hr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 28\n    acting: 25\n  by_consequence:\n    read: 28\n    write: 13\n    safety-critical: 2\n    physical: 10\n  human_in_the_loop_required: 2\noperations:\n- path: /employees\n  method: get\n  operationId: Employee_listActiveEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees\n  method: post\n  operationId: Employee_createNewEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{id}\n  method: get\n  operationId: Employee_getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{id}\n  method: put\n  operationId: Employee_updateById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{id}/custom-fields\n  method: get\n  operationId: Employee_getCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{id}/custom-fields/{custom_field_id}\n\
  \  method: put\n  operationId: Employee_updateCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{id}/terminations\n  method: post\n  operationId: Employee_terminateEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /terminated-employees\n  method: get\n  operationId: Employee_listTerminatedEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /terminated-employees/{id}\n\
  \  method: get\n  operationId: Employee_getTerminatedEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leave-management/policies\n  method: get\n  operationId: LeaveManagement_listTimeOffPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leave-management/policies/{id}\n  method: get\n  operationId: LeaveManagement_getTimeOffPolicyById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leave-management/policies/{id}\n  method: patch\n  operationId: LeaveManagement_updateKitDaysConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leave-management/kit-days\n  method: get\n  operationId: LeaveManagement_getKitDays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leave-management/kit-days\n  method: post\n  operationId: LeaveManagement_createKitDay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leave-management/kit-days/{id}\n  method: patch\n  operationId: LeaveManagement_processKitDay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leave-management/reports/individual-allowances\n  method: get\n  operationId: LeaveManagement_getIndividualAllowances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{id}/leave-management/balances\n  method: get\n  operationId: LeaveManagement_getTimeOffBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leave-management/requests\n  method: get\n  operationId: LeaveManagement_listTimeOffRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leave-management/requests\n  method: post\n  operationId: LeaveManagement_newTimeOffRequest\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leave-management/out-of-office-today\n  method: get\n  operationId: LeaveManagement_listEmployeesOutToday\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/categories\n  method: get\n  operationId: Documents_listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: post\n  operationId: Documents_createNewDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /positions\n  method: get\n  operationId: Positions_listCompanyPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: get\n  operationId: Teams_listInCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance/goals/quarterly-progress/overall\n  method: get\n  operationId: Performance_overviewQuarterlyProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance/goals/quarterly-progress/company-goals\n  method: get\n  operationId: Performance_getQuarterlyCompanyGoals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance/goals/quarterly-progress/team-goals\n  method: get\n  operationId: Performance_getQuarterlyTeamGoals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance/goals/quarterly-progress/individual-goals\n  method: get\n  operationId: Performance_getQuarterlyIndividualGoals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{id}/compensations\n  method: get\n  operationId: Employee_getCompensations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recruitment/positions\n  method: get\n  operationId: Recruitment_listPositions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recruitment/positions/{id}\n  method: get\n  operationId: Recruitment_getPositionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recruitment/positions/{id}/applicants\n  method: get\n  operationId: Recruitment_listApplicants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recruitment/positions/{id}/applicants\n  method: post\n  operationId: Recruitment_createApplicantWithReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recruitment/applicants/{id}\n\
  \  method: get\n  operationId: Recruitment_getApplicantDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recruitment/applicants/{id}/actions\n  method: get\n  operationId: Recruitment_listApplicantActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timesheets/clock-in\n  method: post\n  operationId: Timesheets_clockInOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /termination-reasons\n  method: get\n  operationId: TerminationsReasons_listInCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding/categories\n  method: get\n  operationId: Onboarding_listTaskCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding/tasks\n  method: post\n  operationId: Onboarding_createNewTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /offboarding/categories\n  method: get\n  operationId: Offboarding_listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offboarding/tasks\n  method: post\n  operationId: Offboarding_createTask\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vikarina/job-positions\n  method: post\n  operationId: Integrations_transferJobPositionFromSageToVikarina\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vikarina/organization-structure\n  method: post\n  operationId: Integrations_transferOrganizationalStructureFromSageToVikarina\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vikarina/newstarter-employees\n  method: post\n  operationId: Integrations_importNewStartersList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vikarina/contract-information\n  method: post\n  operationId: Integrations_transferContractInformationToVikarina\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /vikarina/appointments\n  method: post\n  operationId: Integrations_transferAppointmentInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vikarina/salaries\n  method: post\n  operationId: Integrations_transferSalaryInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vikarina/bank-accounts\n  method: post\n  operationId: Integrations_transferBankAccountInfo\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vikarina/terminated-employees\n  method: post\n  operationId: Integrations_transferTerminationInfoToVikarina\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /vikarina/unused-days\n  method: post\n  operationId: Integrations_transferUnusedVacationDaysToVikarina\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vikarina/leave-types\n  method: post\n  operationId: Integrations_transferLeaveInformationToVikarina\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vikarina/timesheets\n  method: post\n  operationId: Integrations_transferTimeScheduleInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /vikarina/bonuses\n  method: post\n  operationId: Integrations_sendBonusesToVikarina\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/agentic-access/sage-hr-agentic-access.yml
summary_line: 53 operations · 25 acting · 2 human-in-the-loop
tags:
- HR
- HRIS
- People
- SMB
- Leave Management
- Recruitment
- Performance
- Timesheets
- Onboarding
---
