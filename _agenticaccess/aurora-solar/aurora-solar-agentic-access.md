---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 22
api_specs:
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Projects API
  slug: aurora-solar-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Designs API
  slug: aurora-solar-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Proposals API
  slug: aurora-solar-proposals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Consumption Profiles API
  slug: aurora-solar-consumption-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Users & Tenants API
  slug: aurora-solar-users-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Webhooks API
  slug: aurora-solar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Financings API
  slug: aurora-solar-financings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Agreements API
  slug: aurora-solar-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
consequence_counts:
  read: 22
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aurora Solar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'Aurora Solar exposes 37 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Aurora Solar
provider_slug: aurora-solar
slug: aurora-solar-agentic-access
source_filename: aurora-solar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aurora-solar-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 22\n    acting: 15\n  by_consequence:\n    read: 22\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /tenants/{tenant_id}/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/projects/{project_id}\n  method: get\n  operationId: retrieveProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/projects/{project_id}\n  method: patch\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/projects/{project_id}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/projects/{project_id}/ahj\n  method: get\n  operationId: retrieveAhj\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/design_requests\n  method: post\n  operationId: createDesignRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/design_requests/{design_request_id}\n  method: get\n  operationId: retrieveDesignRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /tenants/{tenant_id}/design_requests/{design_request_id}\n  method: post\n  operationId: acceptDesignRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/designs\n  method: get\n  operationId: listDesigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/designs\n  method: post\n  operationId: createDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/designs/{design_id}\n\
  \  method: get\n  operationId: retrieveDesign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/designs/{design_id}/summary\n  method: get\n  operationId: retrieveDesignSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/proposals\n  method: post\n  operationId: createProposal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/proposals/{proposal_id}\n  method: get\n  operationId: retrieveProposal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/proposals/{proposal_id}\n  method: delete\n  operationId: deleteProposal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/proposal_templates\n  method: get\n  operationId: listProposalTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/designs/{design_id}/web_proposal\n  method: get\n  operationId: generateWebProposalUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/projects/{project_id}/consumption_profile\n\
  \  method: get\n  operationId: retrieveConsumptionProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/projects/{project_id}/consumption_profile\n  method: patch\n  operationId: updateConsumptionProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/projects/{project_id}/utility_bills\n  method: get\n  operationId: listUtilityBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/users/{user_id}\n  method: get\n  operationId: retrieveUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/users/{user_id}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}\n  method: get\n  operationId: retrieveTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/webhooks/{webhook_id}\n  method: get\n  operationId: retrieveWebhook\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/webhooks/{webhook_id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/financings\n  method: get\n  operationId: listFinancings\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/financings/{financing_id}\n  method: get\n  operationId: retrieveFinancing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/financings/{financing_id}/push\n  method: post\n  operationId: pushFinancingToFinancier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/agreements\n  method: get\n  operationId: listAgreements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/agreements/{agreement_id}\n\
  \  method: get\n  operationId: retrieveAgreement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/agreements/{agreement_id}/link\n  method: get\n  operationId: retrieveAgreementLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/agentic-access/aurora-solar-agentic-access.yml
summary_line: 37 operations · 15 acting
tags:
- Solar
- Solar Design
- PV
- Proposals
- CleanTech
- Energy
- Sales Software
---
