---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: magento-watch-meta-api-openapi.yml
  format: yaml
  label: magento-watch Meta API
  slug: magento-watch-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-meta-api-openapi.yml
- filename: magento-watch-patches-api-openapi.yml
  format: yaml
  label: magento-watch Patches API
  slug: magento-watch-patches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-patches-api-openapi.yml
- filename: magento-watch-security-api-openapi.yml
  format: yaml
  label: magento-watch Security API
  slug: magento-watch-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-security-api-openapi.yml
- filename: magento-watch-upstream-fixes-api-openapi.yml
  format: yaml
  label: magento-watch Upstream Fixes API
  slug: magento-watch-upstream-fixes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-upstream-fixes-api-openapi.yml
- filename: magento-watch-versions-api-openapi.yml
  format: yaml
  label: magento-watch Versions API
  slug: magento-watch-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-versions-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Magento Watch Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'magento-watch exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: magento-watch
provider_slug: magento-watch
slug: magento-watch-agentic-access
source_filename: magento-watch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/magento-watch-openapi.json, openapi/magento-watch.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{distribution}/versions\n  method:\
  \ get\n  operationId: getVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{distribution}/versions/supported\n  method: get\n  operationId: getSupportedVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{distribution}/versions/secure\n  method: get\n  operationId: getSecureVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{distribution}/versions/latest\n  method: get\n  operationId: getLatestVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/security-bulletins\n  method: get\n  operationId: getSecurityBulletins\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/security-bulletins/{id}\n  method: get\n  operationId: getSecurityBulletin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patches/search\n  method: get\n  operationId: getPatchSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patches/{id}/composer.zip\n  method: get\n  operationId: getPatchComposerBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patches/{id}/composer/{vendor}/{file}\n  method: get\n  operationId: getPatchComposerFile\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patches/{id}\n  method: get\n  operationId: getPatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patches\n  method: get\n  operationId: getPatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{distribution}/versions/{version}/patches\n  method: get\n  operationId: getVersionPatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{distribution}/versions/{version}/security\n  method: get\n  operationId: getVersionSecurity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/v1/{distribution}/versions/{version}\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{distribution}/versions/{version}/upstream-fixes\n  method: get\n  operationId: getVersionUpstreamFixes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/upstream-fixes/search\n  method: get\n  operationId: getUpstreamFixSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/upstream-fixes/{id}/composer.zip\n  method: get\n  operationId: getUpstreamFixComposerBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/upstream-fixes/{id}/composer/{vendor}/{file}\n  method: get\n  operationId: getUpstreamFixComposerFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/upstream-fixes/{id}\n  method: get\n  operationId: getUpstreamFix\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/upstream-fixes\n  method: get\n  operationId: getUpstreamFixes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/magento-watch/agentic-access/magento-watch-agentic-access.yml
summary_line: 22 operations
tags:
- Company
- Magento
- Lifecycle
- Open Source
---
