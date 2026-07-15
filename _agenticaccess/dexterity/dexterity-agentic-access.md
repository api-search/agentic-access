---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: dexterity-foresight-packing-challenge-openapi.yml
  format: yaml
  label: Dexterity Foresight Packing Challenge API
  slug: dexterity-foresight-packing-challenge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexterity/refs/heads/main/openapi/dexterity-foresight-packing-challenge-openapi.yml
consequence_counts:
  read: 4
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Dexterity Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /stop
operation_count: 8
overview: 'Dexterity exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 3 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dexterity
provider_slug: dexterity
slug: dexterity-agentic-access
source_filename: dexterity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dexterity-foresight-packing-challenge-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 4\n    connected: 4\n  by_consequence:\n    write: 3\n    safety-critical: 1\n    read: 4\n  human_in_the_loop_required: 1\noperations:\n- path: /start\n  method: post\n  operationId: start_game_start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /place\n  method: post\n  operationId: place_box_place_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stop\n  method: post\n  operationId: stop_game_stop_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /status/{game_id}\n  method: get\n  operationId: get_status_status__game_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /my-games\n  method: get\n  operationId: get_my_games_my_games_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /display-name\n  method: post\n  operationId: update_display_name_display_name_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leaderboard\n  method: get\n  operationId: get_leaderboard_leaderboard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexterity/refs/heads/main/agentic-access/dexterity-agentic-access.yml
summary_line: 8 operations · 4 acting · 1 human-in-the-loop
tags:
- Physical AI
- Industrial Robotics
- Robotics
- Warehouse Automation
- Logistics
- Manufacturing
- World Model
- Foresight
- Mech
- Dual-Arm
- Truck Loading
- Palletizing
- Depalletizing
- Singulation
- Research API
- Packing Challenge
---
