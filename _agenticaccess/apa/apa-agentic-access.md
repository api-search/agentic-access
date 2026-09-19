---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: apa-discovery-api-openapi.yml
  format: yaml
  label: APA Corporation
  slug: apa-corporation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-discovery-api-openapi.yml
- filename: apa-ticker-api-openapi.yml
  format: yaml
  label: APA Corporation Ticker API
  slug: apa-ticker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-ticker-api-openapi.yml
- filename: apa-newsroom-api-openapi.yml
  format: yaml
  label: APA Corporation Newsroom API
  slug: apa-newsroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-newsroom-api-openapi.yml
- filename: apa-leadership-api-openapi.yml
  format: yaml
  label: APA Corporation Leadership API
  slug: apa-leadership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-leadership-api-openapi.yml
- filename: apa-pages-api-openapi.yml
  format: yaml
  label: APA Corporation Pages API
  slug: apa-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-pages-api-openapi.yml
- filename: apa-feed-items-api-openapi.yml
  format: yaml
  label: APA Corporation Feed Items API
  slug: apa-feed-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-feed-items-api-openapi.yml
- filename: apa-taxonomy-api-openapi.yml
  format: yaml
  label: APA Corporation Taxonomy API
  slug: apa-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-taxonomy-api-openapi.yml
- filename: apa-authors-api-openapi.yml
  format: yaml
  label: APA Corporation Authors API
  slug: apa-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-authors-api-openapi.yml
- filename: apa-search-api-openapi.yml
  format: yaml
  label: APA Corporation Search API
  slug: apa-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-search-api-openapi.yml
- filename: apa-media-api-openapi.yml
  format: yaml
  label: APA Corporation Media API
  slug: apa-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-media-api-openapi.yml
- filename: apa-o-embed-api-openapi.yml
  format: yaml
  label: APA Corporation o Embed API
  slug: apa-o-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/openapi/apa-o-embed-api-openapi.yml
consequence_counts: {}
description: 'Recommended x-agentic-access contract for the APA Corporation REST surface. The classification is uniform and that is the finding: all 28 operations on the public contract are safe HTTP GETs, none requires a credential, none changes state, and none has a consequence to escalate. An agent can call this entire surface unattended. The one caveat worth carrying into an agent policy is freshness, not risk: the share-price quote is edge-cached for 600 seconds, so an agent must not present it as a real-time price.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apa Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'APA Corporation exposes 28 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: APA Corporation
provider_slug: apa
slug: apa-agentic-access
source_filename: apa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: generated\nsource: classification of every operation in openapi/*.yml, verified anonymously live on 2026-09-14\nprovider: APA Corporation\nproviderId: apa\ndescription: 'Recommended x-agentic-access contract for the APA Corporation REST surface. The classification is uniform and that is the finding: all 28 operations on the public contract are safe HTTP GETs, none requires a credential, none changes state, and none has a consequence to escalate. An agent can call this entire surface unattended. The one caveat worth carrying into an agent policy is freshness, not risk: the share-price quote is edge-cached for 600 seconds, so an agent must not present it as a real-time price.'\nsummary:\n  operations: 28\n  write_operations: 0\n  credentialed_operations: 0\n  escalation_required: 0\n  default_action_class: read\n  default_consequence: none\npolicy:\n  unattended_calls: allowed\n  human_in_the_loop: not required\n  rate_discipline: No published\
  \ limit and no runtime signal (see rate-limits/apa-rate-limits.yml). An agent should honour the 600s Cache-Control rather than poll, cap per_page at the published 100, and read X-WP-TotalPages before paging.\n  data_handling: Everything returned is already public on apacorp.com. The Authors API returns named individuals — five public author records — so an agent should treat those as published bylines, not as contact data, and should not enrich or cross-reference them.\noperations:\n- operationId: listAuthors\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-authors-api-openapi.yml\n  path: /wp/v2/users\n- operationId: getAuthor\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-authors-api-openapi.yml\n  path: /wp/v2/users/{id}\n- operationId: listContentTypes\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required:\
  \ false\n  escalation: none\n  spec: openapi/apa-discovery-api-openapi.yml\n  path: /wp/v2/types\n- operationId: listTaxonomies\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-discovery-api-openapi.yml\n  path: /wp/v2/taxonomies\n- operationId: listPostStatuses\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-discovery-api-openapi.yml\n  path: /wp/v2/statuses\n- operationId: getContentType\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-discovery-api-openapi.yml\n  path: /wp/v2/types/{type}\n- operationId: getTaxonomy\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-discovery-api-openapi.yml\n  path: /wp/v2/taxonomies/{taxonomy}\n- operationId: getPostStatus\n  action_class: read\n\
  \  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-discovery-api-openapi.yml\n  path: /wp/v2/statuses/{status}\n- operationId: listFeedItems\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-feed-items-api-openapi.yml\n  path: /wp/v2/wprss_feed_item\n- operationId: getFeedItem\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-feed-items-api-openapi.yml\n  path: /wp/v2/wprss_feed_item/{id}\n- operationId: listLeadership\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-leadership-api-openapi.yml\n  path: /wp/v2/leaderships\n- operationId: getLeadershipProfile\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-leadership-api-openapi.yml\n\
  \  path: /wp/v2/leaderships/{id}\n- operationId: listMediaHubVideos\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-media-hub-api-openapi.yml\n  path: /wp/v2/presto-videos\n- operationId: getMediaHubVideo\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-media-hub-api-openapi.yml\n  path: /wp/v2/presto-videos/{id}\n- operationId: listMediaAttachments\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-media-hub-api-openapi.yml\n  path: /wp/v2/media\n- operationId: getMediaAttachment\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-media-hub-api-openapi.yml\n  path: /wp/v2/media/{id}\n- operationId: listNewsroomPosts\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required:\
  \ false\n  escalation: none\n  spec: openapi/apa-newsroom-api-openapi.yml\n  path: /wp/v2/posts\n- operationId: getNewsroomPost\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-newsroom-api-openapi.yml\n  path: /wp/v2/posts/{id}\n- operationId: getOembedPayload\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-oembed-api-openapi.yml\n  path: /oembed/1.0/embed\n- operationId: listPages\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-pages-api-openapi.yml\n  path: /wp/v2/pages\n- operationId: getPage\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-pages-api-openapi.yml\n  path: /wp/v2/pages/{id}\n- operationId: searchContent\n  action_class: read\n  consequence: none\n  reversible: na\n\
  \  auth_required: false\n  escalation: none\n  spec: openapi/apa-search-api-openapi.yml\n  path: /wp/v2/search\n- operationId: listCategories\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-taxonomy-api-openapi.yml\n  path: /wp/v2/categories\n- operationId: getCategory\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-taxonomy-api-openapi.yml\n  path: /wp/v2/categories/{id}\n- operationId: listTags\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-taxonomy-api-openapi.yml\n  path: /wp/v2/tags\n- operationId: getTag\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-taxonomy-api-openapi.yml\n  path: /wp/v2/tags/{id}\n- operationId: getApaShareQuote\n  action_class: read\n  consequence: none\n\
  \  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-ticker-api-openapi.yml\n  path: /apa-ticker/v1/quote\n- operationId: getTickerNamespaceIndex\n  action_class: read\n  consequence: none\n  reversible: na\n  auth_required: false\n  escalation: none\n  spec: openapi/apa-ticker-api-openapi.yml\n  path: /apa-ticker/v1\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/agentic-access/apa-agentic-access.yml
summary_line: 28 operations
tags:
- Oil and Gas
- Energy
- Exploration
- Production
- WordPress
- REST
- Content
- Newsroom
- Investor Relations
- Energy Production
---
