---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 34
api_specs:
- filename: shlink-domains-api-openapi.yml
  format: yaml
  label: Shlink Domains API
  slug: shlink-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-domains-api-openapi.yml
- filename: shlink-integrations-api-openapi.yml
  format: yaml
  label: Shlink Integrations API
  slug: shlink-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-integrations-api-openapi.yml
- filename: shlink-monitoring-api-openapi.yml
  format: yaml
  label: Shlink Monitoring API
  slug: shlink-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-monitoring-api-openapi.yml
- filename: shlink-redirect-rules-api-openapi.yml
  format: yaml
  label: Shlink Redirect rules API
  slug: shlink-redirect-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-redirect-rules-api-openapi.yml
- filename: shlink-short-urls-api-openapi.yml
  format: yaml
  label: Shlink Short URLs API
  slug: shlink-short-urls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-short-urls-api-openapi.yml
- filename: shlink-tags-api-openapi.yml
  format: yaml
  label: Shlink Tags API
  slug: shlink-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-tags-api-openapi.yml
- filename: shlink-url-shortener-api-openapi.yml
  format: yaml
  label: Shlink URL Shortener API
  slug: shlink-url-shortener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-url-shortener-api-openapi.yml
- filename: shlink-visits-api-openapi.yml
  format: yaml
  label: Shlink Visits API
  slug: shlink-visits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-visits-api-openapi.yml
consequence_counts:
  read: 34
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shlink Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 52
overview: 'Shlink exposes 52 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shlink
provider_slug: shlink
slug: shlink-agentic-access
source_filename: shlink-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/shlink-openapi-v5.1.0.json, openapi/shlink-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 34\n    acting: 18\n  by_consequence:\n    read: 34\n    write: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /rest/v{version}/short-urls\n  method: get\n  operationId: listShortUrls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls\n  method: post\n  operationId: createShortUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/short-urls/shorten\n  method: get\n  operationId: shortenUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}\n  method: get\n  operationId: getShortUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}\n  method: delete\n  operationId: deleteShortUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /rest/v{version}/short-urls/{shortCode}\n  method: patch\n  operationId: editShortUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/short-urls/{shortCode}/redirect-rules\n  method: get\n  operationId: listShortUrlRedirectRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}/redirect-rules\n  method: post\n  operationId: setShortUrlRedirectRules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /rest/v{version}/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/tags\n  method: put\n  operationId: renameTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/tags\n  method: delete\n  operationId: deleteTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/tags/stats\n  method:\
  \ get\n  operationId: tagsWithStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/visits\n  method: get\n  operationId: getGlobalVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}/visits\n  method: get\n  operationId: getShortUrlVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}/visits\n  method: delete\n  operationId: deleteShortUrlVisits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /rest/v{version}/tags/{tag}/visits\n  method: get\n  operationId: getTagVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/domains/{domain}/visits\n  method: get\n  operationId: getDomainVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/visits/orphan\n  method: get\n  operationId: getOrphanVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/visits/orphan\n  method: delete\n  operationId: deleteOrphanVisits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/visits/non-orphan\n  method: get\n  operationId: getNonOrphanVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/domains/redirects\n  method: patch\n  operationId: setDomainRedirects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/mercure-info\n  method:\
  \ get\n  operationId: mercureInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{shortCode}\n  method: get\n  operationId: shortUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{shortCode}/track\n  method: get\n  operationId: trackShortUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls\n  method: get\n  operationId: listShortUrls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls\n  method: post\n  operationId: createShortUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/short-urls/shorten\n  method: get\n  operationId: shortenUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}\n  method: get\n  operationId: getShortUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}\n  method: delete\n  operationId: deleteShortUrl\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/short-urls/{shortCode}\n  method: patch\n  operationId: editShortUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/short-urls/{shortCode}/redirect-rules\n  method: get\n  operationId: listShortUrlRedirectRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}/redirect-rules\n  method: post\n  operationId: setShortUrlRedirectRules\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/tags\n  method: put\n  operationId: renameTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/tags\n  method: delete\n  operationId: deleteTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/tags/stats\n  method: get\n  operationId: tagsWithStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/visits\n  method: get\n  operationId: getGlobalVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}/visits\n  method: get\n  operationId: getShortUrlVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/short-urls/{shortCode}/visits\n  method: delete\n  operationId: deleteShortUrlVisits\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/tags/{tag}/visits\n  method: get\n  operationId: getTagVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/domains/{domain}/visits\n  method: get\n  operationId: getDomainVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/visits/orphan\n  method: get\n  operationId: getOrphanVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/visits/orphan\n\
  \  method: delete\n  operationId: deleteOrphanVisits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/visits/non-orphan\n  method: get\n  operationId: getNonOrphanVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v{version}/domains/redirects\n  method: patch\n  operationId: setDomainRedirects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v{version}/mercure-info\n  method: get\n  operationId: mercureInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{shortCode}\n  method: get\n  operationId: shortUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{shortCode}/track\n  method: get\n  operationId: trackShortUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/shlink/agentic-access/shlink-agentic-access.yml
summary_line: 52 operations · 18 acting
tags:
- Company
- URL Shorteners
- PHP
- Self-Hosted
- Open Source
- REST API
---
