---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 18
api_specs:
- filename: thirdtrail-life-ephemerides-api-openapi.yml
  format: yaml
  label: thirdtrail-life Ephemerides API
  slug: thirdtrail-life-ephemerides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-ephemerides-api-openapi.yml
- filename: thirdtrail-life-mcp-api-openapi.yml
  format: yaml
  label: thirdtrail-life MCP API
  slug: thirdtrail-life-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-mcp-api-openapi.yml
- filename: thirdtrail-life-solar-api-openapi.yml
  format: yaml
  label: thirdtrail-life Solar API
  slug: thirdtrail-life-solar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-solar-api-openapi.yml
- filename: thirdtrail-life-tides-api-openapi.yml
  format: yaml
  label: thirdtrail-life Tides API
  slug: thirdtrail-life-tides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-tides-api-openapi.yml
- filename: thirdtrail-life-utility-api-openapi.yml
  format: yaml
  label: thirdtrail-life Utility API
  slug: thirdtrail-life-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thirdtrail-life/openapi/thirdtrail-life-utility-api-openapi.yml
consequence_counts:
  read: 18
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thirdtrail Life Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'thirdtrail-life exposes 26 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: thirdtrail-life
provider_slug: thirdtrail-life
slug: thirdtrail-life-agentic-access
source_filename: thirdtrail-life-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/thirdtrail-life-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 8\n    connected: 18\n  by_consequence:\n    write: 8\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: mcp_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/echo/\n  method: get\n  operationId: echo_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ephemerides/\n  method: get\n  operationId: ephemerides_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ephemerides/bulk/\n  method: post\n  operationId: ephemerides_bulk_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ephemerides/feed.ics\n  method: get\n  operationId: ephemerides_feed.ics_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ephemerides/prayer-times/\n  method: get\n  operationId: ephemerides_prayer_times_retrieve\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ephemerides/webhooks/\n  method: get\n  operationId: ephemerides_webhooks_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ephemerides/webhooks/\n  method: post\n  operationId: ephemerides_webhooks_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ephemerides/webhooks/{webhook_id}/\n  method: get\n  operationId: ephemerides_webhooks_retrieve_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/ephemerides/webhooks/{webhook_id}/\n  method: delete\n  operationId: ephemerides_webhooks_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hash/\n  method: get\n  operationId: hash_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solar/\n  method: get\n  operationId: solar_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solar/bulk/\n  method: post\n  operationId: solar_bulk_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/solar/dli/\n  method: get\n  operationId: solar_dli_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solar/feed.ics\n  method: get\n  operationId: solar_feed.ics_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solar/path/\n  method: get\n  operationId: solar_path_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solar/range/\n  method: get\n  operationId: solar_range_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solar/webhooks/\n  method: get\n  operationId: solar_webhooks_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solar/webhooks/\n  method: post\n  operationId: solar_webhooks_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/solar/webhooks/{webhook_id}/\n  method: get\n  operationId: solar_webhooks_retrieve_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/solar/webhooks/{webhook_id}/\n  method: delete\n  operationId: solar_webhooks_destroy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tides/bulk/\n  method: post\n  operationId: tides_bulk_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tides/constituents/\n  method: get\n  operationId: tides_constituents_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tides/extremes/\n  method: get\n  operationId: tides_extremes_retrieve\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tides/heights/\n  method: get\n  operationId: tides_heights_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tides/window/\n  method: get\n  operationId: tides_window_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/thirdtrail-life/agentic-access/thirdtrail-life-agentic-access.yml
summary_line: 26 operations · 8 acting
tags:
- Company
- Astronomy
- Tides
- Solar
---
