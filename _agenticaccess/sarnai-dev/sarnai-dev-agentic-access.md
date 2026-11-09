---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 22
api_specs:
- filename: sarnai-dev-concierge-api-openapi.yml
  format: yaml
  label: sarnai-dev Concierge API
  slug: sarnai-dev-concierge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-concierge-api-openapi.yml
- filename: sarnai-dev-health-api-openapi.yml
  format: yaml
  label: sarnai-dev Health API
  slug: sarnai-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-health-api-openapi.yml
- filename: sarnai-dev-listings-api-openapi.yml
  format: yaml
  label: sarnai-dev Listings API
  slug: sarnai-dev-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-listings-api-openapi.yml
- filename: sarnai-dev-llms-txt-api-openapi.yml
  format: yaml
  label: sarnai-dev Llms.txt API
  slug: sarnai-dev-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-llms-txt-api-openapi.yml
- filename: sarnai-dev-mcp-api-openapi.yml
  format: yaml
  label: sarnai-dev MCP API
  slug: sarnai-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-mcp-api-openapi.yml
- filename: sarnai-dev-reputation-api-openapi.yml
  format: yaml
  label: sarnai-dev Reputation API
  slug: sarnai-dev-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-reputation-api-openapi.yml
- filename: sarnai-dev-robots-txt-api-openapi.yml
  format: yaml
  label: sarnai-dev Robots.txt API
  slug: sarnai-dev-robots-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-robots-txt-api-openapi.yml
- filename: sarnai-dev-score-api-openapi.yml
  format: yaml
  label: sarnai-dev Score API
  slug: sarnai-dev-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-score-api-openapi.yml
- filename: sarnai-dev-verify-api-openapi.yml
  format: yaml
  label: sarnai-dev Verify API
  slug: sarnai-dev-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-verify-api-openapi.yml
- filename: sarnai-dev-well-known-api-openapi.yml
  format: yaml
  label: sarnai-dev .well Known API
  slug: sarnai-dev-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sarnai-dev/openapi/sarnai-dev-well-known-api-openapi.yml
consequence_counts:
  read: 22
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sarnai Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'sarnai-dev exposes 33 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: sarnai-dev
provider_slug: sarnai-dev
slug: sarnai-dev-agentic-access
source_filename: sarnai-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/board-openapi.json, openapi/verify-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 22\n    acting: 11\n  by_consequence:\n    read: 22\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: head\n  operationId: health_check_health_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /listings\n  method: post\n  operationId: create_listing_listings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings\n  method: get\n  operationId: browse_listings_listings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/facets\n  method: get\n  operationId: facets_listings_facets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{listing_id}\n  method: get\n  operationId: get_listing_listings__listing_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{listing_id}\n  method: patch\n  operationId: update_listing_listings__listing_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/{listing_id}\n  method: delete\n  operationId: deactivate_listing_listings__listing_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/{listing_id}/status\n  method: get\n  operationId: get_listing_status_listings__listing_id__status_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{listing_id}/recheck\n  method: post\n  operationId: recheck_listing_listings__listing_id__recheck_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/{listing_id}/template\n  method: get\n  operationId: get_template_listings__listing_id__template_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{listing_id}/ownership\n  method: get\n  operationId: ownership_instructions_listings__listing_id__ownership_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /listings/{listing_id}/claim\n  method: post\n  operationId: claim_listing_listings__listing_id__claim_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/{listing_id}/remove-imported\n  method: post\n  operationId: remove_imported_listing_listings__listing_id__remove_imported_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/{listing_id}/heartbeat\n  method: post\n  operationId: heartbeat_listing_listings__listing_id__heartbeat_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/agent-card\n  method: get\n  operationId: agent_card__well_known_agent_card_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: agent_card__well_known_agent_card_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms_txt_llms_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/{tool}\n\
  \  method: post\n  operationId: concierge_tool_concierge__tool__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: head\n  operationId: health_check_health_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/schema\n  method: post\n  operationId: verify_schema_verify_schema_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/deliverable\n  method: post\n  operationId: verify_deliverable_verify_deliverable_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/agent-card\n  method: get\n  operationId: agent_card__well_known_agent_card_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: agent_card__well_known_agent_card_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  operationId: x402_discovery_manifest__well_known_x402_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reputation/{agent_id}\n  method: get\n  operationId: get_reputation_reputation__agent_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /score/{agent_id}\n  method: get\n  operationId: get_trust_score_score__agent_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /robots.txt\n  method: get\n  operationId: robots_txt_robots_txt_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /robots.txt\n  method: head\n  operationId: robots_txt_robots_txt_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms_txt_llms_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/security.txt\n  method: get\n  operationId: security_txt__well_known_security_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/sarnai-dev/agentic-access/sarnai-dev-agentic-access.yml
summary_line: 33 operations · 11 acting
tags:
- Company
- Artificial Intelligence
- Agents
- Directory
- Platform
---
