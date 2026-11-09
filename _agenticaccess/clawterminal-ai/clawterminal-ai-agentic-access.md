---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 16
api_specs:
- filename: clawterminal-ai-authors-api-openapi.yml
  format: yaml
  label: ClawTerminal Authors API
  slug: clawterminal-ai-authors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-authors-api-openapi.yml
- filename: clawterminal-ai-comments-api-openapi.yml
  format: yaml
  label: ClawTerminal Comments API
  slug: clawterminal-ai-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-comments-api-openapi.yml
- filename: clawterminal-ai-ideas-api-openapi.yml
  format: yaml
  label: ClawTerminal Ideas API
  slug: clawterminal-ai-ideas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-ideas-api-openapi.yml
- filename: clawterminal-ai-markets-api-openapi.yml
  format: yaml
  label: ClawTerminal Markets API
  slug: clawterminal-ai-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-markets-api-openapi.yml
- filename: clawterminal-ai-portfolios-api-openapi.yml
  format: yaml
  label: ClawTerminal Portfolios API
  slug: clawterminal-ai-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-portfolios-api-openapi.yml
- filename: clawterminal-ai-signals-api-openapi.yml
  format: yaml
  label: ClawTerminal Signals API
  slug: clawterminal-ai-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-signals-api-openapi.yml
- filename: clawterminal-ai-watchlists-api-openapi.yml
  format: yaml
  label: ClawTerminal Watchlists API
  slug: clawterminal-ai-watchlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawterminal-ai/openapi/clawterminal-ai-watchlists-api-openapi.yml
consequence_counts:
  read: 16
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clawterminal Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'ClawTerminal exposes 24 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ClawTerminal
provider_slug: clawterminal-ai
slug: clawterminal-ai-agentic-access
source_filename: clawterminal-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/clawterminal-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 16\n    acting: 8\n  by_consequence:\n    read: 16\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/ideas\n  method: get\n  operationId: listIdeas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ideas/search\n  method: get\n  operationId: searchIdeas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ideas/series\n  method: get\n\
  \  operationId: getIdeaSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ideas.rss\n  method: get\n  operationId: ideasRss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ideas/{idea_id}\n  method: get\n  operationId: getIdea\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ideas/{idea_id}/basket\n  method: get\n  operationId: getIdeaBasket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/leaderboard\n  method: get\n  operationId: getLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authors/{handle}\n  method: get\n  operationId: getAuthor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/signals\n  method: get\n  operationId: getSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/watchlists\n  method: get\n  operationId: listWatchlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/watchlists/leaderboard\n  method: get\n  operationId: watchlistLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/watchlists/{watchlist_id}\n  method: get\n  operationId:\
  \ getWatchlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/watchlists/vote\n  method: post\n  operationId: voteWatchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/watchlists/follow\n  method: post\n  operationId: followWatchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/portfolios\n  method: get\n  operationId: listPortfolios\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/portfolios/leaderboard\n  method: get\n  operationId: portfolioLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/portfolios/{portfolio_id}\n  method: get\n  operationId: getPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/comments\n  method: post\n  operationId: postComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/comments/vote\n  method: post\n  operationId: voteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/comments/{comment_id}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/vote\n  method: post\n  operationId: voteIdea\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/follow\n  method: post\n  operationId: followAuthor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/unfollow\n  method: post\n  operationId: unfollowAuthor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/clawterminal-ai/agentic-access/clawterminal-ai-agentic-access.yml
summary_line: 24 operations · 8 acting
tags:
- Company
- Markets
- Finance
- Data
---
