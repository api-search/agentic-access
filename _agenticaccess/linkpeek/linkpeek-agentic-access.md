---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: linkpeek-favicon-api-openapi.yml
  format: yaml
  label: LinkPeek Favicon API
  slug: linkpeek-favicon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-favicon-api-openapi.yml
- filename: linkpeek-link-preview-api-openapi.yml
  format: yaml
  label: LinkPeek Link Preview API
  slug: linkpeek-link-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-link-preview-api-openapi.yml
- filename: linkpeek-meta-tags-api-openapi.yml
  format: yaml
  label: LinkPeek Meta Tags API
  slug: linkpeek-meta-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-meta-tags-api-openapi.yml
- filename: linkpeek-qr-code-api-openapi.yml
  format: yaml
  label: LinkPeek QR Code API
  slug: linkpeek-qr-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-qr-code-api-openapi.yml
- filename: linkpeek-system-api-openapi.yml
  format: yaml
  label: LinkPeek System API
  slug: linkpeek-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/openapi/linkpeek-system-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Linkpeek Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'LinkPeek exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LinkPeek
provider_slug: linkpeek
slug: linkpeek-agentic-access
source_filename: linkpeek-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/linkpeek-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /api/preview\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/qr\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/qrcode\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/favicon-extractor\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meta-tag-parser\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/og-image\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/extract\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/metadata-full\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/batch\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/favicons\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/headers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/key\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/subscribe\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health/json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n# --- API Evangelist review note, added 2026-08-09 -------------------------------------------\n# The method-based heuristic above classified all 16 operations as connected/read because every\n# one is a GET. Two of them are NOT reads and must be overridden before this contract is used:\n#\n#   GET /api/key?email=       mints a 14-day API key        -> acting / write\n#   GET /api/subscribe?email= mints a Pro key AND starts a  -> acting / write\n#                             $1/month PayPal subscription\n#\n# Neither has an idempotency contract,\
  \ so a retry or a prefetch can mint keys or start billing.\n# Any agent policy derived from this file must move those two to action-class: acting,\n# consequence: write, audit: required, and keep them off automatic retry paths.\nreview_overrides:\n- path: /api/key\n  method: get\n  reason: side-effecting GET — issues a 14-day API key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n- path: /api/subscribe\n  method: get\n  reason: side-effecting GET — mints a Pro key and initiates a paid subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n      exchange: required\n    purpose: required\n    audit: required\n    human-in-the-loop: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkpeek/refs/heads/main/agentic-access/linkpeek-agentic-access.yml
summary_line: 16 operations
tags:
- screenshots
- webpage-capture
- website-thumbnails
- image-generation
- rendering
- web-scraping-adjacent
- developer-tools
- saas
- rest-image-api
- Developer Tools
- Utility API
- URL Metadata
- Link Preview
- OpenGraph
- QR Code Generation
- DNS
- WHOIS
- SSL
- Web Security Scanning
- IP Geolocation
- Data Conversion
- LLM-Compatible API
- api-utilities
- url-metadata
- link-preview
- qr-code-generation
- dns-whois
- web-security-scanning
- data-conversion
- openai-compatible-llm
---
