---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: google-search-console-api-openapi.yml
  format: yaml
  label: Google Search Console API
  slug: google-search-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-api-openapi.yml
consequence_counts:
  read: 4
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Search Console Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Google Search Console exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Search Console
provider_slug: google-search-console
slug: google-search-console-agentic-access
source_filename: google-search-console-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-search-console-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 4\n    acting: 6\n  by_consequence:\n    read: 4\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /webmasters/v3/sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/webmasters.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webmasters/v3/sites/{siteUrl}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - https://www.googleapis.com/auth/webmasters.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webmasters/v3/sites/{siteUrl}\n  method: put\n  operationId: addSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /webmasters/v3/sites/{siteUrl}\n  method: delete\n  operationId: deleteSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /webmasters/v3/sites/{siteUrl}/searchAnalytics/query\n\
  \  method: post\n  operationId: querySearchAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /webmasters/v3/sites/{siteUrl}/sitemaps\n  method: get\n  operationId: listSitemaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/webmasters.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webmasters/v3/sites/{siteUrl}/sitemaps/{feedpath}\n  method: get\n  operationId: getSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/webmasters.readonly\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /webmasters/v3/sites/{siteUrl}/sitemaps/{feedpath}\n  method: put\n  operationId: submitSitemap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /webmasters/v3/sites/{siteUrl}/sitemaps/{feedpath}\n  method: delete\n  operationId: deleteSitemap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /v1/urlInspection/index:inspect\n  method: post\n  operationId: inspectUrl\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/agentic-access/google-search-console-agentic-access.yml
summary_line: 10 operations · 6 acting
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
---
