---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: 3bar-biologics-posts-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Posts API
  slug: 3bar-biologics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-posts-api-openapi.yml
- filename: 3bar-biologics-pages-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Pages API
  slug: 3bar-biologics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-pages-api-openapi.yml
- filename: 3bar-biologics-media-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Media API
  slug: 3bar-biologics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-media-api-openapi.yml
- filename: 3bar-biologics-taxonomy-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Taxonomy API
  slug: 3bar-biologics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-taxonomy-api-openapi.yml
- filename: 3bar-biologics-users-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Users API
  slug: 3bar-biologics-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-users-api-openapi.yml
- filename: 3bar-biologics-search-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Search API
  slug: 3bar-biologics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-search-api-openapi.yml
- filename: 3bar-biologics-discovery-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Discovery API
  slug: 3bar-biologics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-discovery-api-openapi.yml
- filename: 3bar-biologics-oembed-api-openapi.yml
  format: yaml
  label: 3Bar Biologics oEmbed API
  slug: 3bar-biologics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-oembed-api-openapi.yml
- filename: 3bar-biologics-seo-api-openapi.yml
  format: yaml
  label: 3Bar Biologics SEO Metadata API
  slug: 3bar-biologics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-seo-api-openapi.yml
consequence_counts: {}
description: Recommended x-agentic-access contracts for the 3Bar Biologics public content API, classified per operation. This is a RECOMMENDATION authored by API Evangelist, not a contract the provider publishes — 3Bar Biologics makes no statement about agent access at all. The classification is unusually simple here because the entire anonymously reachable surface is read-only.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 3Bar Biologics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: '3Bar Biologics exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 3Bar Biologics
provider_slug: 3bar-biologics
slug: 3bar-biologics-agentic-access
source_filename: 3bar-biologics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: generated\nsource: openapi/ + authentication/ + conventions/\ndescription: >-\n  Recommended x-agentic-access contracts for the 3Bar Biologics public content API, classified per\n  operation. This is a RECOMMENDATION authored by API Evangelist, not a contract the provider\n  publishes — 3Bar Biologics makes no statement about agent access at all. The classification is\n  unusually simple here because the entire anonymously reachable surface is read-only.\nposture:\n  overall: safe-read-only\n  detail: >-\n    All 19 documented operations are GET. Every mutating route on the underlying WordPress install\n    returns 401 without a WordPress application password, and that credential has no public issuance\n    path, so no agent operating anonymously can change anything. An agent needs no consent gate, no\n    spend cap, no escalation path and no reversal plan for this surface.\n  robots_signal:\n    x_robots_tag: noindex\n    detail: >-\n     \
  \ Every API response carries `X-Robots-Tag: noindex`. This is an indexing directive rather than an\n      access prohibition, and it is served on the API responses rather than in robots.txt, but it is\n      the only signal the provider gives about machine consumption of this data. An agent should read\n      freely and refrain from republishing the content as indexable material.\n  robots_txt:\n    url: https://www.3barbiologics.com/robots.txt\n    http_status: 200\n    detail: A Yoast-generated robots.txt is served. No /wp-json/ disallow was present.\ndefault_contract:\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  reversible: na\n  rate_guidance: >-\n    No published limits and no rate-limit response headers. Self-throttle. Responses are cached for 7\n    days at the edge, so a cache-respecting agent generates almost no origin load.\noperations:\n- {operationId: listPosts, action_class: read, consequence: none, token:\
  \ none, escalation: not-required}\n- {operationId: getPost, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: listPages, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: getPage, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: listCategories, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: getCategory, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: listTags, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: getTag, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: listUsers, action_class: read, consequence: none, token: none, escalation: not-required,\n   note: 'Returns named individuals (3 public authors). Personal data in the sense that it is attributable to a person,\
  \ though it is published deliberately as bylines. Do not aggregate it into a contact dataset.'}\n- {operationId: getUser, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: searchContent, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: listMediaItems, action_class: read, consequence: none, token: none, escalation: not-required,\n   reliability: degraded,\n   note: 'Two reproducible defects — HTTP 500 on ascending numeric/date sorts, and an advertised total that does not match retrievable records. An agent must not treat an empty 200 here as collection-exhausted. See errors/3bar-biologics-problem-types.yml.'}\n- {operationId: getMediaItem, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: getApiRoot, action_class: read, consequence: none, token: none, escalation: not-required,\n   note: 'Roughly 340KB. Fetch once and cache; do not poll.'}\n- {operationId:\
  \ listTypes, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: listTaxonomies, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: listStatuses, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: getOembed, action_class: read, consequence: none, token: none, escalation: not-required}\n- {operationId: getSeoHead, action_class: read, consequence: none, token: none, escalation: not-required,\n   note: 'Returns 404 with a populated, parseable body. Branch on status, not body shape.'}\nunreachable_write_surface:\n  detail: >-\n    The underlying WordPress install registers POST/PUT/PATCH/DELETE on posts, pages, media,\n    taxonomies, users, blocks, menus, widgets, templates and settings. None is reachable\n    anonymously — all return 401. They are listed here only so that a future re-profile does not\n    mistake their absence from the operations list above for\
  \ an incomplete harvest.\n  credential_required: WordPress application password (Basic over TLS)\n  public_issuance_path: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/agentic-access/3bar-biologics-agentic-access.yml
summary_line: 19 operations
tags:
- Company
- Agriculture
- AgTech
- Biotechnology
- Agricultural Biologicals
- Biomanufacturing
- CDMO
- Microbials
- Crop Inputs
- Sustainability
- Contract Manufacturing
- Content
---
