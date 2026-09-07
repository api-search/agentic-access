---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: keio-koara-oai-pmh-openapi.yml
  format: yaml
  label: KOARA OAI-PMH Metadata API
  slug: koara-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keio/refs/heads/main/openapi/keio-koara-oai-pmh-openapi.yml
- filename: keio-iiif-openapi.yml
  format: yaml
  label: Keio Media Center Digital Collections IIIF API
  slug: iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keio/refs/heads/main/openapi/keio-iiif-openapi.yml
consequence_counts: {}
description: 'What an AI agent arriving at Keio University can actually do. The finding is mixed in an interesting way: the institution publishes none of the modern agent-facing conventions and, on its main web estate, not even the old ones — but the two surfaces it does operate are among the friendliest an agent could ask for, because they are anonymous, standards-described and self-describing. An agent that knows OAI-PMH or IIIF can consume Keio''s scholarly and digitised holdings today with no key, no negotiation and no account.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: derived
name: Keio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 0
overview: 'Keio University exposes 0 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Keio University
provider_slug: keio
slug: keio-agentic-access
source_filename: keio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nauthorship: API Evangelist\nprobe_basis: live probe sweep of Keio University surfaces, 2026-09-01\nsource: >-\n  Direct probes on 2026-09-01 of the agent-facing conventions on Keio's main and service hosts.\n  Every status code below is from a real fetch with a browser User-Agent.\nprovider: Keio University\nproviderId: keio\ndescription: >-\n  What an AI agent arriving at Keio University can actually do. The finding is mixed in an\n  interesting way: the institution publishes none of the modern agent-facing conventions and, on\n  its main web estate, not even the old ones — but the two surfaces it does operate are among the\n  friendliest an agent could ask for, because they are anonymous, standards-described and\n  self-describing. An agent that knows OAI-PMH or IIIF can consume Keio's scholarly and digitised\n  holdings today with no key, no negotiation and no account.\n\nconventions:\n  - name: llms.txt\n    url: https://www.keio.ac.jp/llms.txt\n\
  \    status: 404\n    present: false\n    note: A real HTTP 404 returning the site's Japanese not-found page, not a soft-404.\n  - name: robots.txt (main site)\n    url: https://www.keio.ac.jp/robots.txt\n    status: 404\n    present: false\n    note: >-\n      The primary institutional web estate publishes no robots.txt at all. Recorded as observed;\n      the absence means there is no crawl directive of any kind for the main site.\n  - name: robots.txt (KOARA repository)\n    url: https://koara.lib.keio.ac.jp/robots.txt\n    status: 200\n    present: true\n    content: 'User-agent: * / Allow: /'\n    note: Maximally permissive — the repository invites harvesting.\n  - name: robots.txt (Digital Collections)\n    url: https://dcollections.lib.keio.ac.jp/robots.txt\n    status: 200\n    present: true\n    note: Drupal's stock robots.txt, unmodified.\n  - name: security.txt\n    url: https://www.keio.ac.jp/.well-known/security.txt\n    status: 404\n    present: false\n  - name: MCP server\n\
  \    present: false\n    note: No Model Context Protocol server, manifest or endpoint found on any Keio host.\n  - name: Agent card (/.well-known/agent.json)\n    present: false\n    note: >-\n      Not found, and deliberately not derived. Agent cards are search-only in this pipeline; one is\n      never written on a provider's behalf.\n  - name: OpenAPI published by Keio\n    present: false\n    note: >-\n      Keio publishes no OpenAPI, no AsyncAPI, no apis.json and no WADL. The two contracts in this\n      repository were written by API Evangelist from probes and are marked as such in their\n      x-provenance blocks.\n\nagent_consumable_today:\n  - surface: KOARA OAI-PMH\n    baseURL: https://koara.lib.keio.ac.jp/xoonips/modules/xoonips/oai.php\n    x-operator: institution\n    why: >-\n      Anonymous, no key, no rate limit encountered, responses self-describe against a published\n      schema, and the full set hierarchy is enumerable in one call. An agent can harvest the entire\n\
  \      scholarly record of the university without asking anyone.\n    caveat: >-\n      Protocol errors arrive with HTTP 200 and the failure inside the XML body. An agent branching\n      on status code alone will silently mistake failures for successes.\n  - surface: IIIF Presentation and Image APIs\n    baseURL: https://dcollections.lib.keio.ac.jp/sites/default/files/iiif/\n    x-operator: institution\n    why: >-\n      Anonymous JSON-LD, IIIF-conformant, with an image service that answers arbitrary region, size\n      and rotation requests. An agent can retrieve and reason over 656 folios of the Gutenberg\n      42-line Bible without an account.\n    caveat: >-\n      Archive codes are undocumented. Manifest URLs must be resolved from the site's HTML, which is\n      the one real barrier to autonomous discovery on this surface.\n\nagent_blocked:\n  - surface: keio.figshare.com\n    status: 202\n    detail: >-\n      Returns HTTP 202 with a zero-byte body to a scripted client — a bot\
  \ interstitial. Recorded as\n      a fact about the platform's edge, not about Keio.\n  - surface: www.linkedin.com/school/keio-university/\n    status: 999\n    detail: LinkedIn's standard bot rejection. The pointer is live for a human; not a dead link.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keio/refs/heads/main/agentic-access/keio-agentic-access.yml
summary_line: 0 operations
tags:
- Education
- Higher Education
- University
- Japan
- Research
- Institutional Repository
- Research Repository
- Identity Federation
- Digital Collections
- IIIF
- OAI-PMH
- Open Access
- Cultural Heritage
---
