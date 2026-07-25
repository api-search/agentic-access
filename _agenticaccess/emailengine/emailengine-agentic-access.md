---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 14
api_specs:
- filename: emailengine-account-api-openapi.yml
  format: yaml
  label: EmailEngine Account API
  slug: emailengine-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-account-api-openapi.yml
- filename: emailengine-accounts-api-openapi.yml
  format: yaml
  label: EmailEngine Accounts API
  slug: emailengine-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-accounts-api-openapi.yml
- filename: emailengine-autoconfig-api-openapi.yml
  format: yaml
  label: EmailEngine Autoconfig API
  slug: emailengine-autoconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-autoconfig-api-openapi.yml
- filename: emailengine-deliverytest-api-openapi.yml
  format: yaml
  label: EmailEngine Deliverytest API
  slug: emailengine-deliverytest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-deliverytest-api-openapi.yml
- filename: emailengine-gateways-api-openapi.yml
  format: yaml
  label: EmailEngine Gateways API
  slug: emailengine-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-gateways-api-openapi.yml
- filename: emailengine-license-api-openapi.yml
  format: yaml
  label: EmailEngine License API
  slug: emailengine-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-license-api-openapi.yml
- filename: emailengine-logs-api-openapi.yml
  format: yaml
  label: EmailEngine Logs API
  slug: emailengine-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-logs-api-openapi.yml
- filename: emailengine-oauth2-api-openapi.yml
  format: yaml
  label: EmailEngine Oauth2 API
  slug: emailengine-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-oauth2-api-openapi.yml
- filename: emailengine-outbox-api-openapi.yml
  format: yaml
  label: EmailEngine Outbox API
  slug: emailengine-outbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-outbox-api-openapi.yml
- filename: emailengine-stats-api-openapi.yml
  format: yaml
  label: EmailEngine Stats API
  slug: emailengine-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-stats-api-openapi.yml
- filename: emailengine-templates-api-openapi.yml
  format: yaml
  label: EmailEngine Templates API
  slug: emailengine-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-templates-api-openapi.yml
- filename: emailengine-tokens-api-openapi.yml
  format: yaml
  label: EmailEngine Tokens API
  slug: emailengine-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-tokens-api-openapi.yml
- filename: emailengine-webhookroutes-api-openapi.yml
  format: yaml
  label: EmailEngine Webhookroutes API
  slug: emailengine-webhookroutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/openapi/emailengine-webhookroutes-api-openapi.yml
consequence_counts:
  read: 14
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Emailengine Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'EmailEngine exposes 15 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EmailEngine
provider_slug: emailengine
slug: emailengine-agentic-access
source_filename: emailengine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/emailengine-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 14\n    acting: 1\n  by_consequence:\n    read: 14\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/{account}/mailboxes\n  method: get\n  operationId: listMailboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/{account}/messages\n\
  \  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/{account}/submit\n  method: post\n  operationId: submitMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/outbox\n  method: get\n  operationId: listOutbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deliverytest/check/{deliverytest}\n  method: get\n  operationId: checkDeliveryTest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/tokens\n  method: get\n  operationId: listTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/autoconfig\n  method: get\n  operationId: getAutoconfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/logs/{account}\n  method: get\n  operationId: getAccountLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/license\n  method: get\n  operationId: getLicense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhookroutes\n  method: get\n  operationId: listWebhookRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oauth2\n  method: get\n  operationId: listOauth2Apps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gateways\n  method: get\n  operationId: listGateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailengine/refs/heads/main/agentic-access/emailengine-agentic-access.yml
summary_line: 15 operations · 1 acting
tags:
- Email
- Email API
- IMAP
- SMTP
- Webhooks
---
