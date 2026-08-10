---
acting_count: 0
action_class_counts:
  connected: 23
api_specs:
- filename: accelsius-content-api-openapi.yml
  format: yaml
  label: Accelsius Resources Content API
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-content-api-openapi.yml
- filename: accelsius-news-api-openapi.yml
  format: yaml
  label: Accelsius News API
  slug: news
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-news-api-openapi.yml
- filename: accelsius-pages-api-openapi.yml
  format: yaml
  label: Accelsius Pages API
  slug: pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-pages-api-openapi.yml
- filename: accelsius-media-api-openapi.yml
  format: yaml
  label: Accelsius Media API
  slug: media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-media-api-openapi.yml
- filename: accelsius-search-api-openapi.yml
  format: yaml
  label: Accelsius Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-search-api-openapi.yml
- filename: accelsius-discovery-api-openapi.yml
  format: yaml
  label: Accelsius API Discovery
  slug: discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-discovery-api-openapi.yml
- filename: accelsius-categories-api-openapi.yml
  format: yaml
  label: Accelsius Categories API
  slug: accelsius-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-categories-api-openapi.yml
- filename: accelsius-media-folders-api-openapi.yml
  format: yaml
  label: Accelsius Media Folders API
  slug: accelsius-media-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-media-folders-api-openapi.yml
- filename: accelsius-registry-api-openapi.yml
  format: yaml
  label: Accelsius Registry API
  slug: accelsius-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-registry-api-openapi.yml
- filename: accelsius-tags-api-openapi.yml
  format: yaml
  label: Accelsius Tags API
  slug: accelsius-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/openapi/accelsius-tags-api-openapi.yml
consequence_counts:
  read: 23
description: 'Recommended x-agentic-access execution contracts, classified from the OpenAPI. A governance starting point for exposing this surface to AI agents — review and bind audience per deployment. Classification is trivially uniform here: every documented operation is an unauthenticated GET over published marketing content, so every one is connected/read with no human in the loop. The real agent risk on this surface is not consequence, it is CADENCE — see the throttling contract below.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Accelsius Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Accelsius exposes 23 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Accelsius
provider_slug: accelsius
slug: accelsius-agentic-access
source_filename: accelsius-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/accelsius-content-api-openapi.yml, openapi/accelsius-discovery-api-openapi.yml, openapi/accelsius-media-api-openapi.yml,\n  openapi/accelsius-news-api-openapi.yml, openapi/accelsius-pages-api-openapi.yml, openapi/accelsius-search-api-openapi.yml,\n  openapi/accelsius-taxonomy-api-openapi.yml\ndescription: 'Recommended x-agentic-access execution contracts, classified from the OpenAPI. A governance\n  starting point for exposing this surface to AI agents — review and bind audience per deployment. Classification\n  is trivially uniform here: every documented operation is an unauthenticated GET over published marketing\n  content, so every one is connected/read with no human in the loop. The real agent risk on this surface\n  is not consequence, it is CADENCE — see the throttling contract below.'\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 23\n  by_consequence:\n    read: 23\n  human_in_the_loop_required:\
  \ 0\nx-agentic-throttle:\n  crawl_delay_seconds: 10\n  max_concurrency: 1\n  cache_seconds: 600\n  rate_limit_signalled: false\n  enforcement: Behavioural. The MalCare WordPress firewall on this origin answers HTTP 403 with a text/html\n    interstitial and no Retry-After once it classifies a client as hostile; the block persisted across\n    a user-agent change during profiling. No RateLimit-* or X-RateLimit-* header is published, so an agent\n    cannot discover the budget in band.\n  agent_rule: Prefer collection reads with _fields and _embed over per-item fetches; the entire site is\n    1,095 objects reachable in 12 collection requests. On any 403, halt the plan and escalate rather than\n    retry — a retry loop here converts a soft block into a persistent one.\nexcluded_operations:\n- path: /wp/v2/users\n  method: get\n  status: 200\n  reason: Anonymously readable directory of 14 named site authors. Never modelled as an operation, never\n    exposed as an agent-callable surface.\
  \ Recorded so the exclusion is legible to a governance reviewer\n    rather than looking like an oversight.\noperations:\n- path: /wp/v2/posts\n  method: get\n  operationId: listContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getContentItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getRootIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2\n  method: get\n  operationId: getWpV2Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId:\
  \ listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/news\n  method: get\n  operationId: listNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/news/{id}\n  method: get\n  operationId: getNewsItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: searchSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/happyfiles_category\n  method: get\n  operationId: listMediaFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/happyfiles_category/{id}\n  method: get\n  operationId: getMediaFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listPostTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n\
  \  operationId: getPostType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelsius/refs/heads/main/agentic-access/accelsius-agentic-access.yml
summary_line: 23 operations
tags:
- Company
- Data Centers
- Liquid Cooling
- Thermal Management
- Direct-to-Chip Cooling
- Two-Phase Cooling
- Artificial Intelligence Infrastructure
- High Performance Computing
- Hardware
- Manufacturing
- Content
- WordPress
---
