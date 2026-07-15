---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 24
api_specs:
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Inquiries API
  slug: persona-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Inquiry Sessions API
  slug: persona-inquiry-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Accounts API
  slug: persona-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Verifications API
  slug: persona-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Reports API
  slug: persona-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Cases API
  slug: persona-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Transactions API
  slug: persona-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Devices API
  slug: persona-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Documents API
  slug: persona-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Webhooks API
  slug: persona-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Events API
  slug: persona-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Importers API
  slug: persona-importers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
- filename: withpersona-openapi.yml
  format: yaml
  label: Persona Workflows API
  slug: persona-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/openapi/withpersona-openapi.yml
consequence_counts:
  read: 24
  safety-critical: 1
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Withpersona Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /webhooks/{webhook-id}/disable
operation_count: 49
overview: 'Persona exposes 49 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 24 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Persona
provider_slug: withpersona
slug: withpersona-agentic-access
source_filename: withpersona-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/withpersona-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 24\n    acting: 25\n  by_consequence:\n    read: 24\n    write: 24\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /inquiries\n  method: get\n  operationId: listAllInquiries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inquiries\n  method: post\n  operationId: createInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inquiries/{inquiry-id}\n  method: get\n  operationId: retrieveInquiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inquiries/{inquiry-id}\n  method: patch\n  operationId: updateInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inquiries/{inquiry-id}/approve\n  method: post\n  operationId: approveInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /inquiries/{inquiry-id}/decline\n  method: post\n  operationId: declineInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inquiries/{inquiry-id}/mark-for-review\n  method: post\n  operationId: markInquiryForReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inquiries/{inquiry-id}/expire\n  method: post\n  operationId: expireInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inquiries/{inquiry-id}/resume\n  method: post\n  operationId: resumeInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inquiries/{inquiry-id}/generate-one-time-link\n  method: post\n  operationId: generateInquiryOneTimeLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inquiries/{inquiry-id}:redact\n  method: delete\n  operationId: redactInquiry\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inquiry-sessions\n  method: get\n  operationId: listAllInquirySessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inquiry-sessions\n  method: post\n  operationId: createInquirySession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inquiry-sessions/{inquiry-session-id}\n  method: get\n  operationId: retrieveInquirySession\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inquiry-sessions/{inquiry-session-id}/expire\n  method: post\n  operationId: expireInquirySession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: listAllAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /accounts/{account-id}\n  method: get\n  operationId: retrieveAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account-id}\n  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account-id}/consolidate\n  method: post\n  operationId: consolidateAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /verifications/{verification-id}\n  method: get\n  operationId: retrieveVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports\n  method: get\n  operationId: listAllReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports\n  method: post\n  operationId: createReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{report-id}\n  method: get\n  operationId: retrieveReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /cases\n  method: get\n  operationId: listAllCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cases\n  method: post\n  operationId: createCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases/{case-id}\n  method: get\n  operationId: retrieveCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cases/{case-id}\n  method: patch\n  operationId: updateCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases/{case-id}/assign\n  method: post\n  operationId: assignCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions\n  method: get\n  operationId: listAllTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /transactions/{transaction-id}\n  method: get\n  operationId: retrieveTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transaction-id}\n  method: patch\n  operationId: updateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices\n  method: get\n  operationId: listAllDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{device-id}\n  method: get\n  operationId: retrieveDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document-id}\n  method: get\n  operationId: retrieveDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listAllWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook-id}\n  method: get\n  operationId: retrieveWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook-id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook-id}/enable\n  method: post\n  operationId: enableWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook-id}/disable\n  method: post\n  operationId: disableWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /events\n  method: get\n  operationId: listAllEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event-id}\n  method: get\n  operationId: retrieveEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /importer\n  method: get\n  operationId: listAllImporters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /importer/{importer-id}\n  method: get\n  operationId: retrieveImporter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow-runs\n  method: get\n  operationId: listAllWorkflowRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow-runs\n  method: post\n  operationId: createWorkflowRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflow-runs/{workflow-run-id}\n  method: get\n  operationId: retrieveWorkflowRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withpersona/refs/heads/main/agentic-access/withpersona-agentic-access.yml
summary_line: 49 operations · 25 acting · 1 human-in-the-loop
tags:
- Identity
- Identity Verification
- KYC
- KYB
- AML
- Fraud
- Compliance
---
