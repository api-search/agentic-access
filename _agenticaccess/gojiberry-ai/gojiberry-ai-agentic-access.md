---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 19
api_specs:
- filename: gojiberry-ai-appexternal-api-openapi.yml
  format: yaml
  label: Gojiberry AI AppExternal API
  slug: gojiberry-ai-appexternal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-appexternal-api-openapi.yml
- filename: gojiberry-ai-campaigns-api-openapi.yml
  format: yaml
  label: Gojiberry AI Campaigns API
  slug: gojiberry-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-campaigns-api-openapi.yml
- filename: gojiberry-ai-contacts-api-openapi.yml
  format: yaml
  label: Gojiberry AI Contacts API
  slug: gojiberry-ai-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-contacts-api-openapi.yml
- filename: gojiberry-ai-lead-source-agents-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lead source agents API
  slug: gojiberry-ai-lead-source-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lead-source-agents-api-openapi.yml
- filename: gojiberry-ai-lists-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lists API
  slug: gojiberry-ai-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lists-api-openapi.yml
- filename: gojiberry-ai-organization-api-openapi.yml
  format: yaml
  label: Gojiberry AI Organization API
  slug: gojiberry-ai-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-organization-api-openapi.yml
- filename: gojiberry-ai-unibox-api-openapi.yml
  format: yaml
  label: Gojiberry AI Unibox API
  slug: gojiberry-ai-unibox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-unibox-api-openapi.yml
- filename: gojiberry-ai-user-api-openapi.yml
  format: yaml
  label: Gojiberry AI User API
  slug: gojiberry-ai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-user-api-openapi.yml
consequence_counts:
  read: 19
  safety-critical: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 9
kind: agentic-access
layout: agentic-access
method: generated
name: Gojiberry Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/agent/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/campaign/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/contact
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/contact/list/{listId}/contacts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/contact/list/{listId}/contacts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/contact/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/contact/{id}/enrich/email
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/list
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/unibox/messages/send-message
operation_count: 28
overview: 'Gojiberry AI exposes 28 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 9 safety-critical.


  9 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gojiberry AI
provider_slug: gojiberry-ai
slug: gojiberry-ai-agentic-access
source_filename: gojiberry-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/gojiberry-ai-appexternal-api-openapi.yml, openapi/gojiberry-ai-campaigns-api-openapi.yml,\n  openapi/gojiberry-ai-contacts-api-openapi.yml, openapi/gojiberry-ai-lead-source-agents-api-openapi.yml,\n  openapi/gojiberry-ai-lists-api-openapi.yml, openapi/gojiberry-ai-organization-api-openapi.yml,\n  openapi/gojiberry-ai-unibox-api-openapi.yml, openapi/gojiberry-ai-user-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 19\n    acting: 9\n  by_consequence:\n    read: 19\n    safety-critical: 9\n  human_in_the_loop_required: 9\noperations:\n- path: /\n  method: get\n  operationId: AppExternalController_getHello\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: AppExternalController_healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaign\n  method: get\n  operationId: CampaignExternalController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaign/{id}\n  method: get\n  operationId: CampaignExternalController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaign/{id}\n  method: patch\n  operationId: CampaignExternalController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/contact\n  method: post\n  operationId: ContactExternalController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/contact\n  method: get\n  operationId: ContactExternalController_findMany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contact/{id}\n  method: patch\n  operationId: ContactExternalController_update\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/contact/{id}\n  method: get\n  operationId: ContactExternalController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contact/list/{listId}/contacts\n  method: post\n  operationId: ContactExternalController_addManyToList\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/contact/list/{listId}/contacts\n  method: delete\n  operationId:\
  \ ContactExternalController_removeManyFromList\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/contact/intent-type-counts\n  method: get\n  operationId: ContactExternalController_getIntentTypeCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contact/{id}/enrich/email\n  method: post\n  operationId: ContactExternalController_enrichEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v1/agent\n  method: get\n  operationId: AgentExternalController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/{id}\n  method: get\n  operationId: AgentExternalController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/{id}\n  method: patch\n  operationId: AgentExternalController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/{id}/logs\n  method: get\n  operationId: AgentExternalController_findLogs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list\n  method: post\n  operationId: ListExternalController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/list\n  method: get\n  operationId: ListExternalController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/list/{id}\n  method: get\n  operationId: ListExternalController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization\n\
  \  method: get\n  operationId: OrganizationExternalController_getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization/members\n  method: get\n  operationId: OrganizationExternalController_getOrganizationMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/unibox/contact/{contactId}\n  method: get\n  operationId: UniboxExternalController_getMessagesByContactId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/unibox/threads\n  method: get\n  operationId: UniboxExternalController_getThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/unibox/threads/{threadId}/messages\n  method: get\n  operationId: UniboxExternalController_getThreadMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/unibox/messages/send-message\n  method: post\n  operationId: UniboxExternalController_sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/user/me\n  method: get\n  operationId: UserExternalController_getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/me/permissions\n  method: get\n  operationId: UserExternalController_getMyPermissions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/agentic-access/gojiberry-ai-agentic-access.yml
summary_line: 28 operations · 9 acting · 9 human-in-the-loop
tags:
- Company
- Sales
- Lead Generation
- Sales Intelligence
- AI Agents
- Outbound
- Go-To-Market
- Prospecting
- LinkedIn
- CRM
---
