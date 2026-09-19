---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 18
api_specs:
- filename: clari-activity-api-api-openapi.yml
  format: yaml
  label: Clari Activity API
  slug: clari-activity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-activity-api-api-openapi.yml
- filename: clari-administrative-api-api-openapi.yml
  format: yaml
  label: Clari Administrative API
  slug: clari-administrative-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-administrative-api-api-openapi.yml
- filename: clari-audit-api-api-openapi.yml
  format: yaml
  label: Clari Audit API
  slug: clari-audit-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-audit-api-api-openapi.yml
- filename: clari-bulk-export-framework-api-openapi.yml
  format: yaml
  label: Clari Bulk Export Framework API
  slug: clari-bulk-export-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-export-framework-api-openapi.yml
- filename: clari-bulk-ingest-job-status-api-api-openapi.yml
  format: yaml
  label: Clari Bulk Ingest Job Status API
  slug: clari-bulk-ingest-job-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-bulk-ingest-job-status-api-api-openapi.yml
- filename: clari-forecast-api-api-openapi.yml
  format: yaml
  label: Clari Forecast API
  slug: clari-forecast-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-forecast-api-api-openapi.yml
- filename: clari-ingestion-api-api-openapi.yml
  format: yaml
  label: Clari Ingestion API
  slug: clari-ingestion-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-ingestion-api-api-openapi.yml
- filename: clari-opportunity-api-api-openapi.yml
  format: yaml
  label: Clari Opportunity API
  slug: clari-opportunity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-opportunity-api-api-openapi.yml
- filename: clari-account-api-openapi.yml
  format: yaml
  label: Clari Account API
  slug: clari-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-account-api-openapi.yml
- filename: clari-call-api-openapi.yml
  format: yaml
  label: Clari Call API
  slug: clari-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-call-api-openapi.yml
- filename: clari-contact-api-openapi.yml
  format: yaml
  label: Clari Contact API
  slug: clari-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-contact-api-openapi.yml
- filename: clari-deal-api-openapi.yml
  format: yaml
  label: Clari Deal API
  slug: clari-deal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-deal-api-openapi.yml
- filename: clari-scorecard-api-openapi.yml
  format: yaml
  label: Clari Scorecard API
  slug: clari-scorecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-scorecard-api-openapi.yml
- filename: clari-topics-api-openapi.yml
  format: yaml
  label: Clari Topics API
  slug: clari-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-topics-api-openapi.yml
- filename: clari-user-api-openapi.yml
  format: yaml
  label: Clari User API
  slug: clari-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/openapi/clari-user-api-openapi.yml
consequence_counts:
  read: 18
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Clari Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /export/jobs/{jobId}
operation_count: 35
overview: 'Clari exposes 35 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 16 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clari
provider_slug: clari
slug: clari-agentic-access
source_filename: clari-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/clari-account-api-openapi.yml, openapi/clari-activity-api-api-openapi.yml, openapi/clari-administrative-api-api-openapi.yml,\n  openapi/clari-audit-api-api-openapi.yml, openapi/clari-bulk-export-framework-api-openapi.yml,\n  openapi/clari-bulk-ingest-job-status-api-api-openapi.yml, openapi/clari-call-api-openapi.yml,\n  openapi/clari-contact-api-openapi.yml, openapi/clari-deal-api-openapi.yml, openapi/clari-forecast-api-api-openapi.yml,\n  openapi/clari-ingestion-api-api-openapi.yml, openapi/clari-opportunity-api-api-openapi.yml,\n  openapi/clari-scorecard-api-openapi.yml, openapi/clari-topics-api-openapi.yml, openapi/clari-user-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations:\
  \ 35\n  by_action_class:\n    acting: 17\n    connected: 18\n  by_consequence:\n    write: 16\n    read: 18\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /create-account\n  method: post\n  operationId: postCreateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-account\n  method: get\n  operationId: getGetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update-account\n  method: put\n  operationId: putUpdateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-account\n  method: delete\n  operationId: deleteDeleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /export/activity\n  method: post\n  operationId: postExportActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/limits\n  method: get\n  operationId: limits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /export/audit/events\n  method: post\n  operationId: exportAuditEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audit/events\n  method: get\n  operationId: listAuditEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/jobs/{jobId}\n  method: get\n  operationId: jobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/jobs/{jobId}\n  method: patch\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /export/jobs/{jobId}/results\n  method: get\n  operationId: externalExportDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/jobs\n  method: get\n  operationId: externalFcwExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ingest/job/{jobId}\n  method: get\n  operationId: ingestJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls\n  method: get\n  operationId: getCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /call-details\n  method: get\n  operationId: getCallDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /create-call\n  method: post\n  operationId: postCreateCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create-contact\n  method: post\n  operationId: postCreateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-contact\n  method: get\n\
  \  operationId: getGetContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update-contact\n  method: put\n  operationId: putUpdateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-contact\n  method: delete\n  operationId: deleteDeleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create-deal\n  method: post\n  operationId: postCreateDeal\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-deal\n  method: get\n  operationId: getGetDeal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update-deal\n  method: put\n  operationId: putUpdateDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete-deal\n  method: delete\n  operationId: deleteDeleteDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /export/forecast/{forecastId}\n  method: post\n  operationId: externalFcwExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingest/bulk/entity/{entity}\n  method: post\n  operationId: ingestBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingest/entity/{entity}\n  method: post\n  operationId: ingestIncremental\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingest/schema/{entity}/field\n  method: post\n  operationId: ingestAddPicklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingest/schema/{entity}/field\n  method: get\n  operationId: ingestGetPicklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunity\n  method: get\n  operationId: externalOpportunityResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /scorecard\n  method: get\n  operationId: getScorecard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecard-template\n  method: get\n  operationId: getScorecardTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topics\n  method: get\n  operationId: getTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/topics\n  method: get\n  operationId: getV2Topics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clari/refs/heads/main/agentic-access/clari-agentic-access.yml
summary_line: 35 operations · 17 acting · 1 human-in-the-loop
tags:
- Revenue Operations
- Forecasting
- Pipeline Management
- Sales Intelligence
- Activity Intelligence
- Deal Insights
- CRM
- Conversation Intelligence
- B2B
- Enterprise
- MCP
- Agents
- Sales Engagement
- Bulk Export
- Data Ingestion
---
