---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
api_specs:
- filename: google-search-console-search-analytics-api-openapi.yml
  format: yaml
  label: Google Search Console Search Analytics API
  slug: google-search-console-search-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-search-analytics-api-openapi.yml
- filename: google-search-console-sitemaps-api-openapi.yml
  format: yaml
  label: Google Search Console Sitemaps API
  slug: google-search-console-sitemaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-sitemaps-api-openapi.yml
- filename: google-search-console-sites-api-openapi.yml
  format: yaml
  label: Google Search Console Sites API
  slug: google-search-console-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-sites-api-openapi.yml
- filename: google-search-console-url-inspection-api-openapi.yml
  format: yaml
  label: Google Search Console URL Inspection API
  slug: google-search-console-url-inspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-url-inspection-api-openapi.yml
- filename: google-search-console-urlnotifications-api-openapi.yml
  format: yaml
  label: Google Search Console URL Notifications API
  slug: google-search-console-urlnotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-urlnotifications-api-openapi.yml
- filename: google-search-console-urltestingtools-api-openapi.yml
  format: yaml
  label: Google Search Console URL Testing Tools API
  slug: google-search-console-urltestingtools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/openapi/google-search-console-urltestingtools-api-openapi.yml
consequence_counts:
  read: 6
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Search Console Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Google Search Console exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Search Console
provider_slug: google-search-console
slug: google-search-console-agentic-access
source_filename: google-search-console-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/google-search-console-search-analytics-api-openapi.yml, openapi/google-search-console-sitemaps-api-openapi.yml,\n  openapi/google-search-console-sites-api-openapi.yml, openapi/google-search-console-url-inspection-api-openapi.yml,\n  openapi/google-search-console-urlnotifications-api-openapi.yml, openapi/google-search-console-urltestingtools-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 6\n    acting: 7\n  by_consequence:\n    read: 6\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /webmasters/v3/sites/{siteUrl}/searchAnalytics/query\n  method: post\n  operationId: querySearchAnalytics\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /webmasters/v3/sites/{siteUrl}/sitemaps\n  method: get\n  operationId: listSitemaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/webmasters.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webmasters/v3/sites/{siteUrl}/sitemaps/{feedpath}\n  method: get\n  operationId: getSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/webmasters.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webmasters/v3/sites/{siteUrl}/sitemaps/{feedpath}\n  method: put\n  operationId: submitSitemap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /webmasters/v3/sites/{siteUrl}/sitemaps/{feedpath}\n  method: delete\n  operationId: deleteSitemap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /webmasters/v3/sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/webmasters.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /webmasters/v3/sites/{siteUrl}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/webmasters.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webmasters/v3/sites/{siteUrl}\n  method: put\n  operationId: addSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /webmasters/v3/sites/{siteUrl}\n  method: delete\n  operationId: deleteSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /v1/urlInspection/index:inspect\n  method: post\n  operationId: inspectUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n- path: /v3/urlNotifications:publish\n  method: post\n  operationId: indexing_urlNotifications_publish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/indexing\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v3/urlNotifications/metadata\n  method: get\n  operationId: indexing_urlNotifications_getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/indexing\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/urlTestingTools/mobileFriendlyTest:run\n  method: post\n  operationId: searchconsole_urlTestingTools_mobileFriendlyTest_run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/webmasters\n    - https://www.googleapis.com/auth/webmasters.readonly\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/agentic-access/google-search-console-agentic-access.yml
summary_line: 13 operations · 7 acting
tags:
- Analytics
- Google
- Indexing
- Search
- Search Analytics
- SEO
- Sitemap
- URL Inspection
- Webmaster Tools
---
