---
acting_count: 68
action_class_counts:
  acting: 68
  connected: 44
api_specs:
- filename: devcycle-management-openapi.json
  format: json
  label: DevCycle Management API
  slug: devcycle-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/openapi/devcycle-management-openapi.json
- filename: devcycle-bucketing-openapi.yaml
  format: yaml
  label: DevCycle Bucketing API
  slug: devcycle-bucketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/openapi/devcycle-bucketing-openapi.yaml
consequence_counts:
  read: 44
  safety-critical: 60
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 60
kind: agentic-access
layout: agentic-access
method: generated
name: Devcycle Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/integrations/dynatrace
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/integrations/dynatrace/{dynatraceEnvironmentId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/integrations/jira/organization/{token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/integrations/jira/project/{token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/integrations/jira/{token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/projects/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/projects/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/projects/{key}/settings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/projects/{key}/settings/protected
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{project}/audiences
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/projects/{project}/audiences/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/projects/{project}/audiences/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{project}/customProperties
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/projects/{project}/customProperties/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/projects/{project}/customProperties/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{project}/environments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{project}/environments/{environment}/sdk-keys
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/projects/{project}/environments/{environment}/sdk-keys/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/projects/{project}/environments/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/projects/{project}/environments/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{project}/features
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{project}/features/multiple
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/projects/{project}/features/{feature}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/projects/{project}/features/{feature}
operation_count: 112
overview: 'DevCycle exposes 112 API operations that an AI agent could call, of which 68 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read, 8 write, and 60 safety-critical.


  60 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DevCycle
provider_slug: devcycle
slug: devcycle-agentic-access
source_filename: devcycle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/devcycle-bucketing-openapi.yaml, openapi/devcycle-management-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 112\n  by_action_class:\n    acting: 68\n    connected: 44\n  by_consequence:\n    write: 8\n    read: 44\n    safety-critical: 60\n  human_in_the_loop_required: 60\noperations:\n- path: /v1/variables/{key}\n  method: post\n  operationId: getVariableByKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/variables\n  method: post\n\
  \  operationId: getVariables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/features\n  method: post\n  operationId: getFeatures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/track\n  method: post\n  operationId: postEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edgedb/{user_id}\n\
  \  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/optInConfig\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/optIns/{user_id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ofrep/v1/evaluate/flags/{key}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ofrep/v1/evaluate/flags\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects\n  method: post\n  operationId: ProjectsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects\n  method: get\n  operationId: ProjectsController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{key}\n  method: get\n  operationId: ProjectsController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{key}\n  method: patch\n  operationId: ProjectsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{key}\n  method: delete\n  operationId: ProjectsController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{key}/settings\n  method: patch\n  operationId: ProjectsController_updateSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{key}/settings/protected\n  method: patch\n  operationId: ProjectsController_updateProtectedSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{key}/staleness\n\
  \  method: get\n  operationId: ProjectsController_getStaleness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/jira/{token}\n  method: delete\n  operationId: JiraIntegrationController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/integrations/jira/organization/{token}\n  method: delete\n  operationId: JiraIntegrationController_removeOrganizationConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/integrations/jira/project/{token}\n  method: delete\n  operationId: JiraIntegrationController_removeProjectConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/environments\n  method: post\n  operationId: EnvironmentsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/environments\n  method:\
  \ get\n  operationId: EnvironmentsController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/environments/{key}\n  method: get\n  operationId: EnvironmentsController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/environments/{key}\n  method: patch\n  operationId: EnvironmentsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/environments/{key}\n  method: delete\n  operationId: EnvironmentsController_remove\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/environments/{environment}/sdk-keys\n  method: post\n  operationId: SdkKeysController_generate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/environments/{environment}/sdk-keys/{key}\n  method: delete\n  operationId: SdkKeysController_invalidate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/audiences\n  method: post\n  operationId: AudiencesController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/audiences\n  method: get\n  operationId: AudiencesController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/audiences/{key}\n  method: get\n  operationId: AudiencesController_findOne\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/audiences/{key}\n  method: patch\n  operationId: AudiencesController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/audiences/{key}\n  method: delete\n  operationId: AudiencesController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/audiences/{key}/usage\n\
  \  method: get\n  operationId: AudiencesController_findUsages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/variables\n  method: post\n  operationId: VariablesController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/variables\n  method: get\n  operationId: VariablesController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/variables/{key}\n  method: get\n  operationId: VariablesController_findOne\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/variables/{key}\n  method: patch\n  operationId: VariablesController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/variables/{key}\n  method: delete\n  operationId: VariablesController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/variables/{key}/status\n\
  \  method: patch\n  operationId: VariablesController_updateStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features\n  method: post\n  operationId: FeaturesController_create_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features\n  method: get\n  operationId: FeaturesController_findAll_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/features/multiple\n  method: post\n  operationId: FeaturesController_createMultiple_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}\n  method: get\n  operationId: FeaturesController_findOne_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/features/{feature}\n  method: patch\n  operationId: FeaturesController_update_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}\n  method: delete\n  operationId: FeaturesController_remove_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/status\n  method: patch\n  operationId: FeaturesController_updateStatus_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/projects/{project}/features/{feature}/static-configuration\n  method: get\n  operationId: FeaturesController_findStaticConfiguration_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/features/{feature}/static-configuration\n  method: patch\n  operationId: FeaturesController_updateStaticConfiguration_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/integrations/jira/issues\n  method: post\n  operationId: FeaturesController_linkIssue_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/integrations/jira/issues\n  method: get\n  operationId: FeaturesController_findAllLinkedIssues_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/features/{feature}/integrations/jira/issues/{issue_id}\n  method: delete\n  operationId: FeaturesController_removeLinkedIssue_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /v1/projects/{project}/features/{feature}/variations\n  method: post\n  operationId: VariationsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/variations\n  method: get\n  operationId: VariationsController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/features/{feature}/variations/{key}\n  method: get\n  operationId: VariationsController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/features/{feature}/variations/{key}\n\
  \  method: patch\n  operationId: VariationsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/configurations\n  method: get\n  operationId: FeatureConfigsController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/features/{feature}/configurations\n  method: patch\n  operationId: FeatureConfigsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/results/total-evaluations\n  method: get\n  operationId: ResultsController_getTotalEvaluationsPerHourByFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/results/evaluations\n  method: get\n  operationId: ResultsController_getEvaluationsPerHourByProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/results/total-evaluations\n  method: get\n  operationId: ResultsController_getTotalEvaluationsPerHourByProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/userProfile/current\n\
  \  method: get\n  operationId: UserProfilesController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/userProfile/current\n  method: patch\n  operationId: UserProfilesController_createOrUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/audit\n  method: get\n  operationId: AuditLogController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/customProperties\n  method: post\n  operationId: CustomPropertiesController_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/customProperties\n  method: get\n  operationId: CustomPropertiesController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/customProperties/{key}\n  method: get\n  operationId: CustomPropertiesController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/customProperties/{key}\n  method: patch\n  operationId: CustomPropertiesController_update\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/customProperties/{key}\n  method: delete\n  operationId: CustomPropertiesController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/metrics\n  method: post\n  operationId: MetricsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/metrics\n  method: get\n  operationId: MetricsController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/metrics/{key}\n  method: get\n  operationId: MetricsController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/metrics/{key}\n  method: patch\n  operationId: MetricsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/projects/{project}/metrics/{key}\n  method: delete\n  operationId: MetricsController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/metrics/{key}/results\n  method: get\n  operationId: MetricsController_fetchResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/test-metric-results\n  method: get\n  operationId: TestMetricResultsController_fetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/metric-associations\n\
  \  method: get\n  operationId: MetricAssociationsController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/metric-associations\n  method: post\n  operationId: MetricAssociationsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/metric-associations\n  method: delete\n  operationId: MetricAssociationsController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/overrides/current\n  method: put\n  operationId: OverridesController_updateFeatureOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/overrides/current\n  method: get\n  operationId: OverridesController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/features/{feature}/overrides/current\n  method: delete\n  operationId: OverridesController_deleteOverridesForFeature\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{project}/features/{feature}/overrides\n  method: get\n  operationId: OverridesController_findOverridesForFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/overrides/current\n  method: get\n  operationId: OverridesController_findOverridesForProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project}/overrides/current\n  method: delete\n  operationId: OverridesController_deleteOverridesForProject\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/semantic/projects/{project}/audiences/{key}\n  method: patch\n  operationId: SemanticPatchController_semanticUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/projects/{project}/features/{feature}\n  method: patch\n  operationId: FeaturesController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n \
  \     purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/projects/{project}/features/{feature}\n  method: get\n  operationId: FeaturesController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{project}/features\n  method: post\n  operationId: FeaturesController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/projects/{project}/features\n  method: get\n  operationId: FeaturesController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{project}/features/{feature}/static-configuration\n  method: get\n  operationId: FeaturesController_findStaticConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{project}/features/{feature}/static-configuration\n  method: patch\n  operationId: FeaturesController_updateStaticConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/projects/{project}/features/{feature}/status\n  method: patch\n  operationId: FeaturesController_updateStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/projects/{project}/features/{feature}/staleness\n  method: get\n  operationId: FeaturesController_getStaleness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{project}/features/{feature}/staleness\n  method: patch\n  operationId: FeaturesController_updateStaleness\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: t\n\n# --- truncated at 32 KB (38 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/agentic-access/devcycle-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devcycle/refs/heads/main/agentic-access/devcycle-agentic-access.yml
summary_line: 112 operations · 68 acting · 60 human-in-the-loop
tags:
- Company
- Enterprise Saas
- Feature Flags
- Feature Management
- Feature Flags as a Service
- Experimentation
- OpenFeature
- Developer Tools
- DevOps
---
