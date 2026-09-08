---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: addis-energy-posts-api-openapi.yml
  format: yaml
  label: Addis Energy Posts API
  slug: addis-energy-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-posts-api-openapi.yml
- filename: addis-energy-pages-api-openapi.yml
  format: yaml
  label: Addis Energy Pages API
  slug: addis-energy-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-pages-api-openapi.yml
- filename: addis-energy-media-api-openapi.yml
  format: yaml
  label: Addis Energy Media API
  slug: addis-energy-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-media-api-openapi.yml
- filename: addis-energy-taxonomy-api-openapi.yml
  format: yaml
  label: Addis Energy Taxonomy API
  slug: addis-energy-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-taxonomy-api-openapi.yml
- filename: addis-energy-users-api-openapi.yml
  format: yaml
  label: Addis Energy Users API
  slug: addis-energy-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-users-api-openapi.yml
- filename: addis-energy-search-api-openapi.yml
  format: yaml
  label: Addis Energy Search API
  slug: addis-energy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-search-api-openapi.yml
- filename: addis-energy-discovery-api-openapi.yml
  format: yaml
  label: Addis Energy Discovery API
  slug: addis-energy-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-discovery-api-openapi.yml
- filename: addis-energy-oembed-api-openapi.yml
  format: yaml
  label: Addis Energy oEmbed API
  slug: addis-energy-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-oembed-api-openapi.yml
consequence_counts: {}
description: 'RECOMMENDED x-agentic-access contracts for the public Addis Energy surface. This is an API Evangelist recommendation authored on the provider''s behalf, NOT a declaration Addis Energy has made — the company publishes no agent policy of any kind. The classification is simple because the surface is: every anonymously reachable operation is a safe, reversible, unauthenticated read.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Addis Energy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Addis Energy exposes 21 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Addis Energy
provider_slug: addis-energy
slug: addis-energy-agentic-access
source_filename: addis-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: generated\nsource: classification of every operation in openapi/ against the live surface probed 2026-09-07\ndescription: >-\n  RECOMMENDED x-agentic-access contracts for the public Addis Energy surface. This is an API\n  Evangelist recommendation authored on the provider's behalf, NOT a declaration Addis Energy has\n  made — the company publishes no agent policy of any kind. The classification is simple because\n  the surface is: every anonymously reachable operation is a safe, reversible, unauthenticated\n  read.\nprovider_declared: false\ndefault_policy:\n  action_class: read\n  consequence: none\n  reversible: true\n  token: none\n  escalation: none\n  human_in_the_loop: false\n  rationale: >-\n    The entire public surface is GET over published marketing content. No operation creates,\n    charges, sends, deletes or discloses anything non-public, so no operation warrants a\n    confirmation step.\noperations:\n- operationId: listPosts\n\
  \  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: none\n- operationId: getPost\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: none\n- operationId: listPages\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: none\n- operationId: getPage\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: none\n- operationId: listMedia\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: none\n- operationId: getMediaItem\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: none\n- operationId: listCategories\n  action_class: read\n  consequence: none\n  scope: public-taxonomy\n  token: none\n  escalation: none\n- operationId: getCategory\n  action_class: read\n  consequence: none\n  scope: public-taxonomy\n  token: none\n  escalation:\
  \ none\n- operationId: listTags\n  action_class: read\n  consequence: none\n  scope: public-taxonomy\n  token: none\n  escalation: none\n- operationId: getTag\n  action_class: read\n  consequence: none\n  scope: public-taxonomy\n  token: none\n  escalation: none\n- operationId: listUsers\n  action_class: read\n  consequence: none\n  scope: public-authors\n  token: none\n  escalation: none\n  note: >-\n    Returns display name, slug, author-archive URL and avatar URL for people who have published on\n    the site. No email address or role is exposed in the anonymous `view` context. Treat the\n    returned names as personal data and handle accordingly even though the API discloses them\n    freely.\n- operationId: getUser\n  action_class: read\n  consequence: none\n  scope: public-authors\n  token: none\n  escalation: none\n- operationId: search\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: none\n- operationId: getRouteIndex\n  action_class:\
  \ read\n  consequence: none\n  scope: discovery\n  token: none\n  escalation: none\n- operationId: getWpV2Namespace\n  action_class: read\n  consequence: none\n  scope: discovery\n  token: none\n  escalation: none\n- operationId: listTypes\n  action_class: read\n  consequence: none\n  scope: discovery\n  token: none\n  escalation: none\n- operationId: getType\n  action_class: read\n  consequence: none\n  scope: discovery\n  token: none\n  escalation: none\n- operationId: listTaxonomies\n  action_class: read\n  consequence: none\n  scope: discovery\n  token: none\n  escalation: none\n- operationId: getTaxonomy\n  action_class: read\n  consequence: none\n  scope: discovery\n  token: none\n  escalation: none\n- operationId: listStatuses\n  action_class: read\n  consequence: none\n  scope: discovery\n  token: none\n  escalation: none\n- operationId: getOEmbed\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: none\nout_of_scope:\n  detail: >-\n\
  \    The write half of the wp/v2 routes, the contact-form-7 feedback endpoint, the\n    siteground-optimizer, code-snippets, duplicator and wp-abilities namespaces, and\n    /wp/v2/settings are all administrator-only site-operations surfaces. They are deliberately\n    excluded from openapi/ and no agent contract is recommended for them: they are not a public\n    API and an agent should never attempt them.\nagent_guidance:\n  robots: >-\n    Responses carry X-Robots-Tag: noindex. Read, but do not republish this content into a search\n    index.\n  rate: >-\n    No rate-limit signal is returned. Budget yourself: the entire corpus is four requests at\n    per_page=100, and https://addisenergy.com/feed/ is the cheaper change signal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/agentic-access/addis-energy-agentic-access.yml
summary_line: 21 operations
tags:
- Company
- Energy
- Clean Energy
- Ammonia
- Climate Tech
- Deep Tech
- Geoscience
- Subsurface
- Materials Science
- Hydrogen
- Fertilizer
- Content
---
