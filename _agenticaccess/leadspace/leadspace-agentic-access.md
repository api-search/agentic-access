---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 3
api_specs:
- filename: leadspace-enrichment-openapi.yml
  format: yaml
  label: Leadspace Enrichment API
  slug: leadspace-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-enrichment-openapi.yml
- filename: leadspace-discovery-openapi.yml
  format: yaml
  label: Leadspace Discovery API
  slug: leadspace-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-discovery-openapi.yml
- filename: leadspace-intent-openapi.yml
  format: yaml
  label: Leadspace Intent Only API
  slug: leadspace-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-intent-openapi.yml
consequence_counts:
  read: 3
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Leadspace Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Leadspace exposes 9 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Leadspace
provider_slug: leadspace
slug: leadspace-agentic-access
source_filename: leadspace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/leadspace-discovery-openapi.yml, openapi/leadspace-enrichment-openapi.yml, openapi/leadspace-intent-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 6\n    connected: 3\n  by_consequence:\n    write: 6\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/expansion/company\n  method: post\n  operationId: discoverCompanyContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/expansion/results/{bulkId}\n\
  \  method: get\n  operationId: getDiscoveryResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/authorize\n  method: post\n  operationId: createAuthorizationToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/authorize\n  method: put\n  operationId: refreshAuthorizationToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrichment/enrich/single\n  method: post\n  operationId: enrichSingleRecord\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrichment/enrich/bulk\n  method: post\n  operationId: enrichBulkRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/enrichment/results/{bulkId}\n  method: get\n  operationId: getBulkEnrichmentResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/intent/score/\n  method: post\n  operationId: scoreCompanyIntent\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/intent/results/{jobId}\n  method: get\n  operationId: getIntentResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/agentic-access/leadspace-agentic-access.yml
summary_line: 9 operations · 6 acting
tags:
- B2B Data
- Customer Data Platform
- Data Enrichment
- Intent Data
- Sales Intelligence
- Account-Based Marketing
- Identity Resolution
- Firmographics
- Lead Scoring
- Company
---
