---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: denbury-resources-pages-api-openapi.yml
  format: yaml
  label: Denbury Resources Pages API
  slug: denbury-resources-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-pages-api-openapi.yml
- filename: denbury-resources-media-api-openapi.yml
  format: yaml
  label: Denbury Resources Media API
  slug: denbury-resources-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-media-api-openapi.yml
- filename: denbury-resources-search-api-openapi.yml
  format: yaml
  label: Denbury Resources Search API
  slug: denbury-resources-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-search-api-openapi.yml
- filename: denbury-resources-discovery-api-openapi.yml
  format: yaml
  label: Denbury Resources Discovery API
  slug: denbury-resources-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-discovery-api-openapi.yml
- filename: denbury-resources-oembed-api-openapi.yml
  format: yaml
  label: Denbury Resources oEmbed API
  slug: denbury-resources-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/openapi/denbury-resources-oembed-api-openapi.yml
consequence_counts: {}
description: 'Recommended x-agentic-access classification for every operation Denbury Inc.''s public surface exposes. This is an API Evangelist RECOMMENDATION, not a Denbury publication — Denbury declares no agent policy of any kind. The classification is unusually simple here because the surface is uniformly read-only: twelve GET operations, no credentials, no side effects, nothing to escalate.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: derived
name: Denbury Resources Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Denbury Resources exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Denbury Resources
provider_slug: denbury-resources
slug: denbury-resources-agentic-access
source_filename: denbury-resources-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/ + conventions/denbury-resources-conventions.yml + live probes (2026-09-06)\ndescription: >-\n  Recommended x-agentic-access classification for every operation Denbury Inc.'s public surface\n  exposes. This is an API Evangelist RECOMMENDATION, not a Denbury publication — Denbury declares no\n  agent policy of any kind. The classification is unusually simple here because the surface is\n  uniformly read-only: twelve GET operations, no credentials, no side effects, nothing to escalate.\npolicy_published_by_provider: false\nprovider_agent_policy_evidence:\n- url: https://www.denbury.com/robots.txt\n  status: 200\n  detail: 'Two rules only — Disallow: /wp-admin/ and Disallow: /wp-login.php. No AI/agent directives.'\n- url: https://www.denbury.com/llms.txt\n  status: 301\n  detail: No llms.txt is served.\n- url: https://www.denbury.com/.well-known/ai-plugin.json\n  status: 403\n  detail: The whole /.well-known/ namespace\
  \ is refused at the origin.\ndefaults:\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-applicable\n  human_in_the_loop: false\n  rationale: >-\n    Every documented operation is a GET against published corporate website content. There is no\n    state to mutate, no money to move, no personal data returned (the users route is 403 and the\n    author edge is unresolvable), and no credential to scope.\noperations:\n- operationId: listPages\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-applicable\n- operationId: getPage\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-applicable\n- operationId: listMedia\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-applicable\n- operationId: getMediaItem\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation:\
  \ not-applicable\n  note: >-\n    source_url points at files up to several megabytes (the largest observed was a 6.7 MB PDF).\n    Bandwidth, not risk, is the constraint an agent should plan around.\n- operationId: search\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-applicable\n- operationId: listTypes\n  action_class: read\n  consequence: none\n  scope: metadata\n  token: none\n  escalation: not-applicable\n- operationId: getType\n  action_class: read\n  consequence: none\n  scope: metadata\n  token: none\n  escalation: not-applicable\n- operationId: listTaxonomies\n  action_class: read\n  consequence: none\n  scope: metadata\n  token: none\n  escalation: not-applicable\n- operationId: getTaxonomy\n  action_class: read\n  consequence: none\n  scope: metadata\n  token: none\n  escalation: not-applicable\n- operationId: listCategories\n  action_class: read\n  consequence: none\n  scope: metadata\n  token: none\n  escalation: not-applicable\n\
  - operationId: getCategory\n  action_class: read\n  consequence: none\n  scope: metadata\n  token: none\n  escalation: not-applicable\n- operationId: getOembed\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-applicable\nguidance_for_agents:\n- >-\n  No rate-limit signal is emitted. Absence of a limit header is not a licence — this is a legacy\n  corporate site inside an acquirer's estate. Keep concurrency at 1-2 and pause between pages.\n- >-\n  Honour robots.txt: do not touch /wp-admin/ or /wp-login.php. Nothing under those paths appears in\n  openapi/.\n- >-\n  Do not attempt the write methods. They exist on the same routes but require WordPress\n  application-password credentials that Denbury issues only to its own site administrators;\n  attempting them is a credential-guessing attempt, not an API call.\n- >-\n  Date-stamp everything retrieved. Denbury was acquired by ExxonMobil in November 2023 and\n  deregistered its securities\
  \ on 2023-11-22; this content is historical corporate material.\ncounts:\n  operations: 12\n  read: 12\n  write: 0\n  requiring_escalation: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/denbury-resources/refs/heads/main/agentic-access/denbury-resources-agentic-access.yml
summary_line: 12 operations
tags:
- Acquired
- Carbon Capture
- CO2 EOR
- Energy
- Enhanced Oil Recovery
- ExxonMobil
- Oil and Gas
- Fortune 1000
- Content
- Carbon Sequestration
---
