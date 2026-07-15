---
acting_count: 316
action_class_counts:
  acting: 316
  connected: 270
api_specs:
- filename: pulumi-spec.json
  format: json
  label: Pulumi Cloud REST API
  slug: pulumi-cloud
  spec_type: OpenAPI
  url: https://api.pulumi.com/api/openapi/pulumi-spec.json
consequence_counts:
  physical: 29
  read: 270
  safety-critical: 4
  write: 283
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Pulumi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/esc/cloudsetup/{orgName}/oauth/azure/setup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/orgs/{orgName}/cmk/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/orgs/{orgName}/cmk/{keyID}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/preview/insights/{orgName}/insightstrial/deny
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/esc/environments/{orgName}/{projectName}/{envName}/ownership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orgs/{orgName}/agent-pools
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/orgs/{orgName}/agent-pools/{poolId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/orgs/{orgName}/agent-pools/{poolId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orgs/{orgName}/bulk-transfer/stacks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orgs/{orgName}/deployments/pause
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orgs/{orgName}/deployments/resume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/preview/insights/{orgName}/accounts/{accountName}/ownership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/cache
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/cache/url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/drift/schedules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/drift/schedules/{scheduleID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/pause
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/resume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/schedules
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/schedules/{scheduleID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/schedules/{scheduleID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/schedules/{scheduleID}/pause
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/schedules/{scheduleID}/resume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/stacks/{orgName}/{projectName}/{stackName}/deployments/settings
operation_count: 586
overview: 'Pulumi exposes 586 API operations that an AI agent could call, of which 316 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 270 read, 283 write, 29 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pulumi
provider_slug: pulumi
slug: pulumi-agentic-access
source_filename: pulumi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pulumi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 586\n  by_action_class:\n    acting: 316\n    connected: 270\n  by_consequence:\n    write: 283\n    read: 270\n    safety-critical: 4\n    physical: 29\n  human_in_the_loop_required: 4\noperations:\n- path: /api/ai/template\n  method: post\n  operationId: AITemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/capabilities\n  method: get\n  operationId: Capabilities\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/change-gates/{orgName}\n  method: get\n  operationId: ListGates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/change-gates/{orgName}\n  method: post\n  operationId: CreateGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/change-gates/{orgName}/{gateID}\n  method: delete\n  operationId: DeleteGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/change-gates/{orgName}/{gateID}\n  method: get\n  operationId: ReadGate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/change-gates/{orgName}/{gateID}\n  method: put\n  operationId: UpdateGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/change-requests/{orgName}\n  method: get\n  operationId: List_change_requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/change-requests/{orgName}/{changeRequestID}\n  method: get\n  operationId:\
  \ Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/change-requests/{orgName}/{changeRequestID}\n  method: patch\n  operationId: Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/change-requests/{orgName}/{changeRequestID}/apply\n  method: post\n  operationId: Apply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/change-requests/{orgName}/{changeRequestID}/approve\n  method: delete\n  operationId:\
  \ Unapprove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/change-requests/{orgName}/{changeRequestID}/approve\n  method: post\n  operationId: Approve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/change-requests/{orgName}/{changeRequestID}/close\n  method: post\n  operationId: Close\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/change-requests/{orgName}/{changeRequestID}/comments\n  method: post\n  operationId: AddComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/change-requests/{orgName}/{changeRequestID}/events\n  method: get\n  operationId: ListEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/change-requests/{orgName}/{changeRequestID}/submit\n  method: post\n  operationId: Submit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cli/version\n  method: get\n  operationId: Version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations\n  method: get\n  operationId: ListAllVCSIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/azure-devops\n  method: get\n  operationId: ListAzureDevOpsIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/azure-devops\n  method: post\n  operationId: CreateAzureDevOpsSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/azure-devops/access-status\n  method: get\n  operationId: GetAzureDevOpsAccessStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/azure-devops/oauth/complete\n  method: post\n  operationId: CompleteAzureDevOpsOAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/azure-devops/oauth/initiate\n  method: post\n  operationId: InitiateAzureDevOpsOAuth\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/azure-devops/setup/organizations\n  method: get\n  operationId: ListAzureDevOpsOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/azure-devops/setup/organizations/{adoOrgName}/projects\n  method: get\n  operationId: ListAzureDevOpsProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/azure-devops/{integrationId}\n  method: delete\n  operationId: DeleteAzureDevOpsIntegration\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/azure-devops/{integrationId}\n  method: get\n  operationId: GetAzureDevOpsIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/azure-devops/{integrationId}\n  method: patch\n  operationId: UpdateAzureDevOpsIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/bitbucket\n\
  \  method: get\n  operationId: ListBitBucketIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/bitbucket\n  method: post\n  operationId: CreateBitBucketSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/bitbucket/access-status\n  method: get\n  operationId: GetBitBucketAccessStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/bitbucket/{integrationId}\n  method: delete\n  operationId: DeleteBitBucketIntegration\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/bitbucket/{integrationId}\n  method: get\n  operationId: GetBitBucketIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/bitbucket/{integrationId}\n  method: patch\n  operationId: UpdateBitBucketIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/custom\n\
  \  method: get\n  operationId: ListCustomVCSIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/custom\n  method: post\n  operationId: CreateCustomVCSIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/custom/{integrationId}\n  method: delete\n  operationId: DeleteCustomVCSIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/console/orgs/{orgName}/integrations/custom/{integrationId}\n  method: get\n  operationId: GetCustomVCSIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/custom/{integrationId}\n  method: patch\n  operationId: UpdateCustomVCSIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/custom/{integrationId}/repos\n  method: delete\n  operationId: RemoveCustomVCSRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/custom/{integrationId}/repos\n  method: post\n  operationId: AddCustomVCSRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/github\n  method: get\n  operationId: ListGitHubIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/github\n  method: post\n  operationId: StartGitHubSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/github-enterprise\n  method: get\n  operationId: ListGitHubEnterpriseIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/github-enterprise/{integrationId}\n  method: delete\n  operationId: DeleteGitHubEnterpriseIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/github-enterprise/{integrationId}\n  method: get\n  operationId: GetGitHubEnterpriseIntegration\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/github-enterprise/{integrationId}\n  method: patch\n  operationId: UpdateGitHubEnterpriseIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/github/access-status\n  method: get\n  operationId: GetGitHubAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/github/{integrationId}\n  method: delete\n  operationId: DeleteGitHubIntegration\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/github/{integrationId}\n  method: get\n  operationId: GetGitHubIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/github/{integrationId}\n  method: patch\n  operationId: UpdateGitHubIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/gitlab\n  method: get\n  operationId: ListGitLabIntegrations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/gitlab\n  method: post\n  operationId: CreateGitLabSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/gitlab/access-status\n  method: get\n  operationId: GetGitLabAccessStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/gitlab/{integrationId}\n  method: delete\n  operationId: DeleteGitLabIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/gitlab/{integrationId}\n  method: get\n  operationId: GetGitLabIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/gitlab/{integrationId}\n  method: patch\n  operationId: UpdateGitLabIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/orgs/{orgName}/integrations/{provider}/{integrationId}/repos\n  method: get\n  operationId: ListVCSRepos\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/{provider}/{integrationId}/repos/destinations\n  method: get\n  operationId: ListVCSRepoDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/integrations/{provider}/{integrationId}/repos/{repoId}/branches\n  method: get\n  operationId: ListVCSBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/members/{userLogin}/stacks/{projectName}/{stackName}\n  method: get\n  operationId: ListMemberStackPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/console/orgs/{orgName}/stacks/search\n  method: post\n  operationId: SearchStacks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/stacks/{orgName}/{projectName}/{stackName}/overview\n  method: get\n  operationId: GetStackOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/stacks/{orgName}/{projectName}/{stackName}/teams/{teamName}\n  method: patch\n  operationId: UpdateTeamStackPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/console/stacks/{orgName}/{projectName}/{stackName}/updates/latest/summary\n  method: get\n  operationId: UpdateSummaryHandlerLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/console/stacks/{orgName}/{projectName}/{stackName}/updates/{updateID}/summary\n  method: get\n  operationId: UpdateSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deployments/executor\n  method: get\n  operationId: GetPulumiDeployExecutor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deployments/poll\n  method: get\n  operationId: PollDeploymentsQueue\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deployments/{deploymentId}/status\n  method: get\n  operationId: GetDeploymentsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/cloudsetup/{orgName}/aws/setup\n  method: post\n  operationId: AWSSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/cloudsetup/{orgName}/aws/sso/accounts\n  method: get\n  operationId: AWSSSOListAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/cloudsetup/{orgName}/aws/sso/initiate\n\
  \  method: post\n  operationId: AWSSSOInitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/cloudsetup/{orgName}/aws/sso/setup\n  method: post\n  operationId: AWSSSOSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/cloudsetup/{orgName}/oauth/azure/accounts\n  method: get\n  operationId: AzureListAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/cloudsetup/{orgName}/oauth/azure/setup\n\
  \  method: post\n  operationId: AzureSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/esc/cloudsetup/{orgName}/oauth/complete\n  method: post\n  operationId: CompleteOAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/cloudsetup/{orgName}/oauth/gcp/accounts\n  method: get\n  operationId: GCPListAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/cloudsetup/{orgName}/oauth/gcp/setup\n\
  \  method: post\n  operationId: GCPSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/cloudsetup/{orgName}/oauth/initiate\n  method: post\n  operationId: InitiateOAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments\n  method: get\n  operationId: ListEnvironments_esc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/environments/{orgName}\n  method: get\n  operationId: ListOrgEnvironments_esc\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/environments/{orgName}\n  method: post\n  operationId: CreateEnvironment_esc_environments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/restore\n  method: get\n  operationId: ListDeletedEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/environments/{orgName}/restore\n  method: put\n  operationId: RestoreEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/tags\n  method: get\n  operationId: ListAllEnvironmentTags_esc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/environments/{orgName}/yaml/check\n  method: post\n  operationId: CheckYAML_esc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/yaml/open\n  method: post\n  operationId: OpenYAML_esc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/yaml/open/{openSessionID}\n  method: get\n  operationId: ReadAnonymousOpenEnvironment_esc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}\n  method: delete\n  operationId: DeleteEnvironment_esc_environments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}\n  method: get\n  operationId: ReadEnvironment_esc_environments\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}\n  method: head\n  operationId: HeadEnvironment_esc_environments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}\n  method: patch\n  operationId: UpdateEnvironment_esc_environments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}/check\n  method: post\n  operationId: CheckEnvironment_esc_environments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}/clone\n  method: post\n  operationId: CloneEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}/decrypt\n  method: get\n  operationId: DecryptEnvironment_esc_environments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}/decrypt-secrets\n  method: post\n  operationId:\
  \ DecryptEnvironmentSecrets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}/drafts\n  method: post\n  operationId: CreateEnvironmentDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}/drafts/{changeRequestID}\n  method: get\n  operationId: ReadEnvironmentDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /api/esc/environments/{orgName}/{projectName}/{envName}/drafts/{changeRequestID}\n  method: patch\n  operationId: UpdateEnvironmentDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/esc/environments/{orgName}/{projectName}/{envName}/drafts/{changeRequestID}/open\n  method: post\n  operationId: OpenEnvironmentDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \n\n# --- truncated at 32 KB (189 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/pulumi/refs/heads/main/agentic-access/pulumi-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulumi/refs/heads/main/agentic-access/pulumi-agentic-access.yml
summary_line: 586 operations · 316 acting · 4 human-in-the-loop
tags:
- Automation
- Cloud
- DevOps
- Infrastructure as Code
- Multi-Cloud
- Stacks
- Deployments
- Policy
---
