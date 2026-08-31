---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 10
api_specs:
- filename: justt-chargebacks-api-openapi.yml
  format: yaml
  label: Justt Chargebacks API
  slug: justt-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-chargebacks-api-openapi.yml
- filename: justt-data-subjects-api-openapi.yml
  format: yaml
  label: Justt Data Subjects API
  slug: justt-data-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-data-subjects-api-openapi.yml
- filename: justt-evidence-api-openapi.yml
  format: yaml
  label: Justt Evidence API
  slug: justt-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-evidence-api-openapi.yml
- filename: justt-files-api-openapi.yml
  format: yaml
  label: Justt Files API
  slug: justt-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-files-api-openapi.yml
- filename: justt-integrations-api-openapi.yml
  format: yaml
  label: Justt Integrations API
  slug: justt-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-integrations-api-openapi.yml
- filename: justt-merchants-api-openapi.yml
  format: yaml
  label: Justt Merchants API
  slug: justt-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-merchants-api-openapi.yml
- filename: justt-pre-chargeback-alerts-api-openapi.yml
  format: yaml
  label: Justt Pre-chargeback Alerts API
  slug: justt-pre-chargeback-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-pre-chargeback-alerts-api-openapi.yml
- filename: justt-sandbox-api-openapi.yml
  format: yaml
  label: Justt Sandbox API
  slug: justt-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-sandbox-api-openapi.yml
- filename: justt-transactions-api-openapi.yml
  format: yaml
  label: Justt Transactions API
  slug: justt-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-transactions-api-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 13
kind: agentic-access
layout: agentic-access
method: generated
name: Justt Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /chargebacks/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /chargebacks/{id}/accept
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /chargebacks/{id}/evidence/submit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /chargebacks/{id}/should-fight
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /data-subjects/removal
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /files
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /integrations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /integrations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /merchants
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /merchants
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pre-chargeback-alerts/alerts/outcome
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sandbox/raw-data
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /transactions
operation_count: 23
overview: 'Justt exposes 23 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 13 safety-critical.


  13 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Justt
provider_slug: justt
slug: justt-agentic-access
source_filename: justt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: generated\nsource: openapi/justt-pre-chargeback-alerts-openapi-original.json, openapi/justt-rest-api-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 10\n    acting: 13\n  by_consequence:\n    read: 10\n    safety-critical: 13\n  human_in_the_loop_required: 13\noperations:\n- path: /pre-chargeback-alerts/alerts\n  method: get\n  operationId: AlertController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pre-chargeback-alerts/alerts/{internalAlertId}\n  method: get\n  operationId: AlertController_findOne\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: post\n  operationId: TransactionController_createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chargebacks\n  method: get\n  operationId: ChargebackController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chargebacks/{id}\n  method: get\n  operationId: ChargebackItemController_getChargeback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chargebacks/{id}\n\
  \  method: patch\n  operationId: ChargebackItemController_updateChargeback\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chargebacks/{id}/should-fight\n  method: patch\n  operationId: ChargebackItemController_markShouldFight\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chargebacks/{id}/accept\n  method: post\n  operationId: ChargebackItemController_acceptChargeback\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chargebacks/{id}/accept\n  method: get\n  operationId: ChargebackItemController_getAcceptChargebackStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chargebacks/{id}/evidence/submit\n  method: post\n  operationId: EvidenceController_submitEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chargebacks/{id}/evidence/submit/{submitEvidenceId}\n  method: get\n  operationId:\
  \ EvidenceController_getEvidenceSubmissionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: FilesController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /data-subjects/removal\n  method: post\n  operationId: DataSubjectsController_requestDataSubjectRemoval\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /merchants\n  method: get\n  operationId: MerchantsController_getMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants\n  method: delete\n  operationId: MerchantsController_deactivateMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /merchants\n  method: post\n  operationId: MerchantsController_createMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /merchants/{merchantUuid}\n  method: get\n  operationId: MerchantsController_getMerchant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations\n  method: get\n  operationId: IntegrationsController_getIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations\n  method: post\n  operationId: IntegrationsController_createIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /integrations/{id}\n  method: get\n  operationId: IntegrationsController_getIntegration\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/{id}\n  method: delete\n  operationId: IntegrationsController_deactivateIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pre-chargeback-alerts/alerts/outcome\n  method: post\n  operationId: PreChargebackAlertsController_createOutcome\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /sandbox/raw-data\n  method: post\n  operationId: SandboxController_uploadRawData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/agentic-access/justt-agentic-access.yml
summary_line: 23 operations · 13 acting · 13 human-in-the-loop
tags:
- Company
- Payments
- Chargebacks
- Disputes
- Fraud
- Risk
- Financial-Services
- E-Commerce
- Artificial Intelligence
- Webhook
---
