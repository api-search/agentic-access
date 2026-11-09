---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 34
api_specs:
- filename: feedam-org-analytics-api-openapi.yml
  format: yaml
  label: Feed America Analytics API
  slug: feedam-org-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-analytics-api-openapi.yml
- filename: feedam-org-autocomplete-api-openapi.yml
  format: yaml
  label: Feed America Autocomplete API
  slug: feedam-org-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-autocomplete-api-openapi.yml
- filename: feedam-org-feedback-api-openapi.yml
  format: yaml
  label: Feed America Feedback API
  slug: feedam-org-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-feedback-api-openapi.yml
- filename: feedam-org-health-api-openapi.yml
  format: yaml
  label: Feed America Health API
  slug: feedam-org-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-health-api-openapi.yml
- filename: feedam-org-hsds-api-openapi.yml
  format: yaml
  label: Feed America Hsds API
  slug: feedam-org-hsds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-hsds-api-openapi.yml
- filename: feedam-org-llm-search-api-openapi.yml
  format: yaml
  label: Feed America Llm Search API
  slug: feedam-org-llm-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-llm-search-api-openapi.yml
- filename: feedam-org-llms-full-txt-api-openapi.yml
  format: yaml
  label: Feed America Llms Full.txt API
  slug: feedam-org-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-llms-full-txt-api-openapi.yml
- filename: feedam-org-llms-txt-api-openapi.yml
  format: yaml
  label: Feed America Llms.txt API
  slug: feedam-org-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-llms-txt-api-openapi.yml
- filename: feedam-org-pantry-api-openapi.yml
  format: yaml
  label: Feed America Pantry API
  slug: feedam-org-pantry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-pantry-api-openapi.yml
- filename: feedam-org-partner-api-openapi.yml
  format: yaml
  label: Feed America Partner API
  slug: feedam-org-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-partner-api-openapi.yml
- filename: feedam-org-resources-api-openapi.yml
  format: yaml
  label: Feed America Resources API
  slug: feedam-org-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-resources-api-openapi.yml
- filename: feedam-org-sitemap-xml-api-openapi.yml
  format: yaml
  label: Feed America Sitemap.xml API
  slug: feedam-org-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-sitemap-xml-api-openapi.yml
- filename: feedam-org-sms-api-openapi.yml
  format: yaml
  label: Feed America Sms API
  slug: feedam-org-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-sms-api-openapi.yml
- filename: feedam-org-snap-api-openapi.yml
  format: yaml
  label: Feed America Snap API
  slug: feedam-org-snap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-snap-api-openapi.yml
- filename: feedam-org-stats-api-openapi.yml
  format: yaml
  label: Feed America Stats API
  slug: feedam-org-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-stats-api-openapi.yml
- filename: feedam-org-widget-api-openapi.yml
  format: yaml
  label: Feed America Widget API
  slug: feedam-org-widget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feedam-org/openapi/feedam-org-widget-api-openapi.yml
consequence_counts:
  physical: 1
  read: 34
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Feedam Org Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/sms
operation_count: 40
overview: 'Feed America exposes 40 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Feed America
provider_slug: feedam-org
slug: feedam-org-agentic-access
source_filename: feedam-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/feedam-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 34\n    acting: 6\n  by_consequence:\n    read: 34\n    write: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/llm-search\n  method: get\n  operationId: llmSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/resources/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/resources/nearby\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/resources/urgent\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/resources/counts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/resources/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/resources/{id}/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/resources/types\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/resources/bulk\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/autocomplete\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats/quality\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feedback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partner/find\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partner/edit\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sms\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/widget\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analytics/dashboard\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/snap/calculate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health/deep\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/datapackage.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /hsds/v3/organizations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/services\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/locations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/service_at_location\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/phones\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/addresses\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/schedules\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/languages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/taxonomy_terms\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hsds/v3/attributes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pantry/search\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pantry/claim\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pantry/manage/{token}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pantry/status\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/feedam-org/agentic-access/feedam-org-agentic-access.yml
summary_line: 40 operations · 6 acting
tags:
- Nonprofit
- Food Assistance
- Directory
- United States
- Community
---
