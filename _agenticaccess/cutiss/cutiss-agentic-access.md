---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: cutiss-newsroom-api-openapi.yml
  format: yaml
  label: CUTISS Newsroom API
  slug: cutiss-newsroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-newsroom-api-openapi.yml
- filename: cutiss-posts-api-openapi.yml
  format: yaml
  label: CUTISS Posts API
  slug: cutiss-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-posts-api-openapi.yml
- filename: cutiss-pages-api-openapi.yml
  format: yaml
  label: CUTISS Pages API
  slug: cutiss-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-pages-api-openapi.yml
- filename: cutiss-team-api-openapi.yml
  format: yaml
  label: CUTISS Team API
  slug: cutiss-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-team-api-openapi.yml
- filename: cutiss-teams-api-openapi.yml
  format: yaml
  label: CUTISS Teams Taxonomy API
  slug: cutiss-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-teams-api-openapi.yml
- filename: cutiss-media-api-openapi.yml
  format: yaml
  label: CUTISS Media API
  slug: cutiss-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-media-api-openapi.yml
- filename: cutiss-categories-api-openapi.yml
  format: yaml
  label: CUTISS Categories API
  slug: cutiss-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-categories-api-openapi.yml
- filename: cutiss-search-api-openapi.yml
  format: yaml
  label: CUTISS Search API
  slug: cutiss-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-search-api-openapi.yml
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: derived
name: Cutiss Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'CUTISS exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CUTISS
provider_slug: cutiss
slug: cutiss-agentic-access
source_filename: cutiss-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: derived\nsource: openapi/ + conventions/cutiss-conventions.yml\nsummary: Recommended x-agentic-access posture for the CUTISS content API. Every publicly reachable operation\n  is a safe, read-only retrieval of already-public corporate content, so the whole surface classifies\n  as low-consequence.\ndefaults:\n  action_class: read\n  consequence: none\n  token: none\n  escalation: not-required\n  reversible: true\noperations:\n- operationId: listNewsroom\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: getNewsroomItem\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n   \
  \ listed staff profiles.\n- operationId: listPosts\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: getPostsItem\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: listPages\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: getPagesItem\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET\
  \ of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: listTeam\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: getTeamItem\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: listTeams\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: getTeamsItem\n  action_class: read\n  consequence: none\n  scope:\
  \ public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: listMedia\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: getMediaItem\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: listCategories\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff\
  \ profiles.\n- operationId: getCategoriesItem\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\n- operationId: listSearch\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-required\n  note: Anonymous GET of published corporate content. No state change, no personal data beyond publicly\n    listed staff profiles.\ndenied:\n- surface: all write methods (POST/PUT/PATCH/DELETE)\n  reason: 401 rest_forbidden for anonymous callers — an agent cannot and must not attempt them.\n- surface: /wp/v2/users, /wp/v2/settings, /wp/v2/plugins, /wp/v2/menus\n  reason: Administrative, 401-gated.\n- surface: /wp-abilities/v1/*\n  reason: Agent ability registry, 401-gated.\nagent_guidance:\n- Treat this as a corporate content source, not a product API — there is no\
  \ transactional capability here.\n- Cap per_page at 100 and page with X-WP-TotalPages; self-throttle, since no rate limit is published.\n- 'Filter by language: parallel English and German records exist with distinct ids and will otherwise\n  duplicate.'\n- Branch on the error `code` field — messages are returned in German regardless of request locale.\n- The team directory contains named individuals; treat it as personal data even though it is publicly\n  published.\n- This API carries no CUTISS stability commitment; re-validate the shape rather than caching assumptions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/agentic-access/cutiss-agentic-access.yml
summary_line: 15 operations
tags:
- Company
- Biotechnology
- Regenerative Medicine
- Tissue Engineering
- Life Sciences
- Medical Devices
- Clinical Trials
- Dermatology
- Healthcare
- Switzerland
- Research
- Content
---
