---
acting_count: 6
action_class_counts:
  acting: 6
api_specs:
- filename: gouda-studios-agent-tools-openapi.json
  format: json
  label: Gouda Studios Agent Tools API
  slug: gouda-studios-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gouda-studios-agent-tools/openapi/gouda-studios-agent-tools-openapi.json
consequence_counts:
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gouda Studios Agent Tools Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Gouda Studios Agent Tools exposes 6 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gouda Studios Agent Tools
provider_slug: gouda-studios-agent-tools
slug: gouda-studios-agent-tools-agentic-access
source_filename: gouda-studios-agent-tools-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/gouda-studios-agent-tools-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 6\n  by_consequence:\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /acts/gouda_studios~sam-gov-opportunities-feed/run-sync-get-dataset-items\n  method: post\n  operationId: run_sam_gov_opportunities_feed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acts/gouda_studios~sec-edgar-filings-feed/run-sync-get-dataset-items\n\
  \  method: post\n  operationId: run_sec_edgar_filings_feed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acts/gouda_studios~usaspending-awards-search/run-sync-get-dataset-items\n  method: post\n  operationId: run_usaspending_awards_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acts/gouda_studios~gleif-company-lei-lookup/run-sync-get-dataset-items\n  method: post\n  operationId: run_gleif_company_lei_lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acts/gouda_studios~website-contact-extractor/run-sync-get-dataset-items\n  method: post\n  operationId: run_website_contact_extractor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acts/gouda_studios~youtube-transcript-extractor/run-sync-get-dataset-items\n  method: post\n  operationId: run_youtube_transcript_extractor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n"
source_yaml_url: https://artifacts.apis.io/gouda-studios-agent-tools/agentic-access/gouda-studios-agent-tools-agentic-access.yml
summary_line: 6 operations · 6 acting
tags:
- Data
- Government
- Finance
- Pay-per-result
---
