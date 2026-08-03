---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: probed
name: Bespoke Post Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 0
overview: 'Bespoke Post exposes 0 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bespoke Post
provider_slug: bespoke-post
slug: bespoke-post-agentic-access
source_filename: bespoke-post-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://www.bespokepost.com/robots.txt\n\n# WHAT THIS IS\n# Bespoke Post publishes no OpenAPI and no `x-agentic-access` contract. It does,\n# however, publish a machine-readable, AI-agent-specific access policy in its\n# robots.txt: eight named AI crawlers/agents are granted explicit `Allow:` access\n# to eight named /api/ paths, while the wildcard `User-agent: *` group is\n# `Disallow: /api/`. That is an affirmative, provider-authored statement about\n# which agents may call which API surfaces — captured here verbatim.\n#\n# SCOPE + LIMITS (read before using)\n#   - This is a PATH-level allowlist, not an operation-level execution contract.\n#     No action-class, consequence, token-TTL, or escalation semantics are\n#     published; the fields below are recorded, not inferred.\n#   - robots.txt is advisory. It is not enforcement, and it grants no credential.\n#   - The endpoints themselves sit behind a Cloudflare bot challenge\
  \ (HTTP 403 to\n#     a non-verified client), so their response contracts were NOT observed.\n#     Their existence is asserted by the provider, not confirmed by us.\n\nposture:\n  published_contract: false          # no x-agentic-access / no OpenAPI\n  agent_policy_published: true       # robots.txt agent directives\n  policy_format: robots.txt\n  granularity: path\n  enforcement: advisory\n  default_for_unnamed_agents: disallow   # `User-agent: *` -> Disallow: /api/\n\nsummary:\n  agents_named: 8\n  api_paths_allowed: 8\n  paths_disallowed_to_others: 9\n  authentication_documented: false\n  operation_level_semantics: false\n\n# Verbatim from the two Allow: groups in robots.txt.\nallowed_agents:\n  - agent: Googlebot\n    class: search\n  - agent: Googlebot-Image\n    class: search\n  - agent: Bingbot\n    class: search\n  - agent: GPTBot\n    class: ai-training\n    vendor: OpenAI\n  - agent: ChatGPT-User\n    class: ai-user-agent\n    vendor: OpenAI\n  - agent: OAI-Searchbot\n    class:\
  \ ai-search\n    vendor: OpenAI\n  - agent: ClaudeBot\n    class: ai-training\n    vendor: Anthropic\n  - agent: anthropic-ai\n    class: ai-user-agent\n    vendor: Anthropic\n  - agent: PerplexityBot\n    class: ai-search\n    vendor: Perplexity\n  - agent: meta-externalagent\n    class: ai-training\n    vendor: Meta\n  - agent: cohere-ai\n    class: ai-training\n    vendor: Cohere\n\n# The API surface the provider itself names. Read-only by nature of robots.txt\n# (which governs retrieval, i.e. GET); no write path is allowed to any agent.\nallowed_paths:\n  - path: /api/collections/\n    action_class: connected\n    consequence: read\n    note: product collections\n  - path: /api/products/\n    action_class: connected\n    consequence: read\n    note: product catalog\n  - path: /api/current_user?\n    action_class: connected\n    consequence: read\n    note: session/account read; requires an authenticated session\n  - path: /api/current_user/carts\n    action_class: connected\n    consequence:\
  \ read\n    note: cart read for the current session\n  - path: /api/current_user/box_assignments\n    action_class: connected\n    consequence: read\n    note: monthly box assignment for the current member\n  - path: /api/current_user/for_you_assignments\n    action_class: connected\n    consequence: read\n    note: personalized recommendation assignments\n  - path: /api/user_segments/\n    action_class: connected\n    consequence: read\n    note: audience/segment metadata\n  - path: /api/questions/\n    action_class: connected\n    consequence: read\n    note: onboarding quiz questions\n\n# Explicitly withheld from every unnamed agent.\ndisallowed_paths_wildcard:\n  - /a/\n  - /api/\n  - /cart/\n  - /d/\n  - /land/\n  - /products/search\n  - /press\n  - /account/\n  - /order_returns_searches/\n\nrelated_signals:\n  - kind: dns-txt\n    value: anthropic-domain-verification-bjwvph=17U94yLRvciNQNgGAhHsaTvDv\n    domain: bespokepost.com\n    note: >-\n      Anthropic domain-verification TXT\
  \ record present on the apex domain,\n      consistent with the operator having claimed the domain with Anthropic.\n      Recorded as an observation only; it confers no API surface.\n\ngaps:\n  - No OpenAPI, AsyncAPI, or GraphQL schema published for the /api/ surface.\n  - No developer portal, authentication documentation, or rate-limit policy.\n  - No MCP server and no A2A agent card on any probed host.\n  - Endpoints are bot-challenged, so no agent can actually exercise the allowlist\n    without being an IP-verified crawler.\n\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://www.bespokepost.com/robots.txt\n  http_status: 200\n  content_type: text/plain; charset=utf-8\n  file: bespoke-post-robots.txt\n  endpoint_probes:\n    - {url: 'https://www.bespokepost.com/api/collections/', http_status: 403, note: Cloudflare bot challenge}\n    - {url: 'https://www.bespokepost.com/api/products/', http_status: 403, note: Cloudflare bot challenge}\n    - {url: 'https://www.bespokepost.com/api/current_user',\
  \ http_status: 403, note: Cloudflare bot challenge}\n    - {url: 'https://www.bespokepost.com/api/user_segments/', http_status: 403, note: Cloudflare bot challenge}\n    - {url: 'https://www.bespokepost.com/api/questions/', http_status: 403, note: Cloudflare bot challenge}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bespoke-post/refs/heads/main/agentic-access/bespoke-post-agentic-access.yml
summary_line: 0 operations
tags:
- Company
- E-Commerce
- Retail
- Subscription
- Direct to Consumer
- Consumer Goods
- Apparel
- Men's Lifestyle
---
