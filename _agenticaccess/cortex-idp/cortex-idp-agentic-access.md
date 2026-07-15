---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 22
api_specs:
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Catalog API
  slug: cortex-idp-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Scorecards API
  slug: cortex-idp-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Custom Data API
  slug: cortex-idp-custom-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Initiatives API
  slug: cortex-idp-initiatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Deploys API
  slug: cortex-idp-deploys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
- filename: cortex-idp-openapi.yml
  format: yaml
  label: Cortex Integrations API
  slug: cortex-idp-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/openapi/cortex-idp-openapi.yml
consequence_counts:
  physical: 4
  read: 22
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cortex Idp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /catalog/{tagOrId}/deploys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /catalog/{tagOrId}/deploys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /catalog/{tagOrId}/deploys/{uuid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /catalog/{tagOrId}/deploys/{uuid}
operation_count: 47
overview: 'Cortex exposes 47 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 21 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cortex
provider_slug: cortex-idp
slug: cortex-idp-agentic-access
source_filename: cortex-idp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cortex-idp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 22\n    acting: 25\n  by_consequence:\n    read: 22\n    write: 21\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /catalog\n  method: get\n  operationId: listCatalogEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog\n  method: delete\n  operationId: deleteCatalogEntitiesByType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/descriptors\n  method: get\n  operationId: listEntityDescriptors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{tagOrId}\n  method: get\n  operationId: getCatalogEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{tagOrId}\n  method: delete\n  operationId: deleteCatalogEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/openapi\n  method: get\n  operationId: getEntityDescriptor\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{tagOrId}/archive\n  method: put\n  operationId: archiveEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/unarchive\n  method: put\n  operationId: unarchiveEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/gitops-logs\n  method: get\n  operationId: getGitopsLogs\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-api\n  method: post\n  operationId: upsertEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /open-api\n  method: patch\n  operationId: patchEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/scorecards\n  method: get\n  operationId: getEntityScorecardScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /scorecards\n  method: get\n  operationId: listScorecards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards/descriptor\n  method: post\n  operationId: upsertScorecardDescriptor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scorecards/{tag}\n  method: get\n  operationId: getScorecard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards/{tag}\n  method: delete\n  operationId: deleteScorecard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scorecards/{tag}/descriptor\n  method: get\n  operationId: getScorecardDescriptor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards/{tag}/scores\n  method: get\n  operationId: getScorecardScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards/{tag}/next-steps\n  method: get\n  operationId: getScorecardNextSteps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards/{scorecardTag}/entity/{tagOrId}/badge\n  method: get\n  operationId: getScorecardBadge\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scorecards/{tag}/entity/{entityTag}/scores\n  method: post\n  operationId: submitScorecardScore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scorecards/{tag}/entity/{entityTag}/exemption\n  method: post\n  operationId: requestExemption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-data\n  method: get\n  operationId: getCustomDataAdvanced\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-data\n  method: put\n  operationId: bulkUpsertCustomData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/custom-data\n  method: get\n  operationId: listEntityCustomData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{tagOrId}/custom-data\n  method: post\n  operationId: addEntityCustomData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/custom-data\n  method: delete\n  operationId: deleteEntityCustomData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/custom-data/{key}\n  method: get\n  operationId: getEntityCustomDataByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /initiatives\n  method: get\n  operationId: listInitiatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /initiatives\n  method: post\n  operationId: createInitiative\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /initiatives/{cid}\n  method: get\n  operationId: getInitiative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /initiatives/{cid}\n  method: put\n  operationId: updateInitiative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /initiatives/{cid}\n  method: delete\n  operationId: deleteInitiative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/deploys\n  method: get\n  operationId: listEntityDeploys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{tagOrId}/deploys\n  method: post\n  operationId: addEntityDeploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/deploys\n  method: delete\n  operationId: deleteEntityDeploys\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/deploys/{uuid}\n  method: put\n  operationId: updateEntityDeploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/{tagOrId}/deploys/{uuid}\n  method: delete\n  operationId: deleteEntityDeploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deploys/environments\n  method: get\n  operationId: listDeployEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deploys/search\n  method: get\n  operationId: searchDeploys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /github/configurations\n  method: get\n  operationId: listGithubConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /github/configurations\n  method: delete\n  operationId: deleteGithubConfigurations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /github/default-configuration\n  method: get\n  operationId: getGithubDefaultConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /github/configurations/validate\n  method: post\n  operationId: validateGithubConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /github/configurations/app\n  method: post\n  operationId: addGithubAppConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /github/configurations/app/{alias}\n  method: put\n  operationId: updateGithubAppConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /github/configurations/app/{alias}\n  method: delete\n  operationId: deleteGithubAppConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cortex-idp/refs/heads/main/agentic-access/cortex-idp-agentic-access.yml
summary_line: 47 operations · 25 acting
tags:
- Software Catalog
- Internal Developer Portal
- Service Catalog
- Developer Experience
- IDP
- Scorecards
- Platform Engineering
- Developer Portal
---
