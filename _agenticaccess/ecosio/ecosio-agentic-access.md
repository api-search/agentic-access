---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 19
api_specs:
- filename: ecosio-approval-request-status-api-openapi.yml
  format: yaml
  label: ecosio Approval Request Status API
  slug: ecosio-approval-request-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-approval-request-status-api-openapi.yml
- filename: ecosio-archive-messages-api-openapi.yml
  format: yaml
  label: ecosio Archive messages API
  slug: ecosio-archive-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-archive-messages-api-openapi.yml
- filename: ecosio-check-user-credentials-api-openapi.yml
  format: yaml
  label: ecosio Check user credentials API
  slug: ecosio-check-user-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-check-user-credentials-api-openapi.yml
- filename: ecosio-companies-api-openapi.yml
  format: yaml
  label: ecosio Companies API
  slug: ecosio-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-companies-api-openapi.yml
- filename: ecosio-connectors-api-openapi.yml
  format: yaml
  label: ecosio Connectors API
  slug: ecosio-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-connectors-api-openapi.yml
- filename: ecosio-deliver-messages-to-the-hub-api-openapi.yml
  format: yaml
  label: ecosio Deliver messages to the Hub API
  slug: ecosio-deliver-messages-to-the-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-deliver-messages-to-the-hub-api-openapi.yml
- filename: ecosio-fetch-messages-from-the-hub-api-openapi.yml
  format: yaml
  label: ecosio Fetch messages from the Hub API
  slug: ecosio-fetch-messages-from-the-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-fetch-messages-from-the-hub-api-openapi.yml
- filename: ecosio-message-controller-api-openapi.yml
  format: yaml
  label: ecosio Message Controller API
  slug: ecosio-message-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-message-controller-api-openapi.yml
- filename: ecosio-request-the-documents-for-an-e-invoice-api-openapi.yml
  format: yaml
  label: ecosio Request the documents for an e-invoice API
  slug: ecosio-request-the-documents-for-an-e-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-request-the-documents-for-an-e-invoice-api-openapi.yml
- filename: ecosio-scenarios-api-openapi.yml
  format: yaml
  label: ecosio Scenarios API
  slug: ecosio-scenarios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-scenarios-api-openapi.yml
consequence_counts:
  read: 19
  safety-critical: 2
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Ecosio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/messages
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/messages/{messageId}/confirm
operation_count: 32
overview: 'ecosio exposes 32 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 11 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ecosio
provider_slug: ecosio
slug: ecosio-agentic-access
source_filename: ecosio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/ecosio-api-openapi.yml, openapi/ecosio-management-api-openapi.yml, openapi/ecosio-vertex-messaging-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 19\n    acting: 13\n  by_consequence:\n    read: 19\n    write: 11\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /api/v1/ack/{messageId}\n  method: get\n  operationId: getAcknowledgement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/archives\n  method: post\n  operationId: create-archive\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/archives/{archiveId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/callback/{messageId}\n  method: post\n  operationId: callback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/delivery\n  method: post\n  operationId: deliverMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/delivery/{messageId}\n  method: get\n  operationId: getStatusOfDeliveredMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{messageId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/downloads/{archiveId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fetch\n  method: get\n  operationId: getMessageList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/msg/{messageId}\n\
  \  method: get\n  operationId: getReceivedMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/securityCredentials\n  method: get\n  operationId: securityCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/management/approvals/{approvalUuid}\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/management/companies\n  method: post\n  operationId: createCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/management/companies\n  method: get\n  operationId: findCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/management/companies/{companyUuid}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/management/companies/{companyUuid}\n  method: put\n  operationId: updateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/management/companies/{companyUuid}/scenarios\n  method: post\n  operationId: createScenario\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/management/companies/{companyUuid}/scenarios\n  method: get\n  operationId: listAppliedScenarios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/management/connectors\n  method: post\n  operationId: createConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/management/connectors\n  method: get\n  operationId: findConnectors\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/management/connectors/{connectorUuid}\n  method: get\n  operationId: getConnector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/management/connectors/{connectorUuid}\n  method: put\n  operationId: updateConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/management/connectors/{connectorUuid}/companies\n  method: put\n  operationId: replaceCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/management/connectors/{connectorUuid}/regenerateCredentials\n  method: post\n  operationId: regenerateCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/management/scenarios\n  method: get\n  operationId: listAvailableScenarios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/management/scenarios/{scenarioUuid}\n  method: get\n  operationId: getScenarioById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/management/scenarios/{scenarioUuid}\n  method: put\n  operationId: updateScenario\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/messages\n  method: get\n  operationId: getMessageList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/messages/{messageId}\n\
  \  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/messages/{messageId}/confirm\n  method: post\n  operationId: confirm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/messages/{messageId}/documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ecosio/agentic-access/ecosio-agentic-access.yml
summary_line: 32 operations · 13 acting · 2 human-in-the-loop
tags:
- Company
- EDI
- E-Invoicing
- B2B Integration
- VAT Compliance
- PEPPOL
- Supply Chain
- Messaging
---
