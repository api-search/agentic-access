---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: fullenrich-openapi.yml
  format: yaml
  label: FullEnrich Contact Enrichment API
  slug: fullenrich-contact-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-openapi.yml
- filename: fullenrich-openapi.yml
  format: yaml
  label: FullEnrich Enrichment Results API
  slug: fullenrich-enrichment-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-openapi.yml
- filename: fullenrich-openapi.yml
  format: yaml
  label: FullEnrich Reverse Email Lookup API
  slug: fullenrich-reverse-email-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-openapi.yml
- filename: fullenrich-openapi.yml
  format: yaml
  label: FullEnrich Account Credits API
  slug: fullenrich-account-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fullenrich Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'FullEnrich exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FullEnrich
provider_slug: fullenrich
slug: fullenrich-agentic-access
source_filename: fullenrich-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fullenrich-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 2\n    connected: 5\n  by_consequence:\n    write: 2\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /contact/enrich/bulk\n  method: post\n  operationId: startBulkEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/enrich/bulk\n  method: get\n  operationId: getBulkEnrichmentByQuery\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact/enrich/bulk/{enrichment_id}\n  method: get\n  operationId: getBulkEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contact/reverse/email/bulk\n  method: post\n  operationId: startReverseEmailLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact/reverse/email/bulk\n  method: get\n  operationId: getReverseEmailLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/credits\n  method: get\n  operationId:\
  \ getAccountCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/keys/verify\n  method: get\n  operationId: verifyApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/agentic-access/fullenrich-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- B2B Data
- Contact Enrichment
- Email Finder
- Phone Finder
- Waterfall Enrichment
- Sales Intelligence
---
