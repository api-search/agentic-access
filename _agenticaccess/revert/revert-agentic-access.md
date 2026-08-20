---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 26
api_specs:
- filename: revert-accounting-api-openapi.yml
  format: yaml
  label: Revert Accounting API
  slug: revert-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-accounting-api-openapi.yml
- filename: revert-chat-api-openapi.yml
  format: yaml
  label: Revert Chat API
  slug: revert-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-chat-api-openapi.yml
- filename: revert-connections-api-openapi.yml
  format: yaml
  label: Revert Connections API
  slug: revert-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-connections-api-openapi.yml
- filename: revert-crm-companies-api-openapi.yml
  format: yaml
  label: Revert CRM Companies API
  slug: revert-crm-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-companies-api-openapi.yml
- filename: revert-crm-contacts-api-openapi.yml
  format: yaml
  label: Revert CRM Contacts API
  slug: revert-crm-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-contacts-api-openapi.yml
- filename: revert-crm-deals-api-openapi.yml
  format: yaml
  label: Revert CRM Deals API
  slug: revert-crm-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-deals-api-openapi.yml
- filename: revert-crm-events-api-openapi.yml
  format: yaml
  label: Revert CRM Events API
  slug: revert-crm-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-events-api-openapi.yml
- filename: revert-crm-leads-api-openapi.yml
  format: yaml
  label: Revert CRM Leads API
  slug: revert-crm-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-leads-api-openapi.yml
- filename: revert-crm-notes-api-openapi.yml
  format: yaml
  label: Revert CRM Notes API
  slug: revert-crm-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-notes-api-openapi.yml
- filename: revert-crm-properties-api-openapi.yml
  format: yaml
  label: Revert CRM Properties API
  slug: revert-crm-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-properties-api-openapi.yml
- filename: revert-crm-tasks-api-openapi.yml
  format: yaml
  label: Revert CRM Tasks API
  slug: revert-crm-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-tasks-api-openapi.yml
- filename: revert-crm-users-api-openapi.yml
  format: yaml
  label: Revert CRM Users API
  slug: revert-crm-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-crm-users-api-openapi.yml
- filename: revert-tickets-api-openapi.yml
  format: yaml
  label: Revert Tickets API
  slug: revert-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/openapi/revert-tickets-api-openapi.yml
consequence_counts:
  physical: 1
  read: 26
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Revert Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chat/messages
operation_count: 51
overview: 'Revert exposes 51 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 24 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Revert
provider_slug: revert
slug: revert-agentic-access
source_filename: revert-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/revert-unified-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    connected: 26\n    acting: 25\n  by_consequence:\n    read: 26\n    write: 24\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /connection\n  method: get\n  operationId: getConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connection/webhook\n  method: post\n  operationId: createConnectionWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connection/webhook\n  method: get\n  operationId: getConnectionWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connection/webhook\n  method: delete\n  operationId: deleteConnectionWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/contacts/{id}\n  method: get\n  operationId: getCrmContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/contacts/{id}\n  method: patch\n  operationId:\
  \ updateCrmContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/contacts\n  method: get\n  operationId: getCrmContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/contacts\n  method: post\n  operationId: createCrmContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/contacts/search\n  method: post\n  operationId: searchCrmContacts\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/companies/{id}\n  method: get\n  operationId: getCrmCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/companies/{id}\n  method: patch\n  operationId: updateCrmCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/companies\n  method: get\n  operationId: getCrmCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /crm/companies\n  method: post\n  operationId: createCrmCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/deals/{id}\n  method: get\n  operationId: getCrmDeal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/deals/{id}\n  method: patch\n  operationId: updateCrmDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/deals\n  method: get\n  operationId: getCrmDeals\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/deals\n  method: post\n  operationId: createCrmDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/leads/{id}\n  method: get\n  operationId: getCrmLead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/leads/{id}\n  method: patch\n  operationId: updateCrmLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /crm/leads\n  method: get\n  operationId: getCrmLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/leads\n  method: post\n  operationId: createCrmLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/notes/{id}\n  method: get\n  operationId: getCrmNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/notes/{id}\n  method: patch\n  operationId: updateCrmNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/notes\n  method: get\n  operationId: getCrmNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/notes\n  method: post\n  operationId: createCrmNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/tasks/{id}\n  method: get\n  operationId: getCrmTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/tasks/{id}\n  method: patch\n  operationId: updateCrmTask\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/tasks\n  method: get\n  operationId: getCrmTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/tasks\n  method: post\n  operationId: createCrmTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/events/{id}\n  method: get\n  operationId: getCrmEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /crm/events/{id}\n  method: patch\n  operationId: updateCrmEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/events/{id}\n  method: delete\n  operationId: deleteCrmEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/events\n  method: get\n  operationId: getCrmEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/events\n  method: post\n  operationId: createCrmEvent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/users/{id}\n  method: get\n  operationId: getCrmUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/users\n  method: get\n  operationId: getCrmUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/users\n  method: post\n  operationId: createCrmUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /crm/properties\n  method: get\n  operationId: getCrmProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/properties\n  method: post\n  operationId: createCrmProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crm/proxy\n  method: post\n  operationId: crmProxy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ticket/tasks/{id}\n  method: get\n  operationId:\
  \ getTicketTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ticket/tasks/{id}\n  method: patch\n  operationId: updateTicketTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ticket/tasks\n  method: get\n  operationId: getTicketTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ticket/tasks\n  method: post\n  operationId: createTicketTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ticket/collections\n  method: get\n  operationId: getTicketCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/channels\n  method: get\n  operationId: getChatChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/messages\n  method: get\n  operationId: getChatMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/messages\n  method: post\n  operationId: sendChatMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/accounts\n  method: get\n  operationId: getAccountingAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/expenses\n  method: get\n  operationId: getAccountingExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/expenses\n  method: post\n  operationId: createAccountingExpense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revert/refs/heads/main/agentic-access/revert-agentic-access.yml
summary_line: 51 operations · 25 acting
tags:
- Integration
- CRM
- Unified-API
- Open-Source
---
