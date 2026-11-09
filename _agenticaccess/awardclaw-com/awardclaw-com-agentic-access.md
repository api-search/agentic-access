---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: awardclaw-com-availability-api-openapi.yml
  format: yaml
  label: AwardClaw Availability API
  slug: awardclaw-com-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-availability-api-openapi.yml
- filename: awardclaw-com-briefing-api-openapi.yml
  format: yaml
  label: AwardClaw Briefing API
  slug: awardclaw-com-briefing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-briefing-api-openapi.yml
- filename: awardclaw-com-cards-api-openapi.yml
  format: yaml
  label: AwardClaw Cards API
  slug: awardclaw-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-cards-api-openapi.yml
- filename: awardclaw-com-drops-api-openapi.yml
  format: yaml
  label: AwardClaw Drops API
  slug: awardclaw-com-drops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-drops-api-openapi.yml
- filename: awardclaw-com-me-api-openapi.yml
  format: yaml
  label: AwardClaw Me API
  slug: awardclaw-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-me-api-openapi.yml
- filename: awardclaw-com-news-api-openapi.yml
  format: yaml
  label: AwardClaw News API
  slug: awardclaw-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-news-api-openapi.yml
- filename: awardclaw-com-watches-api-openapi.yml
  format: yaml
  label: AwardClaw Watches API
  slug: awardclaw-com-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awardclaw-com/openapi/awardclaw-com-watches-api-openapi.yml
consequence_counts:
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Awardclaw Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'AwardClaw exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AwardClaw
provider_slug: awardclaw-com
slug: awardclaw-com-agentic-access
source_filename: awardclaw-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/awardclaw-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 8\n    acting: 2\n  by_consequence:\n    read: 8\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /drops\n  method: get\n  operationId: searchDrops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drops/{id}\n  method: get\n  operationId: getDrop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /availability\n  method: get\n  operationId: searchAvailability\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /watches\n  method: get\n  operationId: listWatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /watches\n  method: post\n  operationId: createWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watches\n  method: delete\n  operationId: deleteWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /briefing\n  method: get\n  operationId: getBriefing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news\n  method: get\n  operationId: searchNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards\n  method: get\n  operationId: getCardOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/awardclaw-com/agentic-access/awardclaw-com-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- Travel
- Awards
- Airlines
- flight-deals
- Automation
- Newsletters
---
