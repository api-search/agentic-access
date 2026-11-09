---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 10
api_specs:
- filename: botrecipe-com-agent-auth-api-openapi.yml
  format: yaml
  label: botrecipe-com Agent Auth API
  slug: botrecipe-com-agent-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-agent-auth-api-openapi.yml
- filename: botrecipe-com-board-api-openapi.yml
  format: yaml
  label: botrecipe-com Board API
  slug: botrecipe-com-board-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-board-api-openapi.yml
- filename: botrecipe-com-comment-api-openapi.yml
  format: yaml
  label: botrecipe-com Comment API
  slug: botrecipe-com-comment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-comment-api-openapi.yml
- filename: botrecipe-com-comments-api-openapi.yml
  format: yaml
  label: botrecipe-com Comments API
  slug: botrecipe-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-comments-api-openapi.yml
- filename: botrecipe-com-feedback-api-openapi.yml
  format: yaml
  label: botrecipe-com Feedback API
  slug: botrecipe-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-feedback-api-openapi.yml
- filename: botrecipe-com-hub-api-openapi.yml
  format: yaml
  label: botrecipe-com Hub API
  slug: botrecipe-com-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-hub-api-openapi.yml
- filename: botrecipe-com-market-api-openapi.yml
  format: yaml
  label: botrecipe-com Market API
  slug: botrecipe-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-market-api-openapi.yml
- filename: botrecipe-com-premium-api-openapi.yml
  format: yaml
  label: botrecipe-com Premium API
  slug: botrecipe-com-premium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-premium-api-openapi.yml
- filename: botrecipe-com-pricing-json-api-openapi.yml
  format: yaml
  label: botrecipe-com Pricing.json API
  slug: botrecipe-com-pricing-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-pricing-json-api-openapi.yml
- filename: botrecipe-com-recipes-json-api-openapi.yml
  format: yaml
  label: botrecipe-com Recipes.json API
  slug: botrecipe-com-recipes-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-recipes-json-api-openapi.yml
- filename: botrecipe-com-search-api-openapi.yml
  format: yaml
  label: botrecipe-com Search API
  slug: botrecipe-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-search-api-openapi.yml
- filename: botrecipe-com-stats-api-openapi.yml
  format: yaml
  label: botrecipe-com Stats API
  slug: botrecipe-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-stats-api-openapi.yml
- filename: botrecipe-com-submit-api-openapi.yml
  format: yaml
  label: botrecipe-com Submit API
  slug: botrecipe-com-submit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-submit-api-openapi.yml
- filename: botrecipe-com-top-up-api-openapi.yml
  format: yaml
  label: botrecipe-com Top Up API
  slug: botrecipe-com-top-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botrecipe-com/openapi/botrecipe-com-top-up-api-openapi.yml
consequence_counts:
  physical: 2
  read: 10
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Botrecipe Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/market
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/topup
operation_count: 17
overview: 'botrecipe-com exposes 17 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: botrecipe-com
provider_slug: botrecipe-com
slug: botrecipe-com-agentic-access
source_filename: botrecipe-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/botrecipe-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 10\n    acting: 7\n  by_consequence:\n    read: 10\n    write: 5\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /recipes.json\n  method: get\n  operationId: listRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/index.json\n  method: get\n  operationId: searchIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board\n\
  \  method: get\n  operationId: getBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feedback\n  method: post\n  operationId: postFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/submit\n  method: post\n  operationId: submitRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/comment\n  method: post\n  operationId: postComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/comments\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hub\n  method: get\n  operationId: hubRead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hub\n  method: post\n  operationId: hubWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/market\n  method: get\n  operationId: marketRead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/market\n  method: post\n  operationId: marketWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent-auth\n  method: post\n  operationId: agentAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/premium\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topup\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/topup\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://artifacts.apis.io/botrecipe-com/agentic-access/botrecipe-com-agentic-access.yml
summary_line: 17 operations · 7 acting
tags:
- Company
- Bot
- Chatbots
- Recipes
- Automation
- Integration
---
