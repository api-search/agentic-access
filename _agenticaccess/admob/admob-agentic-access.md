---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 12
api_specs:
- filename: admob-accounts-api-openapi.yml
  format: yaml
  label: AdMob Accounts API
  slug: admob-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-accounts-api-openapi.yml
- filename: admob-adapters-api-openapi.yml
  format: yaml
  label: AdMob Adapters API
  slug: admob-adapters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-adapters-api-openapi.yml
- filename: admob-adsources-api-openapi.yml
  format: yaml
  label: AdMob Ad Sources API
  slug: admob-adsources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-adsources-api-openapi.yml
- filename: admob-adunitmappings-api-openapi.yml
  format: yaml
  label: AdMob Ad Unit Mappings API
  slug: admob-adunitmappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-adunitmappings-api-openapi.yml
- filename: admob-adunits-api-openapi.yml
  format: yaml
  label: AdMob Ad Units API
  slug: admob-adunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-adunits-api-openapi.yml
- filename: admob-apps-api-openapi.yml
  format: yaml
  label: AdMob Apps API
  slug: admob-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-apps-api-openapi.yml
- filename: admob-campaignreport-api-openapi.yml
  format: yaml
  label: AdMob Campaign Report API
  slug: admob-campaignreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-campaignreport-api-openapi.yml
- filename: admob-mediationabexperiments-api-openapi.yml
  format: yaml
  label: AdMob Mediation Ab Experiments API
  slug: admob-mediationabexperiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-mediationabexperiments-api-openapi.yml
- filename: admob-mediationgroups-api-openapi.yml
  format: yaml
  label: AdMob Mediation Groups API
  slug: admob-mediationgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-mediationgroups-api-openapi.yml
- filename: admob-mediationreport-api-openapi.yml
  format: yaml
  label: AdMob Mediation Report API
  slug: admob-mediationreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-mediationreport-api-openapi.yml
- filename: admob-networkreport-api-openapi.yml
  format: yaml
  label: AdMob Network Report API
  slug: admob-networkreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/openapi/admob-networkreport-api-openapi.yml
consequence_counts:
  read: 12
  safety-critical: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Admob Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1beta/accounts/{accountsId}/mediationGroups/{mediationGroupsId}/mediationAbExperiments:stop
operation_count: 25
overview: 'AdMob exposes 25 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 12 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AdMob
provider_slug: admob
slug: admob-agentic-access
source_filename: admob-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/admob-api-v1-openapi.yml, openapi/admob-api-v1beta-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 12\n    acting: 13\n  by_consequence:\n    read: 12\n    write: 12\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/accounts/{accountsId}\n  method: get\n  operationId: accounts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts\n  method: get\n  operationId: accounts_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountsId}/adUnits\n  method: get\n  operationId: accounts_adUnits_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountsId}/networkReport:generate\n  method: post\n  operationId: accounts_networkReport_generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{accountsId}/mediationReport:generate\n  method: post\n  operationId: accounts_mediationReport_generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{accountsId}/apps\n  method: get\n  operationId: accounts_apps_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/accounts/{accountsId}\n  method: get\n  operationId: accounts_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/accounts\n  method: get\n  operationId: accounts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/accounts/{accountsId}/apps\n  method: post\n  operationId: accounts_apps_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n\
  \    - https://www.googleapis.com/auth/admob.report\n- path: /v1beta/accounts/{accountsId}/apps\n  method: get\n  operationId: accounts_apps_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/accounts/{accountsId}/adSources\n  method: get\n  operationId: accounts_adSources_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/accounts/{accountsId}/adSources/{adSourcesId}/adapters\n  method: get\n  operationId: accounts_adSources_adapters_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/accounts/{accountsId}/networkReport:generate\n  method: post\n  operationId: accounts_networkReport_generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/accounts/{accountsId}/mediationReport:generate\n  method: post\n  operationId: accounts_mediationReport_generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/accounts/{accountsId}/campaignReport:generate\n  method: post\n  operationId: accounts_campaignReport_generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/accounts/{accountsId}/adUnits\n  method: get\n  operationId: accounts_adUnits_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/accounts/{accountsId}/adUnits\n  method: post\n  operationId:\
  \ accounts_adUnits_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n- path: /v1beta/accounts/{accountsId}/adUnits/{adUnitsId}/adUnitMappings\n  method: post\n  operationId: accounts_adUnits_adUnitMappings_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n- path: /v1beta/accounts/{accountsId}/adUnits/{adUnitsId}/adUnitMappings\n\
  \  method: get\n  operationId: accounts_adUnits_adUnitMappings_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/accounts/{accountsId}/mediationGroups\n  method: get\n  operationId: accounts_mediationGroups_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta/accounts/{accountsId}/mediationGroups\n  method: post\n  operationId: accounts_mediationGroups_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  \    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n- path: /v1beta/accounts/{accountsId}/mediationGroups/{mediationGroupsId}\n  method: patch\n  operationId: accounts_mediationGroups_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n- path: /v1beta/accounts/{accountsId}/mediationGroups/{mediationGroupsId}/mediationAbExperiments\n  method: post\n  operationId: accounts_mediationGroups_mediationAbExperiments_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n- path: /v1beta/accounts/{accountsId}/mediationGroups/{mediationGroupsId}/mediationAbExperiments:stop\n  method: post\n  operationId: accounts_mediationGroups_mediationAbExperiments_stop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n- path: /v1beta/accounts/{accountsId}/adUnitMappings:batchCreate\n  method: post\n  operationId: accounts_adUnitMappings_batchCreate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/admob.readonly\n    - https://www.googleapis.com/auth/admob.report\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/agentic-access/admob-agentic-access.yml
summary_line: 25 operations · 13 acting · 1 human-in-the-loop
tags:
- Company
- Advertising
- Mobile
- Monetization
- Ads
- Google
- Reporting
- Mediation
- AdTech
---
