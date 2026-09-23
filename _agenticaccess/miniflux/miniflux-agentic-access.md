---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 22
api_specs:
- filename: miniflux-api-keys-api-openapi.yml
  format: yaml
  label: Miniflux Api Keys API
  slug: miniflux-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-api-keys-api-openapi.yml
- filename: miniflux-categories-api-openapi.yml
  format: yaml
  label: Miniflux Categories API
  slug: miniflux-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-categories-api-openapi.yml
- filename: miniflux-enclosures-api-openapi.yml
  format: yaml
  label: Miniflux Enclosures API
  slug: miniflux-enclosures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-enclosures-api-openapi.yml
- filename: miniflux-entries-api-openapi.yml
  format: yaml
  label: Miniflux Entries API
  slug: miniflux-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-entries-api-openapi.yml
- filename: miniflux-export-api-openapi.yml
  format: yaml
  label: Miniflux Export API
  slug: miniflux-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-export-api-openapi.yml
- filename: miniflux-feeds-api-openapi.yml
  format: yaml
  label: Miniflux Feeds API
  slug: miniflux-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-feeds-api-openapi.yml
- filename: miniflux-import-api-openapi.yml
  format: yaml
  label: Miniflux Import API
  slug: miniflux-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-import-api-openapi.yml
- filename: miniflux-integrations-api-openapi.yml
  format: yaml
  label: Miniflux Integrations API
  slug: miniflux-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-integrations-api-openapi.yml
- filename: miniflux-liveness-api-openapi.yml
  format: yaml
  label: Miniflux Liveness API
  slug: miniflux-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-liveness-api-openapi.yml
- filename: miniflux-me-api-openapi.yml
  format: yaml
  label: Miniflux Me API
  slug: miniflux-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-me-api-openapi.yml
- filename: miniflux-readiness-api-openapi.yml
  format: yaml
  label: Miniflux Readiness API
  slug: miniflux-readiness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-readiness-api-openapi.yml
- filename: miniflux-users-api-openapi.yml
  format: yaml
  label: Miniflux Users API
  slug: miniflux-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-users-api-openapi.yml
- filename: miniflux-version-api-openapi.yml
  format: yaml
  label: Miniflux Version API
  slug: miniflux-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-version-api-openapi.yml
- filename: miniflux-discover-api-openapi.yml
  format: yaml
  label: Miniflux Discover API
  slug: miniflux-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-discover-api-openapi.yml
- filename: miniflux-flush-history-api-openapi.yml
  format: yaml
  label: Miniflux Flush History API
  slug: miniflux-flush-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-flush-history-api-openapi.yml
- filename: miniflux-healthz-api-openapi.yml
  format: yaml
  label: Miniflux Healthz API
  slug: miniflux-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-healthz-api-openapi.yml
- filename: miniflux-icons-api-openapi.yml
  format: yaml
  label: Miniflux Icons API
  slug: miniflux-icons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-icons-api-openapi.yml
- filename: miniflux-readyz-api-openapi.yml
  format: yaml
  label: Miniflux Readyz API
  slug: miniflux-readyz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-readyz-api-openapi.yml
- filename: miniflux-health-check-api-openapi.yml
  format: yaml
  label: Miniflux Health Check API
  slug: miniflux-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/openapi/miniflux-health-check-api-openapi.yml
consequence_counts:
  read: 22
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Miniflux Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'Miniflux exposes 42 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Miniflux
provider_slug: miniflux
slug: miniflux-agentic-access
source_filename: miniflux-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: generated\nsource: openapi/miniflux-openapi-generated.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 20\n    connected: 22\n  by_consequence:\n    write: 20\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /feeds/{feedID}/entries/import\n  method: post\n  operationId: post_feeds_feedID_entries_import\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /healthcheck\n  method: get\n  operationId: get_healthcheck\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/status\n  method: get\n  operationId: get_integrations_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liveness\n  method: get\n  operationId: get_liveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /readiness\n  method: get\n  operationId: get_readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: get\n  operationId: get_v1_api_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/api-keys\n  method: post\n  operationId: post_v1_api_keys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys/1\n  method: delete\n  operationId: delete_v1_api_keys_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/categories\n  method: get\n  operationId: get_v1_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories\n  method: post\n  operationId: post_v1_categories\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/categories/123\n  method: put\n  operationId: put_v1_categories_123\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/categories/123/mark-all-as-read\n  method: put\n  operationId: put_v1_categories_123_mark_all_as_read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/categories/123/refresh\n  method: put\n  operationId: put_v1_categories_123_refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/categories/22/entries\n  method: get\n  operationId: get_v1_categories_22_entries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories/802\n  method: delete\n  operationId: delete_v1_categories_802\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/categories/802\n\
  \  method: put\n  operationId: put_v1_categories_802\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enclosures/{enclosureID}\n  method: get\n  operationId: get_v1_enclosures_enclosureID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/enclosures/{enclosureID}\n  method: put\n  operationId: put_v1_enclosures_enclosureID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entries\n  method: get\n  operationId:\
  \ get_v1_entries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entries\n  method: put\n  operationId: put_v1_entries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entries/1234/bookmark\n  method: put\n  operationId: put_v1_entries_1234_bookmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entries/888\n  method: get\n  operationId: get_v1_entries_888\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entries/ids\n  method: get\n  operationId: get_v1_entries_ids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entries/{entryID}\n  method: put\n  operationId: put_v1_entries_entryID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entries/{entryID}/fetch-content\n  method: get\n  operationId: get_v1_entries_entryID_fetch_content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entries/{entryID}/save\n  method: post\n  operationId:\
  \ post_v1_entries_entryID_save\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/export\n  method: get\n  operationId: get_v1_export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feeds/123/mark-all-as-read\n  method: put\n  operationId: put_v1_feeds_123_mark_all_as_read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feeds/42/entries\n  method: get\n  operationId: get_v1_feeds_42_entries\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feeds/42/entries/888\n  method: get\n  operationId: get_v1_feeds_42_entries_888\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feeds/counters\n  method: get\n  operationId: get_v1_feeds_counters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/import\n  method: post\n  operationId: post_v1_import\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: get\n  operationId: get_v1_me\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: get\n  operationId: get_v1_users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: post\n  operationId: post_v1_users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/123/mark-all-as-read\n  method: put\n  operationId: put_v1_users_123_mark_all_as_read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/270\n  method: delete\n  operationId: delete_v1_users_270\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/270\n  method: get\n  operationId: get_v1_users_270\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/270\n  method: put\n  operationId: put_v1_users_270\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/foobar\n\
  \  method: get\n  operationId: get_v1_users_foobar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/version\n  method: get\n  operationId: get_v1_version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: get\n  operationId: get_version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miniflux/refs/heads/main/agentic-access/miniflux-agentic-access.yml
summary_line: 42 operations · 20 acting
tags:
- Feed Reader
- Open-Source
- Self-Hosted
- Minimalist
- Privacy
---
