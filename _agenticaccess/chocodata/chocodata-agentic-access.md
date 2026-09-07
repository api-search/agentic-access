---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: chocodata-openapi.json
  format: json
  label: Chocodata Scraper API
  slug: chocodata-scraper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chocodata/refs/heads/main/openapi/chocodata-openapi.json
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chocodata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Chocodata exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chocodata
provider_slug: chocodata
slug: chocodata-agentic-access
source_filename: chocodata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: generated\nsource: openapi/chocodata-openapi.json + https://chocodata.com/docs (billing, batch, auth guides)\nnote: >-\n  Recommended x-agentic-access classifications for each OpenAPI operation. Chocodata is almost\n  entirely a read surface — every operation except createBatch is a GET scrape with no state\n  change on the provider side beyond credit consumption (5 credits per successful request,\n  non-2xx free). The consequential dimension is spend, not mutation.\noperations:\n  - operationId: scrape\n    action_class: read\n    consequence: billable-read\n    scope: any supported site/resource\n    token: api-key (api_key query parameter)\n    escalation: none\n    note: 5 credits per successful call; agent spend is bounded by plan credits and rate ceilings.\n  - operationId: universalGet\n    action_class: read\n    consequence: billable-read\n    scope: any URL on the web\n    token: api-key\n    escalation: none\n  - operationId: getProduct\n\
  \    action_class: read\n    consequence: billable-read\n    scope: single Amazon product\n    token: api-key\n    escalation: none\n  - operationId: getSearch\n    action_class: read\n    consequence: billable-read\n    scope: Amazon search results\n    token: api-key\n    escalation: none\n  - operationId: getAppStoreProduct\n    action_class: read\n    consequence: billable-read\n    scope: single App Store app\n    token: api-key\n    escalation: none\n  - operationId: getAppStoreReviews\n    action_class: read\n    consequence: billable-read\n    scope: App Store reviews for one app\n    token: api-key\n    escalation: none\n  - operationId: getGooglePlayProduct\n    action_class: read\n    consequence: billable-read\n    scope: single Google Play app\n    token: api-key\n    escalation: none\n  - operationId: getYouTubeTranscript\n    action_class: read\n    consequence: billable-read\n    scope: transcript of one YouTube video\n    token: api-key\n    escalation: none\n  - operationId:\
  \ getYouTubeComments\n    action_class: read\n    consequence: billable-read\n    scope: comments of one YouTube video\n    token: api-key\n    escalation: none\n  - operationId: getRedditPost\n    action_class: read\n    consequence: billable-read\n    scope: single Reddit post with comment tree\n    token: api-key\n    escalation: none\n  - operationId: createBatch\n    action_class: create\n    consequence: bulk-spend\n    scope: up to 1,000 items per submission, each billed independently on success (up to 5,000 credits per batch)\n    token: api-key\n    escalation: recommend human confirmation above the agent's spend cap — no cancel operation exists once submitted\n    note: The one mutating operation; no documented reversal or cancellation path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chocodata/refs/heads/main/agentic-access/chocodata-agentic-access.yml
summary_line: 11 operations
tags:
- Web Scraping
- Data Extraction
- SERP
- E-Commerce Data
- social-media-data
- Proxy
- MCP
- agent-native
- structured-json
---
