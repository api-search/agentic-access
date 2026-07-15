---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 10
api_specs:
- filename: typo3-releases-openapi.json
  format: json
  label: TYPO3 Releases REST API
  slug: releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typo3/refs/heads/main/openapi/typo3-releases-openapi.json
consequence_counts:
  read: 10
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Typo3 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'TYPO3 exposes 23 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TYPO3
provider_slug: typo3
slug: typo3-agentic-access
source_filename: typo3-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/typo3-releases-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 13\n    connected: 10\n  by_consequence:\n    write: 13\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/cache/majorVersion/{version}\n  method: delete\n  operationId: delete_app_api_cache_purgemajorrelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cache/release/{version}\n  method: delete\n  operationId:\
  \ delete_app_api_cache_purgerelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/major/{version}/release/\n  method: get\n  operationId: get_app_api_majorversion_releases_getreleasesbymajorversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/major/{version}/release/latest\n  method: get\n  operationId: get_app_api_majorversion_releases_getlatestreleasebymajorversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/major/{version}/release/latest/security\n  method: get\n  operationId: get_app_api_majorversion_releases_getlatestsecurityreleasebymajorversion\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/major/{version}/release/latest/content\n  method: get\n  operationId: get_app_api_majorversion_releases_getlatestreleasecontentbymajorversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/major/{version}/requirements\n  method: get\n  operationId: get_app_api_majorversion_requirements_getrequirementsbymajorversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/major/{version}/requirement/\n  method: post\n  operationId: post_app_api_majorversion_requirements_addrequirement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/major/{version}/requirement/\n  method: patch\n  operationId: patch_app_api_majorversion_requirements_updaterequirement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/major/{version}/requirement/{category}/{name}\n  method: delete\n  operationId: delete_app_api_majorversion_requirements_deleterequirement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/major/\n  method: get\n  operationId: get_app_api_majorversion_getmajorreleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/major/\n  method: post\n  operationId: post_app_api_majorversion_createmajorrelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/major/{version}\n  method: get\n  operationId: get_majorVersion_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/major/{version}\n  method: delete\n  operationId: delete_app_api_majorversion_deletemajorrelease\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/major/{version}\n  method: patch\n  operationId: patch_app_api_majorversion_updatemajorrelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/release/\n  method: get\n  operationId: get_app_api_release_getrelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/release/\n  method: post\n  operationId: post_app_api_release_addrelease\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/release/{version}\n  method: get\n  operationId: get_release_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/release/{version}\n  method: delete\n  operationId: delete_app_api_release_deleterelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/release/{version}\n  method: patch\n  operationId: patch_app_api_release_updaterelease\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/release/{version}/release-notes\n  method: put\n  operationId: put_app_api_release_addreleasenotesforversion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/release/{version}/content\n  method: get\n  operationId: get_app_api_release_getcontentforversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sitepackage/\n  method: post\n  operationId: post_app_api_sitepackage_createsitepackage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typo3/refs/heads/main/agentic-access/typo3-agentic-access.yml
summary_line: 23 operations · 13 acting
tags:
- CMS
- Content Management
- Enterprise
- PHP
- Headless
- JSON API
- Open Source
---
