---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: xgs-energy-posts-api-openapi.yml
  format: yaml
  label: XGS Energy Posts API
  slug: xgs-energy-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-posts-api-openapi.yml
- filename: xgs-energy-pages-api-openapi.yml
  format: yaml
  label: XGS Energy Pages API
  slug: xgs-energy-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-pages-api-openapi.yml
- filename: xgs-energy-media-api-openapi.yml
  format: yaml
  label: XGS Energy Media API
  slug: xgs-energy-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-media-api-openapi.yml
- filename: xgs-energy-search-api-openapi.yml
  format: yaml
  label: XGS Energy Search API
  slug: xgs-energy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-search-api-openapi.yml
- filename: xgs-energy-categories-api-openapi.yml
  format: yaml
  label: XGS Energy Categories API
  slug: xgs-energy-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-categories-api-openapi.yml
- filename: xgs-energy-tags-api-openapi.yml
  format: yaml
  label: XGS Energy Tags API
  slug: xgs-energy-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-tags-api-openapi.yml
- filename: xgs-energy-discovery-api-openapi.yml
  format: yaml
  label: XGS Energy Discovery API
  slug: xgs-energy-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-discovery-api-openapi.yml
- filename: xgs-energy-oembed-api-openapi.yml
  format: yaml
  label: XGS Energy oEmbed API
  slug: xgs-energy-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-oembed-api-openapi.yml
consequence_counts: {}
description: 'Recommended x-agentic-access contract for the XGS Energy public surface. Every documented operation is an anonymous read of public website content: no writes, no cost, no consent boundary, no reversibility question. This is a recommendation by API Evangelist, not a contract XGS Energy publishes.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Xgs Energy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'XGS Energy exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: XGS Energy
provider_slug: xgs-energy
slug: xgs-energy-agentic-access
source_filename: xgs-energy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: generated\nsource: openapi/ — classification of every documented operation\ndescription: 'Recommended x-agentic-access contract for the XGS Energy public surface. Every documented operation\n  is an anonymous read of public website content: no writes, no cost, no consent boundary, no reversibility\n  question. This is a recommendation by API Evangelist, not a contract XGS Energy publishes.'\nposture:\n  overall: safe-read-only\n  writes: 0\n  reads: 17\n  human_in_the_loop_required: false\n  spend_risk: none\n  data_sensitivity: public\n  caveat: One route on the host, /wp-json/wp/v2/users, returns personal data and is deliberately outside this\n    contract and outside every tool and skill in this repository.\noperations:\n- operation: listPosts\n  path: /wp/v2/posts\n  spec: openapi/xgs-energy-posts-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note:\
  \ Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: getPost\n  path: /wp/v2/posts/{id}\n  spec: openapi/xgs-energy-posts-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: listPages\n  path: /wp/v2/pages\n  spec: openapi/xgs-energy-pages-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: getPage\n  path: /wp/v2/pages/{id}\n  spec: openapi/xgs-energy-pages-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change,\
  \ no cost, no personal data.\n- operation: listMedia\n  path: /wp/v2/media\n  spec: openapi/xgs-energy-media-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: getMediaItem\n  path: /wp/v2/media/{id}\n  spec: openapi/xgs-energy-media-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: search\n  path: /wp/v2/search\n  spec: openapi/xgs-energy-search-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: listCategories\n\
  \  path: /wp/v2/categories\n  spec: openapi/xgs-energy-categories-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: getCategory\n  path: /wp/v2/categories/{id}\n  spec: openapi/xgs-energy-categories-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: listTags\n  path: /wp/v2/tags\n  spec: openapi/xgs-energy-tags-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: getTag\n  path: /wp/v2/tags/{id}\n  spec: openapi/xgs-energy-tags-api-openapi.yml\n\
  \  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: getRouteIndex\n  path: /\n  spec: openapi/xgs-energy-discovery-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: getCoreNamespaceIndex\n  path: /wp/v2\n  spec: openapi/xgs-energy-discovery-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: listContentTypes\n  path: /wp/v2/types\n  spec: openapi/xgs-energy-discovery-api-openapi.yml\n  action_class: read\n  consequence: none\n\
  \  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: listTaxonomies\n  path: /wp/v2/taxonomies\n  spec: openapi/xgs-energy-discovery-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: listStatuses\n  path: /wp/v2/statuses\n  spec: openapi/xgs-energy-discovery-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n- operation: getOEmbed\n  path: /oembed/1.0/embed\n  spec: openapi/xgs-energy-oembed-api-openapi.yml\n  action_class: read\n  consequence: none\n  reversible: na\n  scope: public-content\n\
  \  token: none\n  escalation: none\n  note: Anonymous GET over public website content. No state change, no cost, no personal data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/agentic-access/xgs-energy-agentic-access.yml
summary_line: 17 operations
tags:
- Company
- Energy
- Geothermal
- Renewable Energy
- Clean Energy
- Power Generation
- Energy Infrastructure
- Data Center Power
- Climate Tech
- Content
---
