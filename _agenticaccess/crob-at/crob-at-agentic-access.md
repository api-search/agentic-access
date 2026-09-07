---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: crob-at-openapi.json
  format: json
  label: crob.at REST API
  slug: crobat-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crob-at/refs/heads/main/openapi/crob-at-openapi.json
consequence_counts:
  read: 6
  write: 4
description: 'Recommended x-agentic-access execution contracts, classified from the OpenAPI. crob.at is unusually agent-friendly for its size: anonymous keyless API, an llms.txt that explicitly addresses agents, markdown twins of every team page (append .md or send Accept: text/markdown — verified live), robots.txt Content-Signal (search=yes, ai-train=no, ai-input=yes) with named AI crawlers allowed, and a stated agentPolicy of "allowed" in its APIs Onboarding document. Review and bind audience per deployment.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crob At Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'crob.at exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: crob.at
provider_slug: crob-at
slug: crob-at-agentic-access
source_filename: crob-at-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: generated\nsource: openapi/crob-at-openapi.json + https://crob.at/robots.txt + https://crob.at/llms.txt\ndescription: >-\n  Recommended x-agentic-access execution contracts, classified from the OpenAPI.\n  crob.at is unusually agent-friendly for its size: anonymous keyless API, an\n  llms.txt that explicitly addresses agents, markdown twins of every team page\n  (append .md or send Accept: text/markdown — verified live), robots.txt\n  Content-Signal (search=yes, ai-train=no, ai-input=yes) with named AI crawlers\n  allowed, and a stated agentPolicy of \"allowed\" in its APIs Onboarding\n  document. Review and bind audience per deployment.\nprovider_signals:\n  agent_policy: allowed (declared in /.well-known/api-onboarding account.agentPolicy)\n  content_signal: 'search=yes, ai-train=no, ai-input=yes'\n  markdown_twins: append .md to any team URL or send Accept text/markdown (probed 200 text/markdown)\n  llms_txt: https://crob.at/llms.txt\nsummary:\n\
  \  operations: 10\n  by_action_class:\n    connected: 8\n    acting: 2\n  by_consequence:\n    read: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n  - path: /api/team/{slug}\n    method: get\n    operationId: getTeamBySlug\n    x-agentic-access: {action-class: connected, consequence: read, subject: none}\n  - path: /api/team/{slug}/{teamSlug}\n    method: get\n    operationId: getTeamInPasteBySlug\n    x-agentic-access: {action-class: connected, consequence: read, subject: none}\n  - path: /api/team\n    method: post\n    operationId: createTeam\n    x-agentic-access:\n      action-class: connected\n      consequence: write\n      subject: none\n      note: Creates a permanent public/unlisted page with no API reversal path; rate-limited 500/hour.\n  - path: /api/random-team/{format}\n    method: get\n    operationId: generateRandomTeam\n    x-agentic-access: {action-class: connected, consequence: read, subject: none}\n  - path: /api/random-team/{format}/save\n    method:\
  \ post\n    operationId: saveRandomTeam\n    x-agentic-access:\n      action-class: connected\n      consequence: write\n      subject: none\n      note: Idempotent via idempotencyKey; creates a permanent unlisted URL; rate-limited 30/hour.\n  - path: /api/samples/{tier}\n    method: get\n    operationId: listSampleTeams\n    x-agentic-access: {action-class: connected, consequence: read, subject: none}\n  - path: /api/type-chart-data\n    method: get\n    operationId: getTypeChartData\n    x-agentic-access: {action-class: connected, consequence: read, subject: none}\n  - path: /api/me\n    method: get\n    operationId: getCurrentUser\n    x-agentic-access: {action-class: acting, consequence: read, subject: session-user}\n  - path: /api/feedback\n    method: post\n    operationId: sendFeedback\n    x-agentic-access:\n      action-class: connected\n      consequence: write\n      subject: none\n      note: Cannot be recalled; rate-limited 5/hour — agents should not use it for automated traffic.\n\
  \  - path: /api/showdown/assertion\n    method: post\n    operationId: createShowdownAssertion\n    x-agentic-access:\n      action-class: acting\n      consequence: write\n      subject: session-user\n      note: Auth broker for Pokemon Showdown login; same-origin session only — not an agent surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crob-at/refs/heads/main/agentic-access/crob-at-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- Gaming
- Esports
- Pokemon
- Pokemon Showdown
- Team Building
- Content Rendering
- Developer Tools
- REST API
---
