---
acting_count: 350
action_class_counts:
  acting: 350
  connected: 476
api_specs:
- filename: nuon-oapi-v3-openapi.json
  format: json
  label: Nuon Control Plane API
  slug: nuon-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-oapi-v3-openapi.json
consequence_counts:
  physical: 20
  read: 476
  safety-critical: 16
  write: 314
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 16
kind: agentic-access
layout: agentic-access
method: generated
name: Nuon Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/account/user-journeys/{journey_name}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/account/user-journeys/{journey_name}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/orgs/current/invites/{invite_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/orgs/current/invites/{invite_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/orgs/{org_id}/slack/org-links/{link_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/orgs/{org_id}/slack/org-links/{link_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/force-shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/force-shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/graceful-shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/graceful-shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/mng/shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/mng/shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/mng/shutdown-vm
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/mng/shutdown-vm
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/processes/{process_id}/shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runners/{runner_id}/processes/{process_id}/shutdown
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/installs/{install_id}/components/deploy-all
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/installs/{install_id}/components/deploy-all
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/installs/{install_id}/components/{component_id}/deploys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/installs/{install_id}/components/{component_id}/deploys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/installs/{install_id}/deploys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/installs/{install_id}/deploys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/installs/{install_id}/deprovision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/installs/{install_id}/deprovision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/installs/{install_id}/deprovision-sandbox
operation_count: 826
overview: 'Nuon exposes 826 API operations that an AI agent could call, of which 350 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 476 read, 314 write, 20 physical, and 16 safety-critical.


  16 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nuon
provider_slug: nuon
slug: nuon-agentic-access
source_filename: nuon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/nuon-oapi-v2-openapi.json, openapi/nuon-oapi-v3-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 826\n  by_action_class:\n    acting: 350\n    connected: 476\n  by_consequence:\n    write: 314\n    read: 476\n    safety-critical: 16\n    physical: 20\n  human_in_the_loop_required: 16\noperations:\n- path: /slack/commands/nuon\n  method: post\n  operationId: SlackSlashCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /slack/events\n\
  \  method: post\n  operationId: SlackEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /slack/interactions\n  method: post\n  operationId: SlackInteractions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /slack/oauth/callback\n  method: get\n  operationId: SlackOAuthCallback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: GetCurrentAccount\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/static-token\n  method: post\n  operationId: CreateStaticToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/static-tokens\n  method: get\n  operationId: ListStaticTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/static-tokens/{token_id}\n  method: delete\n  operationId: DeleteStaticToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/user-journeys\n  method: get\n  operationId: GetUserJourneys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/user-journeys\n  method: post\n  operationId: CreateUserJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/user-journeys/{journey_name}/complete\n  method: post\n  operationId: CompleteUserJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/user-journeys/{journey_name}/reset\n  method: post\n  operationId: ResetUserJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/account/user-journeys/{journey_name}/steps/{step_name}\n  method: patch\n  operationId: UpdateUserJourneyStep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/action-workflows/configs/{action_workflow_config_id}\n  method: get\n  operationId: GetActionWorkflowConfig\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/action-workflows/{action_workflow_id}\n  method: delete\n  operationId: DeleteActionWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/action-workflows/{action_workflow_id}\n  method: get\n  operationId: GetActionWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/action-workflows/{action_workflow_id}\n  method: patch\n  operationId: UpdateAppActionWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/action-workflows/{action_workflow_id}/configs\n  method: get\n  operationId: GetActionWorkflowConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/action-workflows/{action_workflow_id}/configs\n  method: post\n  operationId: CreateActionWorkflowConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/action-workflows/{action_workflow_id}/latest-config\n  method: get\n  operationId: GetActionWorkflowLatestConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps\n  method: get\n  operationId: GetApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps\n  method: post\n  operationId: CreateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}\n  method: delete\n  operationId: DeleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}\n  method: get\n  operationId:\
  \ GetApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}\n  method: patch\n  operationId: UpdateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/action-workflows\n  method: get\n  operationId: GetActionWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/action-workflows\n  method: post\n  operationId: CreateAppActionWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/action-workflows/{action_workflow_id}\n  method: get\n  operationId: GetAppActionWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/actions\n  method: get\n  operationId: GetAppActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/actions\n  method: post\n  operationId: CreateAppAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/actions/configs/{action_config_id}\n\
  \  method: get\n  operationId: GetAppActionConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/actions/label-keys\n  method: get\n  operationId: GetActionLabelKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/actions/{action_id}\n  method: delete\n  operationId: DeleteAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/actions/{action_id}\n  method: get\n  operationId: GetAppAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/actions/{action_id}\n  method: patch\n  operationId: UpdateAppAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/actions/{action_id}/configs\n  method: get\n  operationId: GetAppActionConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/actions/{action_id}/configs\n  method: post\n  operationId: CreateActionConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/actions/{action_id}/labels\n  method: delete\n  operationId: RemoveAppActionLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/actions/{action_id}/labels\n  method: post\n  operationId: AddAppActionLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/actions/{action_id}/latest-config\n  method: get\n  operationId: GetActionLatestConfig\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/branches\n  method: get\n  operationId: GetAppBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/branches\n  method: post\n  operationId: CreateAppBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/branches/{app_branch_id}\n  method: delete\n  operationId: DeleteAppBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/branches/{app_branch_id}\n  method: get\n  operationId: GetAppBranch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/branches/{app_branch_id}\n  method: patch\n  operationId: UpdateAppBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/branches/{app_branch_id}/configs\n  method: get\n  operationId: GetAppBranchAppConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/branches/{app_branch_id}/configs\n  method: post\n \
  \ operationId: CreateAppBranchConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/branches/{app_branch_id}/latest-config\n  method: get\n  operationId: GetAppBranchLatestConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/branches/{app_branch_id}/runs\n  method: get\n  operationId: GetAppBranchRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/branches/{app_branch_id}/runs\n  method: post\n  operationId: TriggerAppBranchRun\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/branches/{app_branch_id}/runs/{run_id}/builds\n  method: get\n  operationId: GetAppBranchRunBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/branches/{app_branch_id}/runs/{run_id}/install-group-runs\n  method: get\n  operationId: GetInstallGroupRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/branches/{app_branch_id}/runs/{run_id}/install-group-runs/{install_group_run_id}\n  method: get\n  operationId: GetInstallGroupRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/branches/{app_branch_id}/runs/{run_id}/install-groups\n  method: get\n  operationId: GetAppBranchRunInstallGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/break-glass-configs\n  method: post\n  operationId: CreateAppBreakGlassConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/break-glass-configs/{config_id}\n  method: get\n  operationId: GetAppBreakGlassConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/apps/{app_id}/component/{component_name_or_id}\n  method: get\n  operationId: GetAppComponent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components\n  method: get\n  operationId: GetAppComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components\n  method: post\n  operationId: CreateComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/build-all\n  method: post\n  operationId: BuildAllComponents\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/label-keys\n  method: get\n  operationId: GetComponentLabelKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components/{component_id}\n  method: delete\n  operationId: DeleteAppComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}\n  method: patch\n  operationId: UpdateAppComponent\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/builds\n  method: get\n  operationId: GetAppComponentBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components/{component_id}/builds\n  method: post\n  operationId: CreateAppComponentBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/builds/latest\n  method: get\n  operationId: GetAppComponentLatestBuild\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components/{component_id}/builds/{build_id}\n  method: get\n  operationId: GetAppComponentBuild\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components/{component_id}/builds/{build_id}/cancel\n  method: post\n  operationId: CancelAppComponentBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/configs\n  method: get\n  operationId: GetAppComponentConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components/{component_id}/configs/docker-build\n  method: post\n  operationId: CreateAppDockerBuildComponentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/configs/external-image\n  method: post\n  operationId: CreateAppExternalImageComponentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/configs/helm\n  method: post\n\
  \  operationId: CreateAppHelmComponentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/configs/job\n  method: post\n  operationId: CreateAppJobComponentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/configs/kubernetes-manifest\n  method: post\n  operationId: CreateAppKubernetesManifestComponentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/configs/latest\n  method: get\n  operationId: GetAppComponentLatestConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components/{component_id}/configs/pulumi\n  method: post\n  operationId: CreateAppPulumiComponentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/configs/terraform-module\n  method: post\n  operationId: CreateAppTerraformModuleComponentConfig\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/configs/{config_id}\n  method: get\n  operationId: GetAppComponentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components/{component_id}/dependencies\n  method: get\n  operationId: GetAppComponentDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components/{component_id}/dependents\n  method: get\n  operationId: GetAppComponentDependents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/components/{component_id}/labels\n  method: delete\n  operationId: RemoveAppComponentLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/components/{component_id}/labels\n  method: post\n  operationId: AddAppComponentLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/config\n  method: post\n  operationId: CreateAppConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/config/{app_config_id}\n  method: get\n  operationId: GetAppConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/config/{app_config_id}\n  method: patch\n  operationId: UpdateAppConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/config/{app_config_id}/graph\n  method: get\n  operationId: GetAppConfigGraph\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/config/{app_config_id}/update-installs\n  method: post\n  operationId: UpdateAppConfigInstalls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/configs\n  method: get\n  operationId: GetAppConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/configs\n  method: post\n  operationId: CreateAppConfigV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/configs/{config_id}\n  method: get\n  operationId: GetAppConflgV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/configs/{config_id}\n  method: patch\n  operationId: UpdateAppConflgV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/configs/{config_id}/build\n  method: post\n  operationId: BuildAppConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/configs/{config_id}/diff\n  method: get\n  operationId: GetAppConfigDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/configs/{config_id}/graph\n  method: get\n  operationId: GetAppConfigGraphV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/configs/{config_id}/update-installs\n  method: post\n  operationId: UpdateAppConfigInstallsV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/input-config\n  method: post\n\
  \  operationId: CreateAppInputConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/input-configs\n  method: get\n  operationId: GetAppInputConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/input-configs/{input_config_id}\n  method: get\n  operationId: GetAppInputConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/input-latest-config\n  method: get\n  operationId: GetAppInputLatestConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/installs\n  method: get\n  operationId: GetAppInstalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/installs\n  method: post\n  operationId: CreateInstall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/{app_id}/kubernetes-contexts-configs\n  method: post\n  operationId: CreateAppKubernetesContextsConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /v1/apps/{app_id}/labels\n  method: get\n  operationId: GetAppLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/latest-break-glass-config\n  method: get\n  operationId: GetLatestAppBreakGlassConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/latest-config\n  method: get\n  operationId: GetAppLatestConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{app_id}/latest-permissions-config\n  method: get\n  operationId: GetLatestAppPermissionsConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/apps/{app_id}/latest-poli\n\n# --- truncated at 32 KB (237 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/agentic-access/nuon-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/agentic-access/nuon-agentic-access.yml
summary_line: 826 operations · 350 acting · 16 human-in-the-loop
tags:
- Company
- BYOC
- Deployment
- Continuous Delivery
- DevOps
- Infrastructure
- Cloud
- Multi-Cloud
- Kubernetes
- Terraform
- Platform Engineering
---
