---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 39
api_specs:
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy API Registry (Artifacts) API
  slug: speakeasy-api-registry-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Workspaces API
  slug: speakeasy-api-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Organizations API
  slug: speakeasy-api-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Schema Store API
  slug: speakeasy-api-schema-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Code Samples API
  slug: speakeasy-api-code-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Generation Events API
  slug: speakeasy-api-generation-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Reports API
  slug: speakeasy-api-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy GitHub Automation API
  slug: speakeasy-api-github-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Suggest (OpenAPI AI) API
  slug: speakeasy-api-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Auth API
  slug: speakeasy-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Publishing Tokens API
  slug: speakeasy-api-publishing-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Subscriptions API
  slug: speakeasy-api-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
consequence_counts:
  read: 39
  safety-critical: 3
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Speakeasy Api Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/suggest/openapi
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/suggest/openapi/{namespace_name}/{revision_reference}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/workspace/{workspace_id}/team/{userId}
operation_count: 77
overview: 'Speakeasy exposes 77 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 39 read, 35 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Speakeasy
provider_slug: speakeasy-api
slug: speakeasy-api-agentic-access
source_filename: speakeasy-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/speakeasy-api-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 77\n  by_action_class:\n    connected: 39\n    acting: 38\n  by_consequence:\n    read: 39\n    write: 35\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/auth/validate\n  method: get\n  operationId: validateApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/access_token\n\
  \  method: get\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/code_sample\n  method: get\n  operationId: getCodeSamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/code_sample/preview\n  method: post\n  operationId: generateCodeSamplePreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/code_sample/preview/async\n  method: post\n  operationId: generateCodeSamplePreviewAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/code_sample/preview/async/{jobID}\n  method: get\n  operationId: getCodeSamplePreviewAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/github/setup\n  method: get\n  operationId: getGithubSetupState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/github/check_access\n  method: get\n  operationId: checkGithubAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/github/link\n  method: post\n  operationId: linkGithubAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/github/publishing_prs\n  method: get\n  operationId: githubCheckPublishingPRs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/github/publishing_secrets\n  method: get\n  operationId: githubCheckPublishingSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/github/publishing_secrets\n  method: post\n  operationId: githubStorePublishingSecrets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/github/configure_code_samples\n  method: post\n  operationId: githubConfigureCodeSamples\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/github/configure_mintlify_repo\n  method: post\n  operationId: githubConfigureMintlifyRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/github/configure_target\n  method: post\n  operationId: githubConfigureTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/github/trigger_action\n  method: post\n  operationId: githubTriggerAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/github/action\n  method: get\n  operationId: getGitHubAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations\n  method: get\n  operationId: getOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization\n\
  \  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organization/{organizationID}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization/free_trial\n  method: post\n  operationId: createFreeTrial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organization/usage\n  method: get\n  operationId: getOrganizationUsage\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization/add_ons\n  method: post\n  operationId: createBillingAddOns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organization/add_ons\n  method: get\n  operationId: getBillingAddOns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organization/add_ons/{add_on}\n  method: delete\n  operationId: deleteBillingAddOn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/publishing-tokens\n  method: get\n  operationId: getPublishingToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/publishing-tokens\n  method: post\n  operationId: createPublishingToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/publishing-tokens/{tokenID}\n  method: get\n  operationId: getPublishingTokenByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/publishing-tokens/{tokenID}\n  method: put\n\
  \  operationId: updatePublishingTokenExpiration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/publishing-tokens/{tokenID}\n  method: delete\n  operationId: deletePublishingToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/publishing-tokens/{tokenID}/target\n  method: get\n  operationId: getPublishingTokenTargetByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/publishing-tokens/{tokenID}/metadata\n\
  \  method: get\n  operationId: getPublishingTokenPublicMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspaces\n  method: get\n  operationId: getWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace\n  method: get\n  operationId: getWorkspaceByContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/workspace/{workspace_id}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace/{workspace_id}/details\n  method: post\n  operationId: updateWorkspaceDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspace/{workspace_id}/settings\n  method: get\n  operationId: getWorkspaceSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace/{workspace_id}/settings\n  method: put\n  operationId: updateWorkspaceSettings\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspace/{workspace_id}/events\n  method: get\n  operationId: searchWorkspaceEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace/{workspace_id}/events\n  method: post\n  operationId: postWorkspaceEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspace/{workspace_id}/team\n  method: get\n  operationId: getWorkspaceTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace/{workspace_id}/team/email/{email}\n  method: put\n  operationId: grantUserAccessToWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspace/{workspace_id}/team/{userId}\n  method: delete\n  operationId: revokeUserAccessToWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/workspace/{workspace_id}/tokens\n  method: get\n  operationId: getWorkspaceTokens\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace/{workspace_id}/tokens\n  method: post\n  operationId: createWorkspaceToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspace/{workspace_id}/tokens/{tokenID}\n  method: delete\n  operationId: deleteWorkspaceToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspace/feature_flags\n  method: post\n  operationId: setWorkspaceFeatureFlags\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workspace/{workspace_id}/feature_flags\n  method: get\n  operationId: getWorkspaceFeatureFlags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace/{workspace_id}/events/targets/{target_id}/events\n  method: get\n  operationId: getWorkspaceEventsByTarget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace/access\n  method: get\n  operationId: getWorkspaceAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v1/workspace/events/targets\n  method: get\n  operationId: getWorkspaceTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace/{workspace_id}/events/targets\n  method: get\n  operationId: getWorkspaceTargetsDeprecated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports\n  method: post\n  operationId: uploadReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reports/linting/{documentChecksum}\n  method: get\n  operationId: getLintingReportSignedUrl\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/changes/{documentChecksum}\n  method: get\n  operationId: getChangesReportSignedUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/suggest/openapi\n  method: post\n  operationId: suggestOpenAPI\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/suggest/openapi_from_summary\n  method: post\n  operationId: suggest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/suggest/items\n  method: post\n  operationId: suggestItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/suggest/openapi/{namespace_name}/{revision_reference}\n  method: post\n  operationId: suggestOpenAPIRegistry\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/schema_store\n  method: get\n  operationId: getSchemaStoreItem\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schema_store\n  method: post\n  operationId: createSchemaStoreItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/short_urls\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/preflight\n  method: post\n  operationId: preflight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/namespaces\n  method: get\n  operationId: getNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/artifacts/namespaces/{namespace_name}/archive\n  method: post\n  operationId: archiveNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/namespaces/{namespace_name}/revisions\n  method: get\n  operationId: getRevisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/artifacts/namespaces/{namespace_name}/tags\n  method: get\n  operationId: getTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/artifacts/namespaces/{namespace_name}/tags\n  method: post\n  operationId: postTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/artifacts/namespaces/{namespace_name}/visibility\n  method: post\n  operationId: setVisibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/artifacts/remote_sources\n  method: get\n  operationId: listRemoteSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/artifacts/remote_sources\n  method: post\n  operationId: createRemoteSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/oci/v2/{organization_slug}/{workspace_slug}/{namespace_name}/manifests/{revision_reference}\n  method: get\n  operationId: getManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oci/v2/{organization_slug}/{workspace_slug}/{namespace_name}/blobs/{digest}\n  method: get\n  operationId:\
  \ getBlob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions/{subscriptionID}/{namespaceName}/ignore\n  method: post\n  operationId: ignoreSubscriptionNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions/{subscriptionID}/{namespaceName}/activate\n  method: post\n  operationId: activateSubscriptionNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/agentic-access/speakeasy-api-agentic-access.yml
summary_line: 77 operations · 38 acting · 3 human-in-the-loop
tags:
- API Lifecycle
- SDK Generation
- Client Library
- API Design
- Developer Tools
- OpenAPI
- Code Generation
- Terraform
- MCP
- Developer Experience
---
