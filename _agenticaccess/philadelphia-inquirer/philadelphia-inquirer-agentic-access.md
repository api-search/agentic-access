---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 10
api_specs:
- filename: rss-openapi.yml
  format: yaml
  label: The Philadelphia Inquirer RSS Feeds
  slug: rss
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/philadelphia-inquirer/refs/heads/main/openapi/rss-openapi.yml
- filename: sitemaps-openapi.yml
  format: yaml
  label: The Philadelphia Inquirer Sitemaps
  slug: sitemaps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/philadelphia-inquirer/refs/heads/main/openapi/sitemaps-openapi.yml
- filename: dewey-mcp-openapi.yml
  format: yaml
  label: Dewey MCP
  slug: dewey-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/philadelphia-inquirer/refs/heads/main/openapi/dewey-mcp-openapi.yml
consequence_counts:
  read: 10
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Philadelphia Inquirer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'The Philadelphia Inquirer exposes 11 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Philadelphia Inquirer
provider_slug: philadelphia-inquirer
slug: philadelphia-inquirer-agentic-access
source_filename: philadelphia-inquirer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dewey-mcp-openapi.yml, openapi/rss-openapi.yml, openapi/sitemaps-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 1\n    connected: 10\n  by_consequence:\n    write: 1\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: postMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /livez\n  method: get\n  operationId: getLiveness\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /readyz\n  method: get\n  operationId: getReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arc/outboundfeeds/rss/\n  method: get\n  operationId: getSiteRssFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arc/outboundfeeds/rss/category/{category}/\n  method: get\n  operationId: getCategoryRssFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arc/outboundfeeds/sitemap-index-2/\n  method: get\n  operationId: getSitemapIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /arc/outboundfeeds/sitemap/latest/\n  method: get\n  operationId: getLatestSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arc/outboundfeeds/sitemap/{date}/\n  method: get\n  operationId: getDailySitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arc/outboundfeeds/news-sitemap/\n  method: get\n  operationId: getNewsSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arc/outboundfeeds/sitemap-author-page/\n  method: get\n  operationId: getAuthorSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arc/outboundfeeds/sitemap-restaurant-page/\n\
  \  method: get\n  operationId: getRestaurantSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/philadelphia-inquirer/refs/heads/main/agentic-access/philadelphia-inquirer-agentic-access.yml
summary_line: 11 operations · 1 acting
tags:
- News
- News Media
- Newspaper
- Journalism
- Philadelphia
- Pennsylvania
- Local News
- RSS
- Sitemap
- Arc Publishing
- MCP
---
