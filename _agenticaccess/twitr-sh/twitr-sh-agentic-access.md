---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 9
api_specs:
- filename: twitr-sh-accounts-api-openapi.yml
  format: yaml
  label: twitr-sh Accounts API
  slug: twitr-sh-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-accounts-api-openapi.yml
- filename: twitr-sh-creator-api-openapi.yml
  format: yaml
  label: twitr-sh Creator API
  slug: twitr-sh-creator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-creator-api-openapi.yml
- filename: twitr-sh-intelligence-api-openapi.yml
  format: yaml
  label: twitr-sh Intelligence API
  slug: twitr-sh-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-intelligence-api-openapi.yml
- filename: twitr-sh-monitors-api-openapi.yml
  format: yaml
  label: twitr-sh Monitors API
  slug: twitr-sh-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-monitors-api-openapi.yml
- filename: twitr-sh-search-api-openapi.yml
  format: yaml
  label: twitr-sh Search API
  slug: twitr-sh-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-search-api-openapi.yml
- filename: twitr-sh-snapshots-api-openapi.yml
  format: yaml
  label: twitr-sh Snapshots API
  slug: twitr-sh-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-snapshots-api-openapi.yml
- filename: twitr-sh-social-api-openapi.yml
  format: yaml
  label: twitr-sh Social API
  slug: twitr-sh-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-social-api-openapi.yml
- filename: twitr-sh-webhooks-api-openapi.yml
  format: yaml
  label: twitr-sh Webhooks API
  slug: twitr-sh-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitr-sh/openapi/twitr-sh-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 9
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Twitr Sh Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/webhooks/{id}/test
operation_count: 32
overview: 'twitr-sh exposes 32 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 22 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: twitr-sh
provider_slug: twitr-sh
slug: twitr-sh-agentic-access
source_filename: twitr-sh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/twitr-sh-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 9\n    acting: 23\n  by_consequence:\n    read: 9\n    write: 22\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/snapshots\n  method: get\n  operationId: list_my_snapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/snapshots/{id}\n  method: get\n  operationId: get_snapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/monitors\n\
  \  method: get\n  operationId: list_my_monitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/monitors/{id}\n  method: get\n  operationId: get_monitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/monitors/{id}\n  method: delete\n  operationId: delete_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/monitors/{id}/events\n  method: get\n  operationId: poll_monitor_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /api/webhooks\n  method: get\n  operationId: list_my_webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks\n  method: post\n  operationId: register_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{id}\n  method: get\n  operationId: get_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/{id}\n  method: delete\n  operationId: delete_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{id}/rotate\n  method: post\n  operationId: rotate_webhook_secret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{id}/test\n  method: post\n  operationId: test_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{id}/deliveries\n  method: get\n  operationId: list_webhook_deliveries\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x-accounts\n  method: get\n  operationId: list_connected_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x-accounts/start\n  method: post\n  operationId: start_account_connect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x-accounts/connect\n  method: post\n  operationId: connect_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x-accounts/confirm\n  method: post\n  operationId: confirm_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x-accounts/{handle}\n  method: delete\n  operationId: disconnect_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_read\n  method: post\n  operationId: x_read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_search\n  method: post\n  operationId: x_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_timeline\n  method: post\n  operationId: x_timeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_lists\n  method: post\n  operationId: x_lists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_communities\n  method: post\n  operationId: x_communities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_extract\n  method: post\n  operationId: x_extract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_monitor\n  method: post\n  operationId: x_monitor\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/draws\n  method: post\n  operationId: x_draws\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_write\n  method: post\n  operationId: x_write\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_inbox\n  method: post\n  operationId: x_inbox\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_profile\n  method: post\n  operationId: x_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/x_community\n  method: post\n  operationId: x_community\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/radar\n  method: post\n\
  \  operationId: x_radar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/compose\n  method: post\n  operationId: x_compose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/twitr-sh/agentic-access/twitr-sh-agentic-access.yml
summary_line: 32 operations · 23 acting
tags:
- Company
- X
- Twitter
- Pay-per-call
- Artificial Intelligence
---
