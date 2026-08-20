---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 21
api_specs:
- filename: heroku-account-api-openapi.yml
  format: yaml
  label: Heroku Account API
  slug: heroku-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-account-api-openapi.yml
- filename: heroku-add-ons-api-openapi.yml
  format: yaml
  label: Heroku Add-ons API
  slug: heroku-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-add-ons-api-openapi.yml
- filename: heroku-apps-api-openapi.yml
  format: yaml
  label: Heroku Apps API
  slug: heroku-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-apps-api-openapi.yml
- filename: heroku-builds-api-openapi.yml
  format: yaml
  label: Heroku Builds API
  slug: heroku-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-builds-api-openapi.yml
- filename: heroku-collaborators-api-openapi.yml
  format: yaml
  label: Heroku Collaborators API
  slug: heroku-collaborators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-collaborators-api-openapi.yml
- filename: heroku-config-vars-api-openapi.yml
  format: yaml
  label: Heroku Config Vars API
  slug: heroku-config-vars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-config-vars-api-openapi.yml
- filename: heroku-domains-api-openapi.yml
  format: yaml
  label: Heroku Domains API
  slug: heroku-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-domains-api-openapi.yml
- filename: heroku-dynos-api-openapi.yml
  format: yaml
  label: Heroku Dynos API
  slug: heroku-dynos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-dynos-api-openapi.yml
- filename: heroku-formation-api-openapi.yml
  format: yaml
  label: Heroku Formation API
  slug: heroku-formation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-formation-api-openapi.yml
- filename: heroku-log-sessions-api-openapi.yml
  format: yaml
  label: Heroku Log Sessions API
  slug: heroku-log-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-log-sessions-api-openapi.yml
- filename: heroku-pipelines-api-openapi.yml
  format: yaml
  label: Heroku Pipelines API
  slug: heroku-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-pipelines-api-openapi.yml
- filename: heroku-regions-api-openapi.yml
  format: yaml
  label: Heroku Regions API
  slug: heroku-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-regions-api-openapi.yml
- filename: heroku-releases-api-openapi.yml
  format: yaml
  label: Heroku Releases API
  slug: heroku-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-releases-api-openapi.yml
- filename: heroku-stacks-api-openapi.yml
  format: yaml
  label: Heroku Stacks API
  slug: heroku-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-stacks-api-openapi.yml
consequence_counts:
  read: 21
  safety-critical: 1
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Heroku Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /apps/{app_id_or_name}/dynos/{dyno_id_or_name}/actions/stop
operation_count: 44
overview: 'Heroku exposes 44 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 22 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Heroku
provider_slug: heroku
slug: heroku-agentic-access
source_filename: heroku-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/heroku-platform-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 21\n    acting: 23\n  by_consequence:\n    read: 21\n    write: 22\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}\n  method: patch\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}\n  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /apps/{app_id_or_name}/dynos\n  method: get\n  operationId: listDynos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/dynos\n  method: post\n  operationId: createDyno\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/dynos/{dyno_id_or_name}\n  method: get\n  operationId: getDyno\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/dynos/{dyno_id_or_name}/actions/stop\n  method: post\n  operationId: stopDyno\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /apps/{app_id_or_name}/dynos/actions/restart-all\n  method: post\n  operationId: restartAllDynos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/config-vars\n  method: get\n  operationId: getConfigVars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/config-vars\n  method: patch\n  operationId: updateConfigVars\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/addons\n  method: get\n  operationId: listAddons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/addons\n  method: post\n  operationId: createAddon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/addons/{addon_id_or_name}\n  method: get\n  operationId: getAddon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/addons/{addon_id_or_name}\n  method: delete\n  operationId: deleteAddon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/domains\n  method: post\n  operationId: createDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/domains/{domain_id_or_hostname}\n  method: get\n  operationId: getDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/domains/{domain_id_or_hostname}\n  method: delete\n  operationId: deleteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/formation\n  method: get\n  operationId: listFormation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/formation\n  method: patch\n  operationId: batchUpdateFormation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/formation/{formation_id_or_type}\n  method: patch\n  operationId: updateFormation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/releases\n  method: get\n  operationId: listReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/releases\n  method: post\n  operationId: createRelease\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/releases/{release_id_or_version}\n  method: get\n  operationId: getRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/builds\n  method: get\n  operationId: listBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/builds\n  method: post\n  operationId: createBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/builds/{build_id}\n  method: get\n  operationId: getBuild\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/log-sessions\n  method: post\n  operationId: createLogSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines\n  method: get\n  operationId: listPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines\n  method: post\n  operationId: createPipeline\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipeline_id}\n  method: get\n  operationId: getPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipeline_id}\n  method: patch\n  operationId: updatePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipeline_id}\n  method: delete\n  operationId: deletePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipeline_id}/pipeline-couplings\n  method: get\n  operationId: listPipelineCouplings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipeline-couplings\n  method: post\n  operationId: createPipelineCoupling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /account\n  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /regions\n  method: get\n  operationId: listRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stacks\n  method: get\n  operationId: listStacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id_or_name}/collaborators\n  method: get\n  operationId: listCollaborators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /apps/{app_id_or_name}/collaborators\n  method: post\n  operationId: createCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{app_id_or_name}/collaborators/{collaborator_email_or_id}\n  method: delete\n  operationId: deleteCollaborator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/agentic-access/heroku-agentic-access.yml
summary_line: 44 operations · 23 acting · 1 human-in-the-loop
tags:
- Application Deployment
- Cloud Platform
- DevOps
- Platform-as-a-Service
---
