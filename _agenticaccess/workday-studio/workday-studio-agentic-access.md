---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 11
api_specs:
- filename: workday-studio-integration-openapi.yml
  format: yaml
  label: Workday Studio Integration API
  slug: workday-studio-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-openapi.yml
- filename: workday-studio-web-services-openapi.yml
  format: yaml
  label: Workday Web Services API
  slug: workday-web-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-web-services-openapi.yml
consequence_counts:
  read: 11
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Workday Studio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Workday Studio exposes 22 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Workday Studio
provider_slug: workday-studio
slug: workday-studio-agentic-access
source_filename: workday-studio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/workday-studio-integration-openapi.yml, openapi/workday-studio-web-services-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 11\n    acting: 11\n  by_consequence:\n    read: 11\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /integrationSystems\n  method: get\n  operationId: listIntegrationSystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /integrationSystems/{ID}\n  method: get\n  operationId: getIntegrationSystem\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /integrationSystems/{ID}/launch\n  method: post\n  operationId: launchIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /integrationEvents\n  method: get\n  operationId: listIntegrationEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /integrationEvents/{ID}\n  method: get\n  operationId: getIntegrationEvent\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /integrationEvents/{ID}/logs\n  method: get\n  operationId: getIntegrationEventLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /integrationAssemblies\n  method: get\n  operationId: listIntegrationAssemblies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /integrationAssemblies/{ID}\n  method: get\n  operationId: getIntegrationAssembly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n\
  \    - w:integrations\n- path: /integrationTemplates\n  method: get\n  operationId: listIntegrationTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /integrationTemplates/{ID}\n  method: get\n  operationId: getIntegrationTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /launchParameters\n  method: get\n  operationId: listLaunchParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:integrations\n    - w:integrations\n- path: /Human_Resources\n  method: get\n  operationId: getHumanResourcesService\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - r:wws\n    - w:wws\n- path: /Human_Resources/Get_Workers\n  method: post\n  operationId: getWorkers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n- path: /Human_Resources/Get_Organizations\n  method: post\n  operationId: getOrganizations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n- path: /Financial_Management/Get_Journal_Entries\n\
  \  method: post\n  operationId: getJournalEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n- path: /Payroll/Get_Payroll_Results\n  method: post\n  operationId: getPayrollResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n- path: /Benefits_Administration/Get_Benefit_Plans\n  method: post\n  operationId: getBenefitPlans\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n- path: /Absence_Management/Get_Absence_Inputs\n  method: post\n  operationId: getAbsenceInputs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n- path: /Staffing/Get_Job_Postings\n  method: post\n  operationId: getJobPostings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n- path:\
  \ /Recruiting/Get_Candidates\n  method: post\n  operationId: getCandidates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n- path: /Compensation/Get_Compensation_Plans\n  method: post\n  operationId: getCompensationPlans\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n- path: /Time_Tracking/Get_Time_Clock_Events\n  method: post\n  operationId: getTimeClockEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - r:wws\n    - w:wws\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/agentic-access/workday-studio-agentic-access.yml
summary_line: 22 operations · 11 acting
tags:
- Cloud
- Development
- Enterprise
- Finance
- HR
- IDE
- Integration
---
