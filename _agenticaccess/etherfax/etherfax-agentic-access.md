---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 19
api_specs:
- filename: etherfax-accounts-api-openapi.yml
  format: yaml
  label: etherFAX Accounts API
  slug: etherfax-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-accounts-api-openapi.yml
- filename: etherfax-devices-api-openapi.yml
  format: yaml
  label: etherFAX Devices API
  slug: etherfax-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-devices-api-openapi.yml
- filename: etherfax-inbox-api-openapi.yml
  format: yaml
  label: etherFAX Inbox API
  slug: etherfax-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-inbox-api-openapi.yml
- filename: etherfax-outbox-api-openapi.yml
  format: yaml
  label: etherFAX Outbox API
  slug: etherfax-outbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-outbox-api-openapi.yml
- filename: etherfax-routes-api-openapi.yml
  format: yaml
  label: etherFAX Routes API
  slug: etherfax-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-routes-api-openapi.yml
- filename: etherfax-status-api-openapi.yml
  format: yaml
  label: etherFAX Status API
  slug: etherfax-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-status-api-openapi.yml
consequence_counts:
  read: 19
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Etherfax Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'etherFAX exposes 23 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: etherFAX
provider_slug: etherfax
slug: etherfax-agentic-access
source_filename: etherfax-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/etherfax-rest-api-30-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 19\n    acting: 4\n  by_consequence:\n    read: 19\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/pkinfo\n  method: post\n  operationId: accounts-pkino\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/pkinfo\n  method: post\n  operationId: devices-pkinfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices?a=actionreset\n  method: get\n  operationId: devices-actionreset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices?a=list\n  method: get\n  operationId: devices-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices?a=register\n  method: get\n  operationId: devices-register\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices?a=setaddr\n  method: get\n  operationId: devices-setaddr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices?a=setconfig\n  method: get\n  operationId: devices-setconfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices?a=status\n  method: get\n  operationId: devices-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices?a=unread\n  method: get\n  operationId: devices-unread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /inbox?a=get\n  method: get\n  operationId: inbox-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbox?a=getnext\n  method: get\n  operationId: inbox-getnext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbox?a=list\n  method: get\n  operationId: inbox-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbox?a=received\n  method: get\n  operationId: inbox-received\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inbox?a=unread\n  method: get\n  operationId: inbox-unread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outbox\n  method: post\n  operationId: outbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /outbox\n  method: get\n  operationId: outbox-pending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes\n  method: get\n  operationId: routes-enable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes?a=info\n  method: get\n  operationId: routes-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /routes?a=list\n  method: get\n  operationId: routes-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes?a=parse\n  method: get\n  operationId: routes-parse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: post\n  operationId: status-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/etherfax/agentic-access/etherfax-agentic-access.yml
summary_line: 23 operations · 4 acting
tags:
- Fax
- Cloud
- Artificial Intelligence
- Secure
- Document Automation
---
