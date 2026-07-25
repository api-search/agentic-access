---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 15
api_specs:
- filename: mojang-attributes-api-openapi.yml
  format: yaml
  label: Mojang Attributes API
  slug: mojang-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-attributes-api-openapi.yml
- filename: mojang-authentication-api-openapi.yml
  format: yaml
  label: Mojang Authentication API
  slug: mojang-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-authentication-api-openapi.yml
- filename: mojang-blocklist-api-openapi.yml
  format: yaml
  label: Mojang Blocklist API
  slug: mojang-blocklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-blocklist-api-openapi.yml
- filename: mojang-capes-api-openapi.yml
  format: yaml
  label: Mojang Capes API
  slug: mojang-capes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-capes-api-openapi.yml
- filename: mojang-entitlements-api-openapi.yml
  format: yaml
  label: Mojang Entitlements API
  slug: mojang-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-entitlements-api-openapi.yml
- filename: mojang-friends-api-openapi.yml
  format: yaml
  label: Mojang Friends API
  slug: mojang-friends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-friends-api-openapi.yml
- filename: mojang-identity-api-openapi.yml
  format: yaml
  label: Mojang Identity API
  slug: mojang-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-identity-api-openapi.yml
- filename: mojang-keys-api-openapi.yml
  format: yaml
  label: Mojang Keys API
  slug: mojang-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-keys-api-openapi.yml
- filename: mojang-presence-api-openapi.yml
  format: yaml
  label: Mojang Presence API
  slug: mojang-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-presence-api-openapi.yml
- filename: mojang-profile-api-openapi.yml
  format: yaml
  label: Mojang Profile API
  slug: mojang-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-profile-api-openapi.yml
- filename: mojang-server-api-openapi.yml
  format: yaml
  label: Mojang Server API
  slug: mojang-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-server-api-openapi.yml
- filename: mojang-session-api-openapi.yml
  format: yaml
  label: Mojang Session API
  slug: mojang-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-session-api-openapi.yml
- filename: mojang-skins-api-openapi.yml
  format: yaml
  label: Mojang Skins API
  slug: mojang-skins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-skins-api-openapi.yml
- filename: mojang-textures-api-openapi.yml
  format: yaml
  label: Mojang Textures API
  slug: mojang-textures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/openapi/mojang-textures-api-openapi.yml
consequence_counts:
  physical: 1
  read: 15
  safety-critical: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Mojang Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /minecraft/profile/skins/active
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/statistics
operation_count: 29
overview: 'Mojang exposes 29 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 12 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mojang
provider_slug: mojang
slug: mojang-agentic-access
source_filename: mojang-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mojang-minecraft-services-openapi.yml, openapi/mojang-public-api-openapi.yml,\n  openapi/mojang-session-server-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 14\n    connected: 15\n  by_consequence:\n    write: 12\n    read: 15\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /authentication/login_with_xbox\n  method: post\n  operationId: loginWithXbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /minecraft/profile/lookup/name/{username}\n  method: get\n  operationId: lookupProfileByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minecraft/profile/lookup/{uuid}\n  method: get\n  operationId: lookupProfileByUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minecraft/profile/lookup/bulk/byname\n  method: post\n  operationId: lookupProfilesBulkByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /minecraft/profile\n  method: get\n  operationId: getAuthenticatedProfile\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minecraft/profile/namechange\n  method: get\n  operationId: getNameChangeInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minecraft/profile/name/{name}/available\n  method: get\n  operationId: checkNameAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minecraft/profile/name/{name}\n  method: put\n  operationId: changeName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /minecraft/profile/skins\n\
  \  method: post\n  operationId: changeSkin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /minecraft/profile/skins/active\n  method: delete\n  operationId: resetSkin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /minecraft/profile/capes/active\n  method: put\n  operationId: showCape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /minecraft/profile/capes/active\n  method: delete\n  operationId: hideCape\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /player/attributes\n  method: get\n  operationId: getPlayerAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /player/attributes\n  method: post\n  operationId: updatePlayerAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /privacy/blocklist\n  method: get\n  operationId: getBlocklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /friends\n  method: get\n  operationId: getFriends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /friends\n  method: put\n  operationId: updateFriends\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /presence\n  method: post\n  operationId: reportPresence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /player/certificates\n  method: post\n  operationId: getPlayerCertificates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /publickeys\n  method: get\n  operationId: getPublicKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entitlements/mcstore\n  method: get\n  operationId: getMinecraftEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/profiles/minecraft/{username}\n  method: get\n \
  \ operationId: getProfileByUsername\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/minecraft\n  method: post\n  operationId: getProfilesByUsernamesBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/profiles/{uuid}/names\n  method: get\n  operationId: getNameHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/statistics\n  method: post\n  operationId: getSaleStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session/minecraft/profile/{uuid}\n  method: get\n  operationId: getSessionProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /session/minecraft/hasJoined\n  method: get\n  operationId: hasJoined\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /session/minecraft/join\n  method: post\n  operationId: joinSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /blockedservers\n  method: get\n  operationId: getBlockedServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mojang/refs/heads/main/agentic-access/mojang-agentic-access.yml
summary_line: 29 operations · 14 acting · 1 human-in-the-loop
tags:
- Games And Comics
- Minecraft
- Gaming
- Identity
- Player Profiles
- Session
- Public APIs
---
