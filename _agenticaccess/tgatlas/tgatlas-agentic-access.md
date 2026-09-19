---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: tgatlas-openapi.json
  format: json
  label: ChannelIndex Telegram Channel Data API
  slug: channelindex-telegram-channel-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tgatlas/refs/heads/main/openapi/tgatlas-openapi.json
consequence_counts: {}
description: 'Recommended x-agentic-access contract. Every one of the 19 operations is a read-only GET over public Telegram data, so the entire surface is low consequence and safe for autonomous agent use under a subscriber key. There is no write, no mutation and no destructive action to escalate. The only cost dimension is quota: four discovery routes spend the metered "lookups" counter.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tgatlas Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'ChannelIndex (tgAtlas) exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ChannelIndex (tgAtlas)
provider_slug: tgatlas
slug: tgatlas-agentic-access
source_filename: tgatlas-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/tgatlas-openapi.json (classification of every operation)\nprovider: tgAtlas\napi: tgAtlas Telegram Channel Data API\ndescription: >-\n  Recommended x-agentic-access contract. Every one of the 19 operations is a\n  read-only GET over public Telegram data, so the entire surface is low\n  consequence and safe for autonomous agent use under a subscriber key. There is\n  no write, no mutation and no destructive action to escalate. The only cost\n  dimension is quota: four discovery routes spend the metered \"lookups\" counter.\ndefaults:\n  action_class: read\n  consequence: low\n  reversibility: na\n  token: api-key\n  escalation: none\n  human_in_the_loop: not-required\noperations:\n  - group: read-cheap\n    consequence: low\n    note: Spends one request; no lookup counter. Safe to call in volume.\n    operationIds:\n      - health\n      - getChannels\n      - getFullChannel\n      - getChannelMessages\n      - getChannelParticipants\n\
  \      - getHistory\n      - getDiscussionMessage\n      - getReplies\n      - getPeerStories\n      - getStoriesByID\n      - getFullUser\n      - getUserPhotos\n      - downloadFile\n      - getOpenAPIDocument\n  - group: read-metered-lookup\n    consequence: low\n    note: >-\n      Spends the discovery \"lookups\" counter in addition to a request. An agent\n      running large sweeps should prefer the cheap read routes and reserve these\n      for genuine discovery.\n    operationIds:\n      - resolveUsername\n      - getChannelRecommendations\n      - searchContacts\n      - searchMessages\n  - group: read-metered-phone\n    consequence: low\n    note: resolvePhone draws down a separate phone-resolution counter.\n    operationIds:\n      - resolvePhone\nguardrails:\n  - Respect the x-ratelimit-*-remaining headers; back off on 429 until reset.\n  - Seed unknown peer ids via a resolve route before reading (else 409 RESOURCE_UNAVAILABLE).\n  - Scope is public metadata only; no private\
  \ groups or message contents are returned.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tgatlas/refs/heads/main/agentic-access/tgatlas-agentic-access.yml
summary_line: 3 operations
tags:
- Telegram
- Public Channels
- Social-Media
- Social Monitoring
- Messaging
- Directory
- Search
- Analytics
- OSINT
- Market Research
- AI-agent context
---
