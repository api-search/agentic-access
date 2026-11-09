---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 27
api_specs:
- filename: beliefstate-ai-access-api-openapi.yml
  format: yaml
  label: BeliefState Access API
  slug: beliefstate-ai-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-access-api-openapi.yml
- filename: beliefstate-ai-beliefs-api-openapi.yml
  format: yaml
  label: BeliefState Beliefs API
  slug: beliefstate-ai-beliefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-beliefs-api-openapi.yml
- filename: beliefstate-ai-brief-api-openapi.yml
  format: yaml
  label: BeliefState Brief API
  slug: beliefstate-ai-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-brief-api-openapi.yml
- filename: beliefstate-ai-research-api-openapi.yml
  format: yaml
  label: BeliefState Research API
  slug: beliefstate-ai-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-research-api-openapi.yml
- filename: beliefstate-ai-research-payments-api-openapi.yml
  format: yaml
  label: BeliefState Research payments API
  slug: beliefstate-ai-research-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-research-payments-api-openapi.yml
- filename: beliefstate-ai-sources-api-openapi.yml
  format: yaml
  label: BeliefState Sources API
  slug: beliefstate-ai-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-sources-api-openapi.yml
- filename: beliefstate-ai-tickers-api-openapi.yml
  format: yaml
  label: BeliefState Tickers API
  slug: beliefstate-ai-tickers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beliefstate-ai/openapi/beliefstate-ai-tickers-api-openapi.yml
consequence_counts:
  physical: 13
  read: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Beliefstate Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/compare_beliefs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/evaluate_belief_scenario
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/get_author_track_record
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/get_belief
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/get_belief_catalysts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/get_belief_changes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/get_belief_relationships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/get_belief_risks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/get_brief
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/get_context_assessment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/get_research_visual
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/mcp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/research/refresh_market_data
operation_count: 40
overview: 'BeliefState exposes 40 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 13 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BeliefState
provider_slug: beliefstate-ai
slug: beliefstate-ai-agentic-access
source_filename: beliefstate-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/beliefstate-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 27\n    acting: 13\n  by_consequence:\n    read: 27\n    physical: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/brief\n  method: get\n  operationId: getBrief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beliefs\n  method: get\n  operationId: getBeliefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tickers\n  method: get\n  operationId:\
  \ getTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research\n  method: get\n  operationId: getX402ResearchCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/mcp\n  method: post\n  operationId: callX402ResearchMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/get_belief_risks\n  method: get\n  operationId: getX402Contract_get_belief_risks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_belief_risks\n  method: post\n  operationId: purchaseResearch_get_belief_risks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/get_belief_catalysts\n  method: get\n  operationId: getX402Contract_get_belief_catalysts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_belief_catalysts\n  method: post\n  operationId: purchaseResearch_get_belief_catalysts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/get_author_track_record\n  method: get\n  operationId: getX402Contract_get_author_track_record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_author_track_record\n  method: post\n  operationId: purchaseResearch_get_author_track_record\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/search_beliefs\n  method: get\n  operationId: getX402Contract_search_beliefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/search_beliefs\n  method: post\n  operationId: purchaseResearch_search_beliefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_belief\n  method: get\n  operationId: getX402Contract_get_belief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/research/get_belief\n  method: post\n  operationId: purchaseResearch_get_belief\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/compare_beliefs\n  method: get\n  operationId: getX402Contract_compare_beliefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/compare_beliefs\n  method: post\n  operationId: purchaseResearch_compare_beliefs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/get_brief\n  method: get\n  operationId: getX402Contract_get_brief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_brief\n  method: post\n  operationId: purchaseResearch_get_brief\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/get_beliefs\n  method: get\n  operationId: getX402Contract_get_beliefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/research/get_beliefs\n  method: post\n  operationId: purchaseResearch_get_beliefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/search_entities\n  method: get\n  operationId: getX402Contract_search_entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/search_entities\n  method: post\n  operationId: purchaseResearch_search_entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_belief_changes\n  method: get\n  operationId: getX402Contract_get_belief_changes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v1/research/get_belief_changes\n  method: post\n  operationId: purchaseResearch_get_belief_changes\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/get_context_assessment\n  method: get\n  operationId: getX402Contract_get_context_assessment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_context_assessment\n  method: post\n  operationId: purchaseResearch_get_context_assessment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/list_research_visuals\n  method: get\n  operationId: getX402Contract_list_research_visuals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/list_research_visuals\n  method: post\n  operationId: purchaseResearch_list_research_visuals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_research_visual\n  method: get\n  operationId: getX402Contract_get_research_visual\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_research_visual\n  method: post\n\
  \  operationId: purchaseResearch_get_research_visual\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/get_belief_relationships\n  method: get\n  operationId: getX402Contract_get_belief_relationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/get_belief_relationships\n  method: post\n  operationId: purchaseResearch_get_belief_relationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/evaluate_belief_scenario\n  method: get\n  operationId: getX402Contract_evaluate_belief_scenario\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/evaluate_belief_scenario\n  method: post\n  operationId: purchaseResearch_evaluate_belief_scenario\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research/refresh_market_data\n  method: get\n  operationId: getX402Contract_refresh_market_data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/research/refresh_market_data\n  method: post\n  operationId: purchaseResearch_refresh_market_data\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/brief/{ticker}\n  method: get\n  operationId: purchaseTickerOverviewWithX402\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/beliefstate-ai/agentic-access/beliefstate-ai-agentic-access.yml
summary_line: 40 operations · 13 acting
tags:
- Artificial Intelligence
- Finance
- Research
- Analytics
- Platform
---
