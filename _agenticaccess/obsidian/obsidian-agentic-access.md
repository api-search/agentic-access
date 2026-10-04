---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 13
api_specs:
- filename: obsidian-active-file-api-openapi.yml
  format: yaml
  label: Obsidian Active File API
  slug: obsidian-active-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-active-file-api-openapi.yml
- filename: obsidian-commands-api-openapi.yml
  format: yaml
  label: Obsidian Commands API
  slug: obsidian-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-commands-api-openapi.yml
- filename: obsidian-open-api-openapi.yml
  format: yaml
  label: Obsidian Open API
  slug: obsidian-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-open-api-openapi.yml
- filename: obsidian-periodic-notes-api-openapi.yml
  format: yaml
  label: Obsidian Periodic Notes API
  slug: obsidian-periodic-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-periodic-notes-api-openapi.yml
- filename: obsidian-search-api-openapi.yml
  format: yaml
  label: Obsidian Search API
  slug: obsidian-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-search-api-openapi.yml
- filename: obsidian-system-api-openapi.yml
  format: yaml
  label: Obsidian System API
  slug: obsidian-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-system-api-openapi.yml
- filename: obsidian-tags-api-openapi.yml
  format: yaml
  label: Obsidian Tags API
  slug: obsidian-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-tags-api-openapi.yml
- filename: obsidian-vault-directories-api-openapi.yml
  format: yaml
  label: Obsidian Vault Directories API
  slug: obsidian-vault-directories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-vault-directories-api-openapi.yml
- filename: obsidian-vault-files-api-openapi.yml
  format: yaml
  label: Obsidian Vault Files API
  slug: obsidian-vault-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/openapi/obsidian-vault-files-api-openapi.yml
consequence_counts:
  read: 13
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Obsidian Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /open/{filename}
operation_count: 31
overview: 'Obsidian exposes 31 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 17 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Obsidian
provider_slug: obsidian
slug: obsidian-agentic-access
source_filename: obsidian-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/obsidian-active-file-api-openapi.yml, openapi/obsidian-commands-api-openapi.yml,\n  openapi/obsidian-open-api-openapi.yml, openapi/obsidian-periodic-notes-api-openapi.yml, openapi/obsidian-search-api-openapi.yml,\n  openapi/obsidian-system-api-openapi.yml, openapi/obsidian-tags-api-openapi.yml, openapi/obsidian-vault-directories-api-openapi.yml,\n  openapi/obsidian-vault-files-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 18\n    connected: 13\n  by_consequence:\n    write: 17\n    read: 13\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /active/\n  method: delete\n  operationId: deleteActive\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /active/\n  method: get\n  operationId: getActive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /active/\n  method: patch\n  operationId: patchActive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /active/\n  method: post\n  operationId: postActive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /active/\n  method: put\n  operationId: putActive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/\n  method: get\n  operationId: getCommands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commands/{commandId}/\n  method: post\n  operationId: postCommandsByCommandId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /open/{filename}\n  method: post\n  operationId: postOpenByFilename\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /periodic/{period}/\n  method: delete\n  operationId: deletePeriodicByPeriod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /periodic/{period}/\n  method: get\n  operationId: getPeriodicByPeriod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /periodic/{period}/\n  method: patch\n  operationId: patchPeriodicByPeriod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /periodic/{period}/\n  method: post\n  operationId: postPeriodicByPeriod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /periodic/{period}/\n  method: put\n  operationId: putPeriodicByPeriod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /periodic/{period}/{year}/{month}/{day}/\n  method: delete\n  operationId: deletePeriodicByPeriodByYearByMonthByDay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /periodic/{period}/{year}/{month}/{day}/\n  method: get\n  operationId: getPeriodicByPeriodByYearByMonthByDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /periodic/{period}/{year}/{month}/{day}/\n  method: patch\n  operationId: patchPeriodicByPeriodByYearByMonthByDay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /periodic/{period}/{year}/{month}/{day}/\n  method: post\n  operationId: postPeriodicByPeriodByYearByMonthByDay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /periodic/{period}/{year}/{month}/{day}/\n  method: put\n  operationId: putPeriodicByPeriodByYearByMonthByDay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/\n  method: post\n  operationId: postSearch\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/simple/\n  method: post\n  operationId: postSearchSimple\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /obsidian-local-rest-api.crt\n  method: get\n  operationId: getObsidianLocalRestApiCrt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.yaml\n  method: get\n  operationId: getOpenapiYaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /tags/\n  method: get\n  operationId: getTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vault/\n  method: get\n  operationId: getVault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vault/{pathToDirectory}/\n  method: get\n  operationId: getVaultByPathToDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vault/{filename}\n  method: delete\n  operationId: deleteVaultByFilename\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /vault/{filename}\n  method: get\n  operationId: getVaultByFilename\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vault/{filename}\n  method: patch\n  operationId: patchVaultByFilename\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vault/{filename}\n  method: post\n  operationId: postVaultByFilename\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vault/{filename}\n  method: put\n\
  \  operationId: putVaultByFilename\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/obsidian/refs/heads/main/agentic-access/obsidian-agentic-access.yml
summary_line: 31 operations · 18 acting · 1 human-in-the-loop
tags:
- Productivity
- Knowledge Management
- Markdown
- Notes
- Local-First
---
