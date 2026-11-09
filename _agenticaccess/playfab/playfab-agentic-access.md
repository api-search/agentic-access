---
acting_count: 13
action_class_counts:
  acting: 13
api_specs:
- filename: playfab-client-openapi.yml
  format: yaml
  label: PlayFab Client API
  slug: playfab-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-client-openapi.yml
- filename: playfab-server-openapi.yml
  format: yaml
  label: PlayFab Server API
  slug: playfab-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-server-openapi.yml
- filename: playfab-admin-openapi.yml
  format: yaml
  label: PlayFab Admin API
  slug: playfab-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-admin-openapi.yml
- filename: playfab-authentication-openapi.yml
  format: yaml
  label: PlayFab Authentication API
  slug: playfab-entity-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-authentication-openapi.yml
- filename: playfab-cloudscript-openapi.yml
  format: yaml
  label: PlayFab CloudScript API
  slug: playfab-cloudscript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-cloudscript-openapi.yml
- filename: playfab-multiplayer-openapi.yml
  format: yaml
  label: PlayFab Multiplayer API
  slug: playfab-multiplayer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-multiplayer-openapi.yml
- filename: playfab-economy-openapi.yml
  format: yaml
  label: PlayFab Economy (Catalog / Inventory) API
  slug: playfab-economy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-economy-openapi.yml
- filename: playfab-data-openapi.yml
  format: yaml
  label: PlayFab Data API
  slug: playfab-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-data-openapi.yml
- filename: playfab-groups-openapi.yml
  format: yaml
  label: PlayFab Groups API
  slug: playfab-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-groups-openapi.yml
- filename: playfab-profiles-openapi.yml
  format: yaml
  label: PlayFab Profiles API
  slug: playfab-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-profiles-openapi.yml
- filename: playfab-events-openapi.yml
  format: yaml
  label: PlayFab Events API
  slug: playfab-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-events-openapi.yml
- filename: playfab-insights-openapi.yml
  format: yaml
  label: PlayFab Insights API
  slug: playfab-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-insights-openapi.yml
- filename: playfab-localization-openapi.yml
  format: yaml
  label: PlayFab Localization API
  slug: playfab-localization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-localization-openapi.yml
- filename: playfab-addon-openapi.yml
  format: yaml
  label: PlayFab Addon API
  slug: playfab-addon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-addon-openapi.yml
- filename: playfab-experimentation-openapi.yml
  format: yaml
  label: PlayFab Experimentation API
  slug: playfab-experimentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-experimentation-openapi.yml
- filename: playfab-leaderboards-openapi.yml
  format: yaml
  label: PlayFab Leaderboards API
  slug: playfab-leaderboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-leaderboards-openapi.yml
- filename: playfab-progression-openapi.yml
  format: yaml
  label: PlayFab Progression API
  slug: playfab-progression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-progression-openapi.yml
- filename: playfab-account-api-openapi.yml
  format: yaml
  label: PlayFab Account API
  slug: playfab-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-account-api-openapi.yml
- filename: playfab-authentication-api-openapi.yml
  format: yaml
  label: PlayFab Authentication API
  slug: playfab-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-authentication-api-openapi.yml
consequence_counts:
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Playfab Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'PlayFab exposes 13 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PlayFab
provider_slug: playfab
slug: playfab-agentic-access
source_filename: playfab-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/playfab-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 13\n  by_consequence:\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /Client/LoginWithPlayFab\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/LoginWithEmailAddress\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/LoginWithCustomID\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/LoginWithAndroidDeviceID\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/LoginWithIOSDeviceID\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/LoginWithApple\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/LoginWithGoogleAccount\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/LoginWithSteam\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/LoginWithXbox\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/RegisterPlayFabUser\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/GetTitlePublicKey\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/GetPhotonAuthenticationToken\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Client/SetPlayerSecret\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/playfab/agentic-access/playfab-agentic-access.yml
summary_line: 13 operations · 13 acting
tags:
- Authentication
- Microsoft Azure
- Backend
- Backend-as-a-Service
- CloudScript
- Economy
- Game Backend
- Game Development
- Games
- Leaderboards
- Matchmaking
- Microsoft
- Multiplayer
- PlayFab
- REST
---
