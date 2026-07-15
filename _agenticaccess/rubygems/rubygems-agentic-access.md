---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 19
api_specs:
- filename: rubygems-gems-api-openapi.yml
  format: yaml
  label: RubyGems Gems API
  slug: gems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-gems-api-openapi.yml
- filename: rubygems-api-v2-openapi.yml
  format: yaml
  label: RubyGems API V2
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-api-v2-openapi.yml
- filename: rubygems-downloads-api-openapi.yml
  format: yaml
  label: RubyGems Downloads API
  slug: downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-downloads-api-openapi.yml
- filename: rubygems-search-api-openapi.yml
  format: yaml
  label: RubyGems Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-search-api-openapi.yml
- filename: rubygems-activity-api-openapi.yml
  format: yaml
  label: RubyGems Activity API
  slug: activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-activity-api-openapi.yml
- filename: rubygems-webhooks-api-openapi.yml
  format: yaml
  label: RubyGems Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-webhooks-api-openapi.yml
consequence_counts:
  read: 19
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rubygems Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'RubyGems exposes 28 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RubyGems
provider_slug: rubygems
slug: rubygems-agentic-access
source_filename: rubygems-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/rubygems-activity-api-openapi.yml, openapi/rubygems-api-v2-openapi.yml, openapi/rubygems-downloads-api-openapi.yml,\n  openapi/rubygems-gems-api-openapi.yml, openapi/rubygems-search-api-openapi.yml, openapi/rubygems-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 19\n    acting: 9\n  by_consequence:\n    read: 19\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /activity/latest.json\n  method: get\n  operationId: getLatestGems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity/just_updated.json\n\
  \  method: get\n  operationId: getJustUpdatedGems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rubygems/{gemName}/versions/{versionNumber}.json\n  method: get\n  operationId: getGemVersionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /downloads.json\n  method: get\n  operationId: getTotalDownloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /downloads/{gemNameVersion}.json\n  method: get\n  operationId: getVersionDownloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gems/{gemName}.json\n  method: get\n  operationId: getGemInfo\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gems.json\n  method: get\n  operationId: listOwnedGems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gems\n  method: post\n  operationId: pushGem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gems/yank\n  method: delete\n  operationId: yankGem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /gems/{gemName}/reverse_dependencies.json\n  method: get\n  operationId: getReverseDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /versions/{gemName}.json\n  method: get\n  operationId: getGemVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /versions/{gemName}/latest.json\n  method: get\n  operationId: getLatestGemVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeframe_versions.json\n  method: get\n  operationId: getTimeframeVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /owners/{userHandle}/gems.json\n  method: get\n\
  \  operationId: listGemsByOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gems/{gemName}/owners.json\n  method: get\n  operationId: listGemOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gems/{gemName}/owners\n  method: post\n  operationId: addGemOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gems/{gemName}/owners\n  method: delete\n  operationId: removeGemOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gems/{gemName}/owners\n  method: patch\n  operationId: updateGemOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{userHandle}.json\n  method: get\n  operationId: getUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/me.json\n  method: get\n  operationId: getMyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dependencies\n  method: get\n  operationId: getDependencies\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_key.json\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oidc/trusted_publisher/exchange_token\n  method: post\n  operationId: exchangeOidcToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search.json\n  method: get\n  operationId: searchGems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web_hooks.json\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web_hooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web_hooks/remove\n  method: delete\n  operationId: removeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web_hooks/fire\n  method: post\n  operationId: fireWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/agentic-access/rubygems-agentic-access.yml
summary_line: 28 operations · 9 acting
tags:
- Ruby
- Package Manager
- Open Source
- Developer Tools
---
