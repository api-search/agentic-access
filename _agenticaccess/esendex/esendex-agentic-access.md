---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 6
api_specs:
- filename: esendex-credential-management-api-openapi.yml
  format: yaml
  label: Esendex Credential Management API
  slug: esendex-credential-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/openapi/esendex-credential-management-api-openapi.yml
- filename: esendex-message-dispatcher-api-openapi.yml
  format: yaml
  label: Esendex Message Dispatcher API
  slug: esendex-message-dispatcher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/openapi/esendex-message-dispatcher-api-openapi.yml
- filename: esendex-message-headers-api-openapi.yml
  format: yaml
  label: Esendex Message Headers API
  slug: esendex-message-headers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/openapi/esendex-message-headers-api-openapi.yml
consequence_counts:
  physical: 3
  read: 6
  safety-critical: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Esendex Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1.0/messagedispatcher
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1.1/messagedispatcher
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/credentials/account/{accountReference}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/credentials/{credentialId}/sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/credentials/{credentialId}/sessions
operation_count: 16
overview: 'Esendex exposes 16 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 5 write, 3 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Esendex
provider_slug: esendex
slug: esendex-agentic-access
source_filename: esendex-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/esendex-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 10\n    connected: 6\n  by_consequence:\n    write: 5\n    read: 6\n    physical: 3\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/credentials/{credentialId}\n  method: patch\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesUpdateCredentialUpdateCredentialEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/credentials/{credentialId}\n  method: get\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesGetCredentialsSingleGetCredentialEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credentials/{credentialId}\n  method: delete\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesDeleteCredentialDeleteCredentialEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials/{credentialId}/sessions\n  method: get\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesGetSessionsGetSessionsEndpoint\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credentials/{credentialId}/sessions\n  method: delete\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesDeleteSessionsDeleteSessionsEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials/{credentialId}/sessions\n  method: post\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesCreateSessionsCreateSessionsEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials\n  method: get\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesGetCredentialsManyGetCredentialsEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credentials\n  method: post\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesCreateCredentialCreateCredentialEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials/{credentialId}/sessions/{sessionId}\n  method: delete\n  operationId:\
  \ TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesDeleteSessionByIdDeleteSessionByIdEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials/account/{accountReference}/sessions\n  method: delete\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesDeleteSessionByAccountIdDeleteSessionsByAccountIdEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credentials/account/{accountReference}\n  method: delete\n  operationId: TitanAPIAuthServiceEmulationFrameworkCredentialManagementUseCasesDeleteAllCredentialsDeleteAllCredentialsEndpoint\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/messagedispatcher\n  method: post\n  operationId: TitanCustomerUpgradesEmulationEsendexUseCasesSendMessageApiEsendexSendMessageV10Endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1.1/messagedispatcher\n  method: post\n  operationId: TitanCustomerUpgradesEmulationEsendexUseCasesSendMessageApiEsendexSendMessageV11Endpoint\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1.0/messageheaders/{messageId}/body\n  method: get\n  operationId: TitanCustomerUpgradesEmulationEsendexUseCasesGetMessageBodyApiEsendexGetMessageBodyEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/messageheaders/{messageId}\n  method: get\n  operationId: TitanCustomerUpgradesEmulationEsendexUseCasesGetMessageApiEsendexGetMessageEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/messageheaders\n  method: get\n  operationId: TitanCustomerUpgradesEmulationEsendexUseCasesGetAllMessagesApiEsendexGetAllMessagesEndpoint\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/agentic-access/esendex-agentic-access.yml
summary_line: 16 operations · 10 acting · 2 human-in-the-loop
tags:
- SMS
- Messaging
- Communications
- API
- Business
---
