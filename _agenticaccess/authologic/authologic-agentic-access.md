---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: authologic-aml-api-openapi.yml
  format: yaml
  label: Authologic AML API
  slug: authologic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-aml-api-openapi.yml
- filename: authologic-advanced-api-openapi.yml
  format: yaml
  label: Authologic Advanced API
  slug: authologic-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-advanced-api-openapi.yml
- filename: authologic-affordability-assessment-api-openapi.yml
  format: yaml
  label: Authologic Affordability assessment API
  slug: authologic-affordability-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-affordability-assessment-api-openapi.yml
- filename: authologic-aml-api-openapi.yml
  format: yaml
  label: Authologic AML API
  slug: authologic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-aml-api-openapi.yml
- filename: authologic-bank-api-openapi.yml
  format: yaml
  label: Authologic Bank API
  slug: authologic-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-bank-api-openapi.yml
- filename: authologic-conversation-api-openapi.yml
  format: yaml
  label: Authologic Conversation API
  slug: authologic-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-conversation-api-openapi.yml
- filename: authologic-database-verification-api-openapi.yml
  format: yaml
  label: Authologic Database Verification API
  slug: authologic-database-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-database-verification-api-openapi.yml
- filename: authologic-enterprise-integration-api-openapi.yml
  format: yaml
  label: Authologic Enterprise Integration API
  slug: authologic-enterprise-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-enterprise-integration-api-openapi.yml
- filename: authologic-metadata-api-openapi.yml
  format: yaml
  label: Authologic Metadata API
  slug: authologic-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-metadata-api-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Authologic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/conversations/{conversationId}/headless/{next}
operation_count: 14
overview: 'Authologic exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Authologic
provider_slug: authologic
slug: authologic-agentic-access
source_filename: authologic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: generated\nsource: openapi/authologic-customer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 4\n    connected: 10\n  by_consequence:\n    write: 3\n    physical: 1\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/conversations\n  method: post\n  operationId: createConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/conversations/{conversationId}/headless/{next}\n  method: post\n  operationId:\
  \ nextStep\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/conversations/{conversationId}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{conversationId}\n  method: delete\n  operationId: deleteConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/conversations/{conversationId}/identity/metadata\n\
  \  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{conversationId}/identity/metadata/media/{id}\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{conversationId}/headless\n  method: get\n  operationId: currentStep\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{conversationId}/databaseVerification/info\n  method: get\n  operationId: getDbV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{conversationId}/bankTransactions\n\
  \  method: get\n  operationId: getBankTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{conversationId}/bankTransactions/stats\n  method: get\n  operationId: getBankTransactionsStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{conversationId}/bankTransactions/accounts\n  method: get\n  operationId: getBankTransactionsAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{conversationId}/aml/{list}\n  method: get\n  operationId: getAMLList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{conversationId}/affordability/info\n\
  \  method: get\n  operationId: getAffordability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/subscriptions/{conversationId}/aml\n  method: delete\n  operationId: cancelAMLSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/agentic-access/authologic-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- AML
- Digital Identity
- eID
- Identity Verification
- KYB
- KYC
- Liveness Check
---
