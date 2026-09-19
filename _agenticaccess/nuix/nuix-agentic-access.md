---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 15
api_specs:
- filename: nuix-case-api-openapi.yml
  format: yaml
  label: Nuix Case API
  slug: nuix-case-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-case-api-openapi.yml
- filename: nuix-collection-and-survey-api-openapi.yml
  format: yaml
  label: Nuix Collection and Survey API
  slug: nuix-collection-and-survey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-collection-and-survey-api-openapi.yml
- filename: nuix-collection-configuration-api-openapi.yml
  format: yaml
  label: Nuix Collection Configuration API
  slug: nuix-collection-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-collection-configuration-api-openapi.yml
- filename: nuix-computer-api-openapi.yml
  format: yaml
  label: Nuix Computer API
  slug: nuix-computer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-computer-api-openapi.yml
- filename: nuix-computer-configuration-api-openapi.yml
  format: yaml
  label: Nuix Computer Configuration API
  slug: nuix-computer-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-computer-configuration-api-openapi.yml
- filename: nuix-custodian-api-openapi.yml
  format: yaml
  label: Nuix Custodian API
  slug: nuix-custodian-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-custodian-api-openapi.yml
- filename: nuix-group-api-openapi.yml
  format: yaml
  label: Nuix Group API
  slug: nuix-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-group-api-openapi.yml
- filename: nuix-job-api-openapi.yml
  format: yaml
  label: Nuix Job API
  slug: nuix-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-job-api-openapi.yml
- filename: nuix-log-api-openapi.yml
  format: yaml
  label: Nuix Log API
  slug: nuix-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-log-api-openapi.yml
- filename: nuix-target-api-openapi.yml
  format: yaml
  label: Nuix Target API
  slug: nuix-target-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-target-api-openapi.yml
- filename: nuix-utility-api-openapi.yml
  format: yaml
  label: Nuix Utility API
  slug: nuix-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/openapi/nuix-utility-api-openapi.yml
consequence_counts:
  read: 15
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nuix Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 34
overview: 'Nuix exposes 34 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nuix
provider_slug: nuix
slug: nuix-agentic-access
source_filename: nuix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/nuix-case-api-openapi.yml, openapi/nuix-collection-and-survey-api-openapi.yml,\n  openapi/nuix-collection-configuration-api-openapi.yml, openapi/nuix-computer-api-openapi.yml,\n  openapi/nuix-computer-configuration-api-openapi.yml, openapi/nuix-custodian-api-openapi.yml,\n  openapi/nuix-group-api-openapi.yml, openapi/nuix-job-api-openapi.yml, openapi/nuix-log-api-openapi.yml,\n  openapi/nuix-target-api-openapi.yml, openapi/nuix-utility-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 15\n    acting: 19\n  by_consequence:\n    read: 15\n    write: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/cases\n  method: get\n\
  \  operationId: listCasesAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cases\n  method: post\n  operationId: createCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cases/{caseId}\n  method: get\n  operationId: listCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cases/{id}\n  method: put\n  operationId: modifyCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cases/{id}\n  method: delete\n  operationId: deleteCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/collections\n  method: get\n  operationId: listCaseCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/collections\n  method: post\n  operationId: launchCaseCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v2/collectionsByPath\n  method: post\n  operationId: launchCollectionsByPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/collectionsByTarget\n  method: post\n  operationId: launchCollectionsByTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/collectionsByConfiguration\n  method: post\n  operationId: launchCollectionsByConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/configurations\n  method: get\n  operationId: listConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/configurations\n  method: post\n  operationId: createConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/configurations/{id}\n  method: delete\n  operationId: deleteConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v2/computers\n  method: post\n  operationId: listComputersByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/compConfigurations\n  method: get\n  operationId: listComputerConfigsAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/compConfigurations/{confid}\n  method: get\n  operationId: listComputerConfigsOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/custodians\n  method: get\n  operationId: listCustodians\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/custodians\n  method: post\n  operationId: createCustodian\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/custodians\n  method: delete\n  operationId: deleteCustodian\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/groups\n  method: get\n  operationId: listGroupsAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/group\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/group\n  method: put\n  operationId: modifyGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/group\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/jobs/{id}\n  method: get\n  operationId: jobDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/jobs\n  method: post\n  operationId: listJobsByFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/jobAction/{id}\n  method: post\n  operationId: jobAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/logs\n  method: get\n  operationId: listLogByJob\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/targets\n  method: get\n  operationId: listTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/targets/{id}\n  method: get\n  operationId: listTarget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/targets/{id}\n  method: delete\n  operationId: deleteTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/target\n  method: post\n  operationId: createTarget\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/eccInstalled\n  method: get\n  operationId: eccInstalled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/license\n  method: get\n  operationId: getServerLicense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/systemInfo\n  method: get\n  operationId: getServerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuix/refs/heads/main/agentic-access/nuix-agentic-access.yml
summary_line: 34 operations · 19 acting
tags:
- Forensics
- eDiscovery
- Investigations
- Compliance
- Data Processing
- Legal Technology
- Intelligence
---
