---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: crowdwisdomtrading-account-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Account API
  slug: crowdwisdomtrading-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-account-api-openapi.yml
- filename: crowdwisdomtrading-health-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Health API
  slug: crowdwisdomtrading-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-health-api-openapi.yml
- filename: crowdwisdomtrading-signals-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Signals API
  slug: crowdwisdomtrading-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-signals-api-openapi.yml
- filename: crowdwisdomtrading-socialmap-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Socialmap API
  slug: crowdwisdomtrading-socialmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-socialmap-api-openapi.yml
- filename: crowdwisdomtrading-socialmap-preview-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Socialmap Preview API
  slug: crowdwisdomtrading-socialmap-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-socialmap-preview-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crowdwisdomtrading Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'CrowdWisdom Signals API exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CrowdWisdom Signals API
provider_slug: crowdwisdomtrading
slug: crowdwisdomtrading-agentic-access
source_filename: crowdwisdomtrading-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: generated\nsource: openapi/crowdwisdomtrading-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: v1_health_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/top\n  method:\
  \ get\n  operationId: v1_top_signals_v1_signals_top_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals\n  method: get\n  operationId: v1_list_signals_v1_signals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{signal_uid}\n  method: get\n  operationId: v1_get_signal_v1_signals__signal_uid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: v1_account_v1_account_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/keys/rotate\n  method: post\n  operationId: v1_rotate_key_v1_account_keys_rotate_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /socialmap-preview\n  method: get\n  operationId: socialmap_preview_socialmap_preview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/socialmap/{ticker}\n  method: get\n  operationId: v1_socialmap_v1_socialmap__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/agentic-access/crowdwisdomtrading-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Finance
- Trading
- Signals
- B2B
---
