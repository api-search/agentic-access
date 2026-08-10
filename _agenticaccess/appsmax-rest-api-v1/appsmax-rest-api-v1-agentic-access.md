---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 15
api_specs:
- filename: appsmax-rest-api-v1-access-api-openapi.yml
  format: yaml
  label: AppsMax Access API
  slug: appsmax-rest-api-v1-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-access-api-openapi.yml
- filename: appsmax-rest-api-v1-applications-api-openapi.yml
  format: yaml
  label: AppsMax Applications API
  slug: appsmax-rest-api-v1-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-applications-api-openapi.yml
- filename: appsmax-rest-api-v1-bots-api-openapi.yml
  format: yaml
  label: AppsMax Bots API
  slug: appsmax-rest-api-v1-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-bots-api-openapi.yml
- filename: appsmax-rest-api-v1-campaigns-api-openapi.yml
  format: yaml
  label: AppsMax Campaigns API
  slug: appsmax-rest-api-v1-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-campaigns-api-openapi.yml
- filename: appsmax-rest-api-v1-funnels-api-openapi.yml
  format: yaml
  label: AppsMax Funnels API
  slug: appsmax-rest-api-v1-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-funnels-api-openapi.yml
- filename: appsmax-rest-api-v1-interactive-menu-api-openapi.yml
  format: yaml
  label: AppsMax Interactive menu API
  slug: appsmax-rest-api-v1-interactive-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-interactive-menu-api-openapi.yml
- filename: appsmax-rest-api-v1-miniapps-api-openapi.yml
  format: yaml
  label: AppsMax Miniapps API
  slug: appsmax-rest-api-v1-miniapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-miniapps-api-openapi.yml
- filename: appsmax-rest-api-v1-organizations-api-openapi.yml
  format: yaml
  label: AppsMax Organizations API
  slug: appsmax-rest-api-v1-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-organizations-api-openapi.yml
- filename: appsmax-rest-api-v1-subscribers-api-openapi.yml
  format: yaml
  label: AppsMax Subscribers API
  slug: appsmax-rest-api-v1-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-subscribers-api-openapi.yml
consequence_counts:
  read: 15
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Appsmax Rest Api V1 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'AppsMax exposes 21 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AppsMax
provider_slug: appsmax-rest-api-v1
slug: appsmax-rest-api-v1-agentic-access
source_filename: appsmax-rest-api-v1-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/appsmax-rest-api-v1-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 15\n    acting: 6\n  by_consequence:\n    read: 15\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getCurrentApiContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: get\n  operationId:\
  \ listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bots\n  method: get\n  operationId: listBots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bots/{bot}\n  method: get\n  operationId: getBot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bots/{bot}/connections\n  method: get\n  operationId: listBotConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /miniapps\n  method: get\n  operationId: listMiniapps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /funnels\n  method: get\n  operationId: listFunnels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interactive-menu\n  method: get\n  operationId: listInteractiveMenuItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /applications/{id}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application}/tags\n  method: post\n  operationId: syncApplicationTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{campaign}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/run\n  method: post\n  operationId: runCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers\n  method: get\n  operationId: listSubscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers\n  method: post\n  operationId: upsertSubscriber\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{id}\n  method: get\n  operationId: getSubscriber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{id}\n  method: patch\n  operationId: updateSubscriber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/agentic-access/appsmax-rest-api-v1-agentic-access.yml
summary_line: 21 operations · 6 acting
tags:
- Company
- SaaS
- Messaging
- Business Automation
- Chatbots
- Mini Apps
- Customer Requests
- Workflow Automation
- MAX
- Telegram
- Russian Language
---
