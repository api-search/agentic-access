---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: r-metacran-crandb-openapi.yml
  format: yaml
  label: METACRAN CranDB API
  slug: metacran-crandb
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/openapi/r-metacran-crandb-openapi.yml
- filename: r-metacran-cranlogs-openapi.yml
  format: yaml
  label: METACRAN CranLogs API
  slug: metacran-cranlogs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/openapi/r-metacran-cranlogs-openapi.yml
- filename: r-rversions-openapi.yml
  format: yaml
  label: R Versions API
  slug: rversions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/openapi/r-rversions-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: R Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'R exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: R
provider_slug: r
slug: r-agentic-access
source_filename: r-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/r-metacran-crandb-openapi.yml, openapi/r-metacran-cranlogs-openapi.yml, openapi/r-rversions-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /{package}\n  method: get\n  operationId: getPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{package}/{version}\n  method: get\n  operationId: getPackageVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /-/pkgs\n  method: get\n  operationId: listAllPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/desc\n  method: get\n  operationId: listPackageDescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /-/allvign\n  method: get\n  operationId: listPackageVignettes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /downloads/total/{period}/{packages}\n  method: get\n  operationId: getPackageDownloadTotals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /downloads/daily/{period}/{packages}\n  method: get\n  operationId: getPackageDownloadDaily\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /top/{period}/{count}\n  method: get\n  operationId: getTopPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /badges/{period}/{package}\n  method: get\n  operationId: getDownloadBadge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /r-release\n  method: get\n  operationId: getRRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /r-release-win\n  method: get\n  operationId: getRReleaseWindows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /r-release-macos\n  method: get\n  operationId: getRReleaseMacos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /r-oldrel\n  method: get\n  operationId: getROldrel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /r-versions\n  method: get\n  operationId: listRVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/agentic-access/r-agentic-access.yml
summary_line: 14 operations
tags:
- R
- Statistics
- Data Science
- Open Source
- Programming Language
---
