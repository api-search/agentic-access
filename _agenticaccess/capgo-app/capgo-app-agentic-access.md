---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 12
api_specs:
- filename: capgo-app-api-keys-api-openapi.yml
  format: yaml
  label: Capgo API Keys API
  slug: capgo-app-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-api-keys-api-openapi.yml
- filename: capgo-app-apps-api-openapi.yml
  format: yaml
  label: Capgo Apps API
  slug: capgo-app-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-apps-api-openapi.yml
- filename: capgo-app-bundles-api-openapi.yml
  format: yaml
  label: Capgo Bundles API
  slug: capgo-app-bundles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-bundles-api-openapi.yml
- filename: capgo-app-channels-api-openapi.yml
  format: yaml
  label: Capgo Channels API
  slug: capgo-app-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-channels-api-openapi.yml
- filename: capgo-app-devices-api-openapi.yml
  format: yaml
  label: Capgo Devices API
  slug: capgo-app-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-devices-api-openapi.yml
- filename: capgo-app-members-api-openapi.yml
  format: yaml
  label: Capgo Members API
  slug: capgo-app-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-members-api-openapi.yml
- filename: capgo-app-organizations-api-openapi.yml
  format: yaml
  label: Capgo Organizations API
  slug: capgo-app-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-organizations-api-openapi.yml
- filename: capgo-app-statistics-api-openapi.yml
  format: yaml
  label: Capgo Statistics API
  slug: capgo-app-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-statistics-api-openapi.yml
consequence_counts:
  read: 12
  safety-critical: 2
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Capgo App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /device/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /device/
operation_count: 30
overview: 'Capgo exposes 30 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 16 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Capgo
provider_slug: capgo-app
slug: capgo-app-agentic-access
source_filename: capgo-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/capgo-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 12\n    acting: 18\n  by_consequence:\n    read: 12\n    write: 16\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /organization/\n  method: get\n  operationId: getOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /organization/\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /organization/\n  method: put\n  operationId: updateOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /organization/\n  method: delete\n  operationId: deleteOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /organization/members/\n  method: get\n  operationId: listOrganizationMembers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /organization/members/\n  method: post\n  operationId: upsertOrganizationMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /organization/members/\n  method: delete\n  operationId: deleteOrganizationMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /app/\n  method: get\n  operationId:\
  \ listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /app/\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /app/{appId}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /app/{appId}\n  method: put\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /app/{appId}\n  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /apikey/\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /apikey/\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /apikey/{id}/\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /channel/\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /channel/\n  method: post\n  operationId: upsertChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /channel/\n  method: delete\n  operationId: deleteChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /device/\n  method: get\n  operationId: getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /device/\n  method: post\n  operationId: linkDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n    scope:\n    - capgo\n- path: /device/\n  method: delete\n  operationId: deleteDeviceOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - capgo\n- path: /bundle/\n  method: get\n  operationId: listBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /bundle/\n  method: post\n  operationId: createBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /bundle/\n  method: put\n  operationId: setBundleChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /bundle/\n  method: delete\n  operationId: deleteBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /bundle/metadata\n  method: post\n  operationId: updateBundleMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - capgo\n- path: /statistics/app/{appId}/\n  method: get\n  operationId: getAppStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /statistics/app/{appId}/bundle_usage\n  method: get\n  operationId: getAppBundleUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /statistics/org/{orgId}/\n  method: get\n  operationId: getOrganizationStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n- path: /statistics/user/\n  method: get\n\
  \  operationId: getUserStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - capgo\n"
source_yaml_url: https://artifacts.apis.io/capgo-app/agentic-access/capgo-app-agentic-access.yml
summary_line: 30 operations · 18 acting · 2 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Mobile
- Development
- Capacitor
---
