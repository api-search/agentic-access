---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 11
api_specs:
- filename: salesforce-streaming-api-asyncapi.yml
  format: yaml
  label: Service Cloud Streaming API
  slug: service-cloud-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/asyncapi/salesforce-streaming-api-asyncapi.yml
- filename: salesforce-service-cloud-accounts-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Accounts API
  slug: salesforce-service-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-accounts-api-openapi.yml
- filename: salesforce-service-cloud-availability-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Availability API
  slug: salesforce-service-cloud-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-availability-api-openapi.yml
- filename: salesforce-service-cloud-cases-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Cases API
  slug: salesforce-service-cloud-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-cases-api-openapi.yml
- filename: salesforce-service-cloud-contacts-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Contacts API
  slug: salesforce-service-cloud-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-contacts-api-openapi.yml
- filename: salesforce-service-cloud-knowledge-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Knowledge API
  slug: salesforce-service-cloud-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-knowledge-api-openapi.yml
- filename: salesforce-service-cloud-messages-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Messages API
  slug: salesforce-service-cloud-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-messages-api-openapi.yml
- filename: salesforce-service-cloud-query-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Query API
  slug: salesforce-service-cloud-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-query-api-openapi.yml
- filename: salesforce-service-cloud-search-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Search API
  slug: salesforce-service-cloud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-search-api-openapi.yml
- filename: salesforce-service-cloud-sessions-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Sessions API
  slug: salesforce-service-cloud-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-sessions-api-openapi.yml
- filename: salesforce-service-cloud-settings-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud Settings API
  slug: salesforce-service-cloud-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/openapi/salesforce-service-cloud-settings-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Salesforce Service Cloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Chasitor/ChatMessage
operation_count: 18
overview: 'Salesforce Service Cloud exposes 18 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Salesforce Service Cloud
provider_slug: salesforce-service-cloud
slug: salesforce-service-cloud-agentic-access
source_filename: salesforce-service-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/salesforce-live-agent-openapi.yml, openapi/salesforce-service-cloud-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 11\n    acting: 7\n  by_consequence:\n    read: 11\n    write: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /System/SessionId\n  method: get\n  operationId: getSessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Chasitor/ChasitorInit\n  method: post\n  operationId: initiateChatSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /System/Messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Chasitor/ChatMessage\n  method: post\n  operationId: sendChatMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Visitor/Availability\n  method: get\n  operationId: checkAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /Visitor/Settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Chasitor/ChatEnd\n  method: post\n  operationId: endChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sobjects/Case\n  method: get\n  operationId: getCaseInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sobjects/Case\n  method: post\n  operationId: createCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sobjects/Case/{caseId}\n  method: get\n  operationId: getCaseById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sobjects/Case/{caseId}\n  method: patch\n  operationId: updateCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sobjects/Case/{caseId}\n  method: delete\n  operationId: deleteCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sobjects/Contact\n  method: get\n  operationId: getContactInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sobjects/Contact\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sobjects/Account\n  method: get\n  operationId: getAccountInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sobjects/Knowledge__kav\n  method: get\n  operationId: getKnowledgeArticleInfo\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query\n  method: get\n  operationId: executeQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: executeSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/agentic-access/salesforce-service-cloud-agentic-access.yml
summary_line: 18 operations · 7 acting
tags:
- Case Management
- CRM
- Customer Service
- Help Desk
- Support
- Ticketing
---
