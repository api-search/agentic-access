---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 31
api_specs:
- filename: sharpapi-account-api-openapi.yml
  format: yaml
  label: SharpAPI Account API
  slug: sharpapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-account-api-openapi.yml
- filename: sharpapi-betting-splits-api-openapi.yml
  format: yaml
  label: SharpAPI Betting Splits API
  slug: sharpapi-betting-splits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-betting-splits-api-openapi.yml
- filename: sharpapi-deep-links-api-openapi.yml
  format: yaml
  label: SharpAPI Deep Links API
  slug: sharpapi-deep-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-deep-links-api-openapi.yml
- filename: sharpapi-events-api-openapi.yml
  format: yaml
  label: SharpAPI Events API
  slug: sharpapi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-events-api-openapi.yml
- filename: sharpapi-futures-api-openapi.yml
  format: yaml
  label: SharpAPI Futures API
  slug: sharpapi-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-futures-api-openapi.yml
- filename: sharpapi-game-state-api-openapi.yml
  format: yaml
  label: SharpAPI Game State API
  slug: sharpapi-game-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-game-state-api-openapi.yml
- filename: sharpapi-health-api-openapi.yml
  format: yaml
  label: SharpAPI Health API
  slug: sharpapi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-health-api-openapi.yml
- filename: sharpapi-odds-api-openapi.yml
  format: yaml
  label: SharpAPI Odds API
  slug: sharpapi-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-odds-api-openapi.yml
- filename: sharpapi-opportunities-api-openapi.yml
  format: yaml
  label: SharpAPI Opportunities API
  slug: sharpapi-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-opportunities-api-openapi.yml
- filename: sharpapi-reference-data-api-openapi.yml
  format: yaml
  label: SharpAPI Reference Data API
  slug: sharpapi-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-reference-data-api-openapi.yml
- filename: sharpapi-streaming-api-openapi.yml
  format: yaml
  label: SharpAPI Streaming API
  slug: sharpapi-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/openapi/sharpapi-streaming-api-openapi.yml
consequence_counts:
  read: 31
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Sharpapi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/keys/{keyId}
operation_count: 36
overview: 'SharpAPI exposes 36 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SharpAPI
provider_slug: sharpapi
slug: sharpapi-agentic-access
source_filename: sharpapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/sharpapi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 31\n    acting: 5\n  by_consequence:\n    read: 31\n    write: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /splits\n  method: get\n  operationId: listSplits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /splits/history\n  method: get\n\
  \  operationId: getSplitsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sports\n  method: get\n  operationId: listSports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leagues\n  method: get\n  operationId: listLeagues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sportsbooks\n  method: get\n  operationId: listSportsbooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets\n  method: get\n  operationId: listMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/markets\n  method: get\n  operationId: getEventMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/odds\n  method: get\n  operationId: getEventOdds\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /odds\n  method: get\n  operationId: listOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /odds/best\n  method: get\n  operationId: getBestOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /odds/comparison\n  method: get\n  operationId: compareOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /odds/batch\n  method: post\n  operationId: batchOdds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /odds/delta\n  method: get\n  operationId: getOddsDelta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/ev\n  method: get\n  operationId: listEVOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/arbitrage\n  method: get\n  operationId: listArbitrageOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/middles\n  method: get\n  operationId: listMiddleOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/middles/{id}\n  method: get\n\
  \  operationId: getMiddleOpportunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/middles/summary\n  method: get\n  operationId: getMiddlesSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/low_hold\n  method: get\n  operationId: listLowHoldOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stream\n  method: get\n  operationId: stream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/usage\n  method: get\n  operationId: getAccountUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/keys/{keyId}\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/keys/{keyId}/rotate\n  method: post\n  operationId: rotateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deeplinks/batch\n  method: post\n  operationId: batchDeepLinks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deeplink/{id}\n  method: get\n  operationId: redirectDeepLink\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /futures\n  method: get\n  operationId: listFuturesMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /futures/odds\n  method: get\n  operationId: listFuturesOdds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gamestate\n  method: get\n  operationId: listAllGameState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gamestate/{sport}\n  method: get\n  operationId: getGameStateForSport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharpapi/refs/heads/main/agentic-access/sharpapi-agentic-access.yml
summary_line: 36 operations · 5 acting · 1 human-in-the-loop
tags:
- Company
- Sports Betting
- Real-Time Data
- Gambling
---
