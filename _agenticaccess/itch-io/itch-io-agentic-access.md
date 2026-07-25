---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 26
api_specs:
- filename: itch-io-auth-api-openapi.yml
  format: yaml
  label: Itch.io Auth API
  slug: itch-io-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-auth-api-openapi.yml
- filename: itch-io-builds-api-openapi.yml
  format: yaml
  label: Itch.io Builds API
  slug: itch-io-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-builds-api-openapi.yml
- filename: itch-io-bundles-api-openapi.yml
  format: yaml
  label: Itch.io Bundles API
  slug: itch-io-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-bundles-api-openapi.yml
- filename: itch-io-collections-api-openapi.yml
  format: yaml
  label: Itch.io Collections API
  slug: itch-io-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-collections-api-openapi.yml
- filename: itch-io-downloads-api-openapi.yml
  format: yaml
  label: Itch.io Downloads API
  slug: itch-io-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-downloads-api-openapi.yml
- filename: itch-io-games-api-openapi.yml
  format: yaml
  label: Itch.io Games API
  slug: itch-io-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-games-api-openapi.yml
- filename: itch-io-profile-api-openapi.yml
  format: yaml
  label: Itch.io Profile API
  slug: itch-io-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-profile-api-openapi.yml
- filename: itch-io-search-api-openapi.yml
  format: yaml
  label: Itch.io Search API
  slug: itch-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-search-api-openapi.yml
- filename: itch-io-uploads-api-openapi.yml
  format: yaml
  label: Itch.io Uploads API
  slug: itch-io-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-uploads-api-openapi.yml
- filename: itch-io-users-api-openapi.yml
  format: yaml
  label: Itch.io Users API
  slug: itch-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-users-api-openapi.yml
- filename: itch-io-wharf-api-openapi.yml
  format: yaml
  label: Itch.io Wharf API
  slug: itch-io-wharf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/openapi/itch-io-wharf-api-openapi.yml
consequence_counts:
  read: 26
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Itch Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'Itch.io exposes 36 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Itch.io
provider_slug: itch-io
slug: itch-io-agentic-access
source_filename: itch-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 26\n    acting: 10\n  by_consequence:\n    read: 26\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/games\n  method: get\n  operationId: listProfileGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/owned-keys\n  method: get\n  operationId:\
  \ listProfileOwnedKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/collections\n  method: get\n  operationId: listProfileCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/owned-bundles\n  method: get\n  operationId: listProfileOwnedBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile/builds\n  method: get\n  operationId: listProfileBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /games/{gameId}\n  method: get\n  operationId: getGame\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /games/{gameId}/uploads\n  method: get\n  operationId: listGameUploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /games/{gameId}/download-sessions\n  method: post\n  operationId: newDownloadSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads/{uploadId}\n  method: get\n  operationId: getUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploads/{uploadId}/builds\n  method: get\n  operationId: listUploadBuilds\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploads/{uploadId}/scanned-archive\n  method: get\n  operationId: getUploadScannedArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /builds/{buildId}\n  method: get\n  operationId: getBuild\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /builds/{buildId}/upgrade-paths/{targetBuildId}\n  method: get\n  operationId: getBuildUpgradePath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /builds/{buildId}/scanned-archive\n  method: get\n  operationId: getBuildScannedArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/collection-games\n  method: get\n  operationId: getCollectionGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundleId}/bundle-games\n  method: get\n  operationId: getBundleGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundleId}/claim-game\n\
  \  method: post\n  operationId: claimBundleGame\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/games\n  method: get\n  operationId: searchGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/users\n  method: get\n  operationId: searchUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login\n  method: post\n  operationId: loginWithPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login/with-totp-token\n  method: post\n  operationId: totpVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wharf/status\n  method: get\n  operationId: wharfStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wharf/channels\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wharf/channels/{channelName}\n  method: get\n  operationId: getChannel\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wharf/builds\n  method: post\n  operationId: createBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wharf/builds/{buildId}\n  method: get\n  operationId: getWharfBuild\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wharf/builds/{buildId}/files\n  method: get\n  operationId: listBuildFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wharf/builds/{buildId}/files\n  method: post\n  operationId: createBuildFile\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wharf/builds/{buildId}/files/{fileId}\n  method: post\n  operationId: finalizeBuildFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wharf/builds/{buildId}/events\n  method: get\n  operationId: listBuildEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wharf/builds/{buildId}/events\n  method: post\n  operationId: createBuildEvent\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wharf/builds/{buildId}/failures\n  method: post\n  operationId: createBuildFailure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wharf/builds/{buildId}/failures/rediff\n  method: post\n  operationId: createRediffBuildFailure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itch-io/refs/heads/main/agentic-access/itch-io-agentic-access.yml
summary_line: 36 operations · 10 acting
tags:
- Games
- Indie Games
- Game Distribution
- Game Marketplace
- Developers
---
