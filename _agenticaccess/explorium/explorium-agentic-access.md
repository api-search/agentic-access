---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 3
api_specs:
- filename: explorium-openapi.yml
  format: yaml
  label: Explorium Business Enrichment API
  slug: explorium-business-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-openapi.yml
- filename: explorium-openapi.yml
  format: yaml
  label: Explorium Prospect Enrichment API
  slug: explorium-prospect-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-openapi.yml
- filename: explorium-openapi.yml
  format: yaml
  label: Explorium Matching API
  slug: explorium-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-openapi.yml
- filename: explorium-openapi.yml
  format: yaml
  label: Explorium Autocomplete API
  slug: explorium-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-openapi.yml
- filename: explorium-openapi.yml
  format: yaml
  label: Explorium Business and Prospect Events API
  slug: explorium-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/openapi/explorium-openapi.yml
consequence_counts:
  read: 3
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Explorium Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Explorium exposes 17 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Explorium
provider_slug: explorium
slug: explorium-agentic-access
source_filename: explorium-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/explorium-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 14\n    connected: 3\n  by_consequence:\n    write: 14\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/businesses/match\n  method: post\n  operationId: matchBusinesses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses\n  method: post\n  operationId: fetchBusinesses\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/stats\n  method: post\n  operationId: fetchBusinessStats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/autocomplete\n  method: get\n  operationId: autocompleteBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/firmographics/enrich\n  method: post\n  operationId: enrichFirmographics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/technographics/enrich\n  method: post\n  operationId: enrichTechnographics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/firmographics/bulk_enrich\n  method: post\n  operationId: bulkEnrichFirmographics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/events\n  method: post\n\
  \  operationId: fetchBusinessEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/prospects/match\n  method: post\n  operationId: matchProspects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/prospects\n  method: post\n  operationId: fetchProspects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/prospects/stats\n  method: post\n  operationId: fetchProspectStats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/prospects/autocomplete\n  method: get\n  operationId: autocompleteProspects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prospects/contacts_information/enrich\n  method: post\n  operationId: enrichProspectContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/prospects/profiles/enrich\n\
  \  method: post\n  operationId: enrichProspectProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/prospects/events\n  method: post\n  operationId: fetchProspectEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: post\n  operationId: addWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/credits\n  method: get\n  operationId: getActiveCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/explorium/refs/heads/main/agentic-access/explorium-agentic-access.yml
summary_line: 17 operations · 14 acting
tags:
- Data Enrichment
- Web Intelligence
- Reference Data
- B2B Data
- Company Data
- AI Agents
- Prospect Enrichment
- Firmographics
- MCP
---
