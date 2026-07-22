---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 11
api_specs:
- filename: luxury-presence-cms-openapi.json
  format: json
  label: Luxury Presence Public API
  slug: luxury-presence-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luxury-presence/refs/heads/main/openapi/luxury-presence-cms-openapi.json
consequence_counts:
  read: 11
  safety-critical: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 24
kind: agentic-access
layout: agentic-access
method: generated
name: Luxury Presence Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cms/v1/agents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cms/v1/agents/bulkCreate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cms/v1/agents/bulkDelete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /cms/v1/agents/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cms/v1/agents/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cms/v1/agents/{id}/social-links/{type}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cms/v1/offices
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cms/v1/offices/bulkCreate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cms/v1/offices/bulkDelete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /cms/v1/offices/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cms/v1/offices/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cms/v1/offices/{id}/agents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cms/v1/offices/{id}/agents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cms/v1/teams
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cms/v1/teams/bulkCreate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cms/v1/teams/bulkDelete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /cms/v1/teams/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cms/v1/teams/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cms/v1/teams/{id}/agents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cms/v1/teams/{id}/agents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm/v1/webhooks
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /crm/v1/webhooks/webhook-example
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /crm/v1/webhooks/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /crm/v1/webhooks/{id}
operation_count: 35
overview: 'Luxury Presence exposes 35 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 24 safety-critical.


  24 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Luxury Presence
provider_slug: luxury-presence
slug: luxury-presence-agentic-access
source_filename: luxury-presence-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/luxury-presence-cms-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 11\n    acting: 24\n  by_consequence:\n    read: 11\n    safety-critical: 24\n  human_in_the_loop_required: 24\noperations:\n- path: /cms/v1/agents\n  method: get\n  operationId: AgentsController_handleGetAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cms/v1/agents\n  method: post\n  operationId: AgentsController_handlePostAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/agents/{id}\n  method: get\n  operationId: AgentsController_handleGetAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cms/v1/agents/{id}\n  method: patch\n  operationId: AgentsController_handlePatchAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/agents/{id}\n  method: delete\n  operationId: AgentsController_handleDeleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/agents/bulkCreate\n  method: post\n  operationId: AgentsController_handleBulkCreateAgents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/agents/{id}/social-links/{type}\n  method: delete\n  operationId: AgentsController_handleDeleteAgentSocialLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/agents/bulkDelete\n  method: delete\n  operationId: AgentsController_handleBulkDeleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/media/{mediaId}\n  method: get\n  operationId: MediaReadController_getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cms/v1/offices\n  method: get\n  operationId: OfficesController_handleGetOffices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /cms/v1/offices\n  method: post\n  operationId: OfficesController_handlePostOffice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/offices/{id}\n  method: get\n  operationId: OfficesController_handleGetOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cms/v1/offices/{id}\n  method: patch\n  operationId: OfficesController_handlePatchOffice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/offices/{id}\n  method: delete\n  operationId: OfficesController_handleDeleteOffice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/offices/bulkCreate\n  method: post\n  operationId: OfficesController_handleBulkCreateOffices\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/offices/bulkDelete\n  method: delete\n  operationId: OfficesController_handleBulkDeleteOffice\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/offices/{id}/agents\n  method: get\n  operationId: OfficesController_handleGetOfficeAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cms/v1/offices/{id}/agents\n  method: delete\n  operationId: OfficesController_handleDeleteOfficeAgents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /cms/v1/offices/{id}/agents\n  method: post\n  operationId: OfficesController_handlePostOfficeAgents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/teams\n  method: get\n  operationId: TeamsController_handleGetTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cms/v1/teams\n  method: post\n  operationId: TeamsController_handlePostTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /cms/v1/teams/{id}\n  method: get\n  operationId: TeamsController_handleGetTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cms/v1/teams/{id}\n  method: patch\n  operationId: TeamsController_handlePatchTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/teams/{id}\n  method: delete\n  operationId: TeamsController_handleDeleteTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/teams/{id}/agents\n  method: get\n  operationId: TeamsController_handleGetTeamAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cms/v1/teams/{id}/agents\n  method: delete\n  operationId: TeamsController_handleDeleteTeamAgents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/teams/{id}/agents\n  method: post\n  operationId: TeamsController_handlePostTeamAgents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/teams/bulkCreate\n  method: post\n  operationId: TeamsController_handleBulkCreateTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cms/v1/teams/bulkDelete\n  method: delete\n  operationId: TeamsController_handleBulkDeleteTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /crm/v1/webhooks\n  method: post\n  operationId: WebhookController_createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm/v1/webhooks\n  method: get\n  operationId: WebhookController_listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/v1/webhooks/{id}\n  method: get\n  operationId: WebhookController_getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm/v1/webhooks/{id}\n  method: patch\n  operationId: WebhookController_updateWebhook\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm/v1/webhooks/{id}\n  method: delete\n  operationId: WebhookController_deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm/v1/webhooks/webhook-example\n  method: post\n  operationId: WebhookController_exampleWebhookPayload\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luxury-presence/refs/heads/main/agentic-access/luxury-presence-agentic-access.yml
summary_line: 35 operations · 24 acting · 24 human-in-the-loop
tags:
- Company
- Vertical Software
- Real Estate
- PropTech
- CRM
- Marketing
- Websites
- Webhooks
- Lead Generation
---
