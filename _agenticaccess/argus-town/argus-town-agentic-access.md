---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 17
api_specs:
- filename: argus-town-alerts-api-openapi.yml
  format: yaml
  label: argus-town Alerts API
  slug: argus-town-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-alerts-api-openapi.yml
- filename: argus-town-connect-links-api-openapi.yml
  format: yaml
  label: argus-town Connect links API
  slug: argus-town-connect-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-connect-links-api-openapi.yml
- filename: argus-town-connections-api-openapi.yml
  format: yaml
  label: argus-town Connections API
  slug: argus-town-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-connections-api-openapi.yml
- filename: argus-town-events-api-openapi.yml
  format: yaml
  label: argus-town Events API
  slug: argus-town-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-events-api-openapi.yml
- filename: argus-town-negotiated-pricing-api-openapi.yml
  format: yaml
  label: argus-town Negotiated pricing API
  slug: argus-town-negotiated-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-negotiated-pricing-api-openapi.yml
- filename: argus-town-project-api-openapi.yml
  format: yaml
  label: argus-town Project API
  slug: argus-town-project-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-project-api-openapi.yml
- filename: argus-town-providers-api-openapi.yml
  format: yaml
  label: argus-town Providers API
  slug: argus-town-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-providers-api-openapi.yml
- filename: argus-town-spend-api-openapi.yml
  format: yaml
  label: argus-town Spend API
  slug: argus-town-spend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-spend-api-openapi.yml
- filename: argus-town-start-api-openapi.yml
  format: yaml
  label: argus-town Start API
  slug: argus-town-start-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-start-api-openapi.yml
- filename: argus-town-syncs-api-openapi.yml
  format: yaml
  label: argus-town Syncs API
  slug: argus-town-syncs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/argus-town/openapi/argus-town-syncs-api-openapi.yml
consequence_counts:
  physical: 1
  read: 17
  safety-critical: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Argus Town Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/negotiated_pricing/{provider}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/events
operation_count: 31
overview: 'argus-town exposes 31 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 12 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: argus-town
provider_slug: argus-town
slug: argus-town-agentic-access
source_filename: argus-town-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/argus-town-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 17\n    acting: 14\n  by_consequence:\n    read: 17\n    write: 12\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1\n  method: get\n  operationId: index_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/providers\n  method: get\n  operationId: providers_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/providers/{slug}\n\
  \  method: get\n  operationId: providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/device/code\n  method: post\n  operationId: device_code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/device/token\n  method: post\n  operationId: device_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/project\n  method: get\n  operationId: project_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/summary\n  method: get\n  operationId: summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections\n  method: get\n  operationId: connections_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections\n  method: post\n  operationId: connections_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{id}\n  method: get\n  operationId: connections_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{id}\n  method: patch\n  operationId: connections_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{id}\n  method: delete\n  operationId: connections_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events\n  method: post\n  operationId: events_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events\n  method: get\n  operationId: events_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/validate\n  method: post\n  operationId: events_validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/spend\n  method: get\n  operationId: spend_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{id}/syncs\n\
  \  method: post\n  operationId: syncs_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{id}/syncs\n  method: get\n  operationId: syncs_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/syncs/{id}\n  method: get\n  operationId: syncs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connect_links\n  method: post\n  operationId: connect_links_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connect_links/{id}\n  method: get\n  operationId: connect_links_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alert_rules\n  method: post\n  operationId: alert_rules_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alert_rules\n  method: get\n  operationId: alert_rules_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alert_rules/{id}\n  method: patch\n  operationId: alert_rules_update\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alert_rules/{id}\n  method: delete\n  operationId: alert_rules_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alert_firings\n  method: get\n  operationId: alert_firings_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/negotiated_pricing/{provider}\n  method: put\n  operationId: negotiated_pricing_put\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/negotiated_pricing/{provider}\n  method: get\n  operationId: negotiated_pricing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/negotiated_pricing/{provider}\n  method: delete\n  operationId: negotiated_pricing_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/openapi.json\n  method: get\n  operationId: openapi_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/errors\n  method: get\n  operationId: errors_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/argus-town/agentic-access/argus-town-agentic-access.yml
summary_line: 31 operations · 14 acting · 1 human-in-the-loop
tags:
- Company
- API Monitoring
- Cost Management
- Developer Tools
- MCP
---
