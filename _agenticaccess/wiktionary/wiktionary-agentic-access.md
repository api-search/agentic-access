---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 21
api_specs:
- filename: wiktionary-mediawiki-action-api-openapi-original.yml
  format: yaml
  label: MediaWiki Action API (Wiktionary)
  slug: mediawiki-action-api-wiktionary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-mediawiki-action-api-openapi-original.yml
- filename: wiktionary-rest-api-openapi-original.yml
  format: yaml
  label: Wikimedia REST API (Wiktionary)
  slug: wikimedia-rest-api-wiktionary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-rest-api-openapi-original.yml
- filename: wiktionary-core-rest-api-openapi-original.yml
  format: yaml
  label: MediaWiki Core REST API (Wiktionary)
  slug: mediawiki-core-rest-api-wiktionary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-core-rest-api-openapi-original.yml
consequence_counts:
  read: 21
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wiktionary Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Wiktionary exposes 24 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wiktionary
provider_slug: wiktionary
slug: wiktionary-agentic-access
source_filename: wiktionary-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wiktionary-core-rest-api-openapi-original.yml, openapi/wiktionary-mediawiki-action-api-openapi-original.yml,\n  openapi/wiktionary-rest-api-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 21\n    acting: 3\n  by_consequence:\n    read: 21\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/page/{title}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/page/{title}/html\n  method: get\n  operationId: getPageHtml\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/page/{title}/with_html\n  method: get\n  operationId: getPageWithHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/page/{title}/history\n  method: get\n  operationId: getPageHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/page/{title}/history/counts/{type}\n  method: get\n  operationId: getPageHistoryCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/revision/{id}/bare\n  method: get\n  operationId: getRevisionBare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/search/page\n  method: get\n  operationId: searchPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search/title\n  method: get\n  operationId: searchTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/file/{title}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php\n  method: get\n  operationId: queryAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php#query-wikitext\n  method: get\n  operationId: queryWikitext\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php#query-extracts\n  method: get\n  operationId: queryExtracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php#query-search\n  method: get\n  operationId: querySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php#parse\n  method: get\n  operationId: parsePage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php#opensearch\n  method: get\n  operationId: openSearchSuggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api.php#expandtemplates\n  method:\
  \ get\n  operationId: expandTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page/definition/{term}\n  method: get\n  operationId: getDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page/summary/{title}\n  method: get\n  operationId: getPageSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page/html/{title}\n  method: get\n  operationId: getPageHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page/title/{title}\n  method: get\n  operationId: getPageTitle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /page/mobile-html/{title}\n  method: get\n  operationId: getPageMobileHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transform/wikitext/to/html/{title}\n  method: post\n  operationId: transformWikitextToHtml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transform/html/to/wikitext/{title}/{revision}\n  method: post\n  operationId: transformHtmlToWikitext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /transform/wikitext/to/lint/{title}\n  method: post\n  operationId: transformWikitextToLint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/agentic-access/wiktionary-agentic-access.yml
summary_line: 24 operations · 3 acting
tags:
- Dictionaries
- Open Source
- Wikimedia
- MediaWiki
- Linguistics
- Open Data
- Public APIs
---
