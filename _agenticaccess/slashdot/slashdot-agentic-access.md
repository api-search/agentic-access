---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: slashdot-rss-openapi.yml
  format: yaml
  label: Slashdot RSS/Atom Feeds
  slug: rss-feeds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/openapi/slashdot-rss-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Slashdot Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Slashdot exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Slashdot
provider_slug: slashdot
slug: slashdot-agentic-access
source_filename: slashdot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/slashdot-rss-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /Slashdot/slashdotMain\n  method: get\n  operationId: getMainFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Slashdot/slashdotMainatom\n  method: get\n  operationId: getMainFeedAtom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Slashdot/slashdotDevelopers\n  method: get\n\
  \  operationId: getDevelopersFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Slashdot/slashdotLinux\n  method: get\n  operationId: getLinuxFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Slashdot/slashdotApple\n  method: get\n  operationId: getAppleFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Slashdot/slashdotGames\n  method: get\n  operationId: getGamesFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Slashdot/slashdotScience\n  method: get\n  operationId: getScienceFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Slashdot/slashdotYourRightsOnline\n  method: get\n  operationId: getYourRightsOnlineFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/agentic-access/slashdot-agentic-access.yml
summary_line: 8 operations
tags:
- Media
- Open Source
- Technology News
- RSS
---
