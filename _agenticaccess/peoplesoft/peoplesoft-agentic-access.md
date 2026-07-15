---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 45
api_specs:
- filename: rest-api.yml
  format: yaml
  label: PeopleSoft REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/rest-api.yml
- filename: application-services-framework.yml
  format: yaml
  label: PeopleSoft Application Services Framework API
  slug: application-services-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/application-services-framework.yml
- filename: integration-broker.yml
  format: yaml
  label: PeopleSoft Integration Broker
  slug: integration-broker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/integration-broker.yml
- filename: query.yml
  format: yaml
  label: PeopleSoft Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/query.yml
- filename: component-interface.yml
  format: yaml
  label: PeopleSoft Component Interface API
  slug: component-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/component-interface.yml
- filename: search-framework.yml
  format: yaml
  label: PeopleSoft Search Framework API
  slug: search-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/search-framework.yml
- filename: notification-framework.yml
  format: yaml
  label: PeopleSoft Notification Framework API
  slug: notification-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/notification-framework.yml
- filename: chatbot-integration.yml
  format: yaml
  label: PeopleSoft Chatbot Integration Framework API
  slug: chatbot-integration-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/chatbot-integration.yml
- filename: approval-workflow-engine.yml
  format: yaml
  label: PeopleSoft Approval Workflow Engine API
  slug: approval-workflow-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/approval-workflow-engine.yml
- filename: process-scheduler.yml
  format: yaml
  label: PeopleSoft Process Scheduler API
  slug: process-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/process-scheduler.yml
- filename: cloud-manager.yml
  format: yaml
  label: PeopleSoft Cloud Manager API
  slug: cloud-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/cloud-manager.yml
- filename: update-manager.yml
  format: yaml
  label: PeopleSoft Update Manager API
  slug: update-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/update-manager.yml
- filename: pivot-grid.yml
  format: yaml
  label: PeopleSoft Pivot Grid API
  slug: pivot-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/pivot-grid.yml
- filename: hcm.yml
  format: yaml
  label: PeopleSoft HCM API
  slug: hcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/hcm.yml
- filename: recruiting-talent-management.yml
  format: yaml
  label: PeopleSoft Recruiting and Talent Management API
  slug: recruiting-and-talent-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/recruiting-talent-management.yml
- filename: financials.yml
  format: yaml
  label: PeopleSoft Financials API
  slug: financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/financials.yml
- filename: supply-chain-management.yml
  format: yaml
  label: PeopleSoft Supply Chain Management API
  slug: supply-chain-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/supply-chain-management.yml
- filename: crm.yml
  format: yaml
  label: PeopleSoft CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/crm.yml
- filename: campus-solutions.yml
  format: yaml
  label: PeopleSoft Campus Solutions API
  slug: campus-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/campus-solutions.yml
- filename: enterprise-performance-management.yml
  format: yaml
  label: PeopleSoft Enterprise Performance Management API
  slug: enterprise-performance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/enterprise-performance-management.yml
- filename: interaction-hub.yml
  format: yaml
  label: PeopleSoft Interaction Hub API
  slug: interaction-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/interaction-hub.yml
consequence_counts:
  physical: 3
  read: 45
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Peoplesoft Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /environments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fulfill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /notifications
operation_count: 60
overview: 'PeopleSoft exposes 60 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read, 12 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PeopleSoft
provider_slug: peoplesoft
slug: peoplesoft-agentic-access
source_filename: peoplesoft-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/application-services-framework.yml, openapi/approval-workflow-engine.yml, openapi/campus-solutions.yml,\n  openapi/chatbot-integration.yml, openapi/cloud-manager.yml, openapi/component-interface.yml,\n  openapi/crm.yml, openapi/enterprise-performance-management.yml, openapi/financials.yml, openapi/hcm.yml,\n  openapi/integration-broker.yml, openapi/interaction-hub.yml, openapi/notification-framework.yml,\n  openapi/pivot-grid.yml, openapi/process-scheduler.yml, openapi/query.yml, openapi/recruiting-talent-management.yml,\n  openapi/rest-api.yml, openapi/search-framework.yml, openapi/supply-chain-management.yml, openapi/update-manager.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations:\
  \ 60\n  by_action_class:\n    connected: 45\n    acting: 15\n  by_consequence:\n    read: 45\n    write: 12\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /{serviceName}\n  method: get\n  operationId: getServiceResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{serviceName}\n  method: post\n  operationId: createServiceResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /approvals\n  method: get\n  operationId: listPendingApprovals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /approvals/{approvalId}\n \
  \ method: put\n  operationId: processApproval\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /students\n  method: get\n  operationId: listStudents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /students/{studentId}\n  method: get\n  operationId: getStudent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admissions/applications\n  method: get\n  operationId: listAdmissionApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollment/classes\n\
  \  method: get\n  operationId: listClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financial-aid/awards\n  method: get\n  operationId: listFinancialAidAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intents\n  method: get\n  operationId: listIntents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fulfill\n  method: post\n  operationId: fulfillIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /environments\n  method: get\n  operationId: listEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments\n  method: post\n  operationId: provisionEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{componentInterface}\n  method: get\n  operationId: getComponentData\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{componentInterface}\n  method: post\n  operationId: createComponentData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{componentInterface}\n  method: put\n  operationId: updateComponentData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /customers/{customerId}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cases\n  method: get\n  operationId: listCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cases\n  method: post\n  operationId: createCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sales/opportunities\n  method: get\n  operationId: listOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /budgets\n  method: get\n  operationId: listBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecasts\n  method: get\n  operationId: listForecasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/reports\n  method: get\n  operationId: listAnalyticsReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gl/journals\n  method: get\n  operationId: listJournalEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap/vouchers\n  method: get\n  operationId: listVouchers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ar/items\n  method: get\n  operationId: listARItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expenses/reports\n  method: get\n  operationId: listExpenseReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}\n  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /benefits/enrollments\n  method: get\n  operationId: listBenefitEnrollments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payroll/runs\n  method: get\n  operationId: listPayrollRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{serviceOperation}.v1\n  method: get\n  operationId: getServiceOperation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{serviceOperation}.v1\n  method: post\n  operationId: postServiceOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content\n  method: get\n  operationId:\
  \ listContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content\n  method: post\n  operationId: createContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /branding/themes\n  method: get\n  operationId: listThemes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications\n  method: get\n  operationId: listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications\n  method: post\n  operationId: sendNotification\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /grids\n  method: get\n  operationId: listPivotGrids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grids/{gridId}/data\n  method: get\n  operationId: getPivotGridData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes\n  method: get\n  operationId: listProcesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes\n  method:\
  \ post\n  operationId: submitProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /processes/{processInstance}\n  method: get\n  operationId: getProcessStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries\n  method: get\n  operationId: listQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries/{queryName}\n  method: get\n  operationId: executeQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: get\n\
  \  operationId: searchJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}\n  method: get\n  operationId: getJobDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidates/applications\n  method: post\n  operationId: submitApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{resource}\n  method: get\n  operationId: getResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{resource}\n  method: post\n  operationId:\
  \ createResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /index\n  method: post\n  operationId: triggerIndexBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /procurement/requisitions\n  method: get\n  operationId: listRequisitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /procurement/purchase-orders\n  method: get\n  operationId: listPurchaseOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inventory/items\n  method: get\n  operationId: listInventoryItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /updates\n  method: get\n  operationId: listUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /updates/{updateId}/apply\n  method: post\n  operationId:\
  \ applyUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/agentic-access/peoplesoft-agentic-access.yml
summary_line: 60 operations · 15 acting
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
---
