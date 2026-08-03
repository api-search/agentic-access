---
acting_count: 184
action_class_counts:
  acting: 184
  connected: 182
api_specs:
- filename: visier-administration-apis-openapi.yaml
  format: yaml
  label: Visier Administration APIs
  slug: administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-administration-apis-openapi.yaml
- filename: visier-analytic-model-apis-openapi.yaml
  format: yaml
  label: Visier Analytic Model APIs
  slug: analytic-model
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-analytic-model-apis-openapi.yaml
- filename: visier-authentication-apis-openapi.yaml
  format: yaml
  label: Visier Authentication APIs
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-authentication-apis-openapi.yaml
- filename: visier-data-in-apis-openapi.yaml
  format: yaml
  label: Visier Data In APIs
  slug: data-in
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-data-in-apis-openapi.yaml
- filename: visier-data-out-apis-openapi.yaml
  format: yaml
  label: Visier Data Out APIs
  slug: data-out
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-data-out-apis-openapi.yaml
- filename: visier-webhooks-openapi.yaml
  format: yaml
  label: Visier Webhooks APIs
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-webhooks-openapi.yaml
- filename: visier-planning-openapi.yaml
  format: yaml
  label: Visier Planning Public APIs
  slug: planning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-planning-openapi.yaml
- filename: visier-compensation-benchmarks-openapi.yaml
  format: yaml
  label: Visier Compensation Benchmarks API
  slug: compensation-benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-compensation-benchmarks-openapi.yaml
- filename: visier-skills-intelligence-engine-openapi.yaml
  format: yaml
  label: Visier Skills Intelligence Engine API
  slug: skills-intelligence-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-skills-intelligence-engine-openapi.yaml
consequence_counts:
  physical: 9
  read: 182
  safety-critical: 10
  write: 165
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Visier Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/admin/data-access-sets/revert-to-parent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/admin/permissions/revert-to-parent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/admin/tenants/{tenantId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/admin/user-groups/permissions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/op/data-versions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/skills/extract
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/skills/match
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1alpha/alerts/{alertId}/recipient-status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1alpha/data/export-connectors/connectors/{connectorId}/jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/admin/user-groups/revert-to-parent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/admin/tenants/{tenantId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/compensation-benchmarks/jobs/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/op/data-transfer-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/op/data-transfer-sessions/{transferSessionId}/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/op/data-transfer-sessions/{transferSessionId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/op/data-transfer-sessions/{transferSessionId}/upload
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/op/jobs/receiving-jobs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/op/webhooks/{webhookId}/testEvent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/admin/tenants/{tenantId}
operation_count: 366
overview: 'Visier exposes 366 API operations that an AI agent could call, of which 184 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 182 read, 165 write, 9 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Visier
provider_slug: visier
slug: visier-agentic-access
source_filename: visier-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/visier-administration-apis-openapi.yaml, openapi/visier-analytic-model-apis-openapi.yaml,\n  openapi/visier-authentication-apis-openapi.yaml, openapi/visier-compensation-benchmarks-openapi.yaml,\n  openapi/visier-data-in-apis-openapi.yaml, openapi/visier-data-out-apis-openapi.yaml, openapi/visier-planning-openapi.yaml,\n  openapi/visier-skills-intelligence-engine-openapi.yaml, openapi/visier-webhooks-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 366\n  by_action_class:\n    connected: 182\n    acting: 184\n  by_consequence:\n    read: 182\n    write: 165\n    safety-critical: 10\n    physical: 9\n  human_in_the_loop_required: 10\noperations:\n- path: /v1/admin/capabilities\n\
  \  method: get\n  operationId: Permissions_GetCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/capabilities/{capabilityId}\n  method: get\n  operationId: Permissions_GetCapability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/content-packages\n  method: get\n  operationId: Permissions_GetContentPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/content-packages/{contentPackageId}\n  method: get\n  operationId: Permissions_GetContentPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/data-access-sets\n \
  \ method: get\n  operationId: Permissions_GetDataAccessSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/data-access-sets\n  method: put\n  operationId: Permissions_UpdateDataAccessSets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/data-access-sets\n  method: post\n  operationId: Permissions_CreateDataAccessSets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/data-access-sets\n \
  \ method: delete\n  operationId: Permissions_DeleteDataAccessSets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/data-access-sets/revert-to-parent\n  method: post\n  operationId: Permissions_RevertDataAccessSetsToParent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/admin/data-access-sets/{dataAccessSetId}\n  method: get\n  operationId: Permissions_GetDataAccessSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/admin/data-security-objects\n  method: get\n  operationId: Permissions_GetDataSecurityObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/permissions\n  method: get\n  operationId: Permissions_GetPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/permissions\n  method: put\n  operationId: Permissions_UpdatePermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/permissions\n  method: post\n  operationId: Permissions_CreatePermissions\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/permissions\n  method: delete\n  operationId: Permissions_DeletePermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/permissions/revert-to-parent\n  method: post\n  operationId: Permissions_RevertPermissionsToParent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v1/admin/permissions/users\n  method: put\n  operationId: UsersV1_AssignPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/permissions/users\n  method: delete\n  operationId: UsersV1_RemovePermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/permissions/{permissionId}\n  method: get\n  operationId: Permissions_GetPermission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/permissions/{permissionId}/users\n  method: get\n  operationId: UsersV1_GetPermissionAssignedUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/production-versions\n  method: get\n  operationId: ProductionVersions_GetProductionVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/production-versions\n  method: post\n  operationId: ProductionVersions_PostProductionVersions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/production-versions/{productionVersionId}\n\
  \  method: post\n  operationId: ProductionVersions_PostProductionVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/profiles\n  method: get\n  operationId: Profiles_GetAllProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/profiles/accessible-tenants\n  method: get\n  operationId: Profiles_GetAnalyticProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/profiles/accessible-tenants/{profileId}\n  method: get\n  operationId: Profiles_GetAnalyticProfileDetail\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/profiles/accessible-tenants/{profileId}/assign\n  method: put\n  operationId: Profiles_AssignAnalyticProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/profiles/accessible-tenants/{profileId}/remove\n  method: delete\n  operationId: Profiles_RemoveAnalyticProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/profiles/{profileId}\n  method: get\n  operationId: Profiles_GetProfileDetail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/profiles/{profileId}/assign\n  method: put\n  operationId: Profiles_AssignProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/profiles/{profileId}/remove\n  method: delete\n  operationId: Profiles_RemoveProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/projects\n  method: get\n  operationId: Projects_GetProjects\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/projects\n  method: post\n  operationId: Projects_CreateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/projects/{projectId}\n  method: get\n  operationId: Projects_GetProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/projects/{projectId}\n  method: post\n  operationId: Projects_RunProjectOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/projects/{projectId}\n  method: delete\n  operationId: Projects_DeleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/projects/{projectId}/commits\n  method: get\n  operationId: Projects_GetProjectCommits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/projects/{projectId}/commits\n  method: put\n  operationId: Projects_PutProjectCommits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/security-artifacts/sync-to-non-versioned\n  method: post\n  operationId: Permissions_SyncToNonVersioned\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/system-status\n  method: get\n  operationId: SystemStatus_SystemStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/system-status\n  method: post\n  operationId: SystemStatus_PostSystemStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/tenants\n  method: get\n  operationId: TenantsV1_GetTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/tenants\n  method: post\n  operationId: TenantsV1_AddTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/tenants/batch\n  method: post\n  operationId: TenantsV1_AddTenants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /v1/admin/tenants/{tenantId}\n  method: get\n  operationId: TenantsV1_GetTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/tenants/{tenantId}\n  method: put\n  operationId: TenantsV1_UpdateTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/tenants/{tenantId}\n  method: delete\n  operationId: TenantsV1_DeleteTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/tenants/{tenantId}/disable\n  method: put\n  operationId: TenantsV1_DisableTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/admin/tenants/{tenantId}/enable\n  method: put\n  operationId: TenantsV1_EnableTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/user-groups\n  method: get\n  operationId: UsersV1_GetAllUserGroups\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/user-groups/permissions\n  method: put\n  operationId: UsersV1_AssignPermissionsToUserGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/user-groups/permissions\n  method: delete\n  operationId: UsersV1_RevokePermissionsFromUserGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/admin/user-groups/users\n  method: put\n  operationId: UsersV1_AddUsersToUserGroup\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/user-groups/users\n  method: delete\n  operationId: UsersV1_RemoveUsersFromUserGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/user-groups/{userGroupId}/users\n  method: get\n  operationId: UsersV1_GetUserGroupUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/users\n  method: get\n  operationId: UsersV1_GetAllUsers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/users\n  method: post\n  operationId: UsersV1_AddUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/users/{userId}\n  method: get\n  operationId: UsersV1_GetUserDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/users/{userId}\n  method: put\n  operationId: UsersV1_UpdateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/users/{userId}\n  method: delete\n  operationId: UsersV1_DeleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/users/{userId}/accessible-tenant-profiles\n  method: get\n  operationId: Profiles_GetAnalyticUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/users/{userId}/profiles\n  method: get\n  operationId: Profiles_GetUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/vee/instructions\n  method: get\n  operationId: VeeConfiguration_GetVeeInstructions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/vee/instructions\n  method: post\n  operationId: VeeConfiguration_CreateVeeInstruction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/vee/instructions/{instructionId}\n  method: get\n  operationId: VeeConfiguration_GetVeeInstruction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/vee/instructions/{instructionId}\n  method: put\n  operationId: VeeConfiguration_UpdateVeeInstruction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/vee/instructions/{instructionId}\n  method: delete\n  operationId: VeeConfiguration_DeleteVeeInstruction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/vee/safeguards\n  method: get\n  operationId: VeeConfiguration_GetVeeSafeguards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/vee/safeguards\n  method: post\n  operationId: VeeConfiguration_CreateVeeSafeguard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/vee/safeguards/{safeguardId}\n  method: get\n  operationId: VeeConfiguration_GetVeeSafeguard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/vee/safeguards/{safeguardId}\n  method: put\n  operationId: VeeConfiguration_UpdateVeeSafeguard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/vee/safeguards/{safeguardId}\n  method: delete\n  operationId: VeeConfiguration_DeleteVeeSafeguard\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/op/validation/tenants\n  method: get\n  operationId: TenantsV1_ValidateTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/op/validation/tenants/{tenantId}\n  method: get\n  operationId: TenantsV1_ValidateTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/api-network-subnets\n  method: get\n  operationId: NetworkSubnets_GetApiSubnets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/api-network-subnets\n\
  \  method: put\n  operationId: NetworkSubnets_SetApiSubnets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/api-network-subnets\n  method: post\n  operationId: NetworkSubnets_AddApiSubnets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/api-network-subnets\n  method: delete\n  operationId: NetworkSubnets_DeleteApiSubnets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/consolidated-analytics/tenants\n  method: get\n  operationId: ConsolidatedAnalytics_ListTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/consolidated-analytics/tenants\n  method: post\n  operationId: ConsolidatedAnalytics_CreateTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/consolidated-analytics/tenants-with-details\n  method: get\n  operationId: ConsolidatedAnalytics_ListTenantsWithDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/consolidated-analytics/tenants/{tenantId}/excluded-sources\n  method: get\n  operationId: ConsolidatedAnalytics_ListExcludedSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/consolidated-analytics/tenants/{tenantId}/excluded-sources\n  method: put\n  operationId: ConsolidatedAnalytics_SetExcludedSources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/consolidated-analytics/tenants/{tenantId}/excluded-sources\n  method: delete\n  operationId: ConsolidatedAnalytics_RemoveExcludedSources\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/consolidated-analytics/tenants/{tenantId}/excluded-sources\n  method: patch\n  operationId: ConsolidatedAnalytics_AddExcludedSources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/consolidated-analytics/tenants/{tenantId}/source-tenants\n  method: get\n  operationId: ConsolidatedAnalytics_ListSourceTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/consolidated-analytics/tenants/{tenantId}/source-tenants\n\
  \  method: put\n  operationId: ConsolidatedAnalytics_SetSourceTenants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/consolidated-analytics/tenants/{tenantId}/source-tenants\n  method: delete\n  operationId: ConsolidatedAnalytics_RemoveSourceTenants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/consolidated-analytics/tenants/{tenantId}/source-tenants\n  method: patch\n  operationId: ConsolidatedAnalytics_AddSourceTenants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/email-domains\n  method: get\n  operationId: EmailDomains_ListAllowedEmailDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/email-domains\n  method: put\n  operationId: EmailDomains_AddAllowedEmailDomains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/email-domains\n  method: delete\n  operationId: EmailDomains_DeleteAllowedEmailDomains\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/encryption-keys\n  method: get\n  operationId: EncryptionKeys_ListAllEncryptionKeysMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/encryption-keys\n  method: post\n  operationId: EncryptionKeys_GenerateEncryptionKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/encryption-keys/{keyName}\n  method: delete\n  operationId: EncryptionKeys_DeleteEncryptionKeys\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/product/releases\n  method: get\n  operationId: ReleaseVersionConfiguration_GetAvailableReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/product/versions\n  method: get\n  operationId: ReleaseVersionConfiguration_GetReleaseVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/product/versions\n  method: patch\n  operationId: ReleaseVersionConfiguration_SetReleaseVersions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha/admin/sidecar-app-configs/{applicationId}\n  method: get\n  operationId: SidecarSolutions_GetSidecarSolutionSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha/admin/sidecar-app-configs/{applicationId}\n  method: put\n  operationId: SidecarSolutions_SetSidecarAppConfigs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: \n\n# --- truncated at 32 KB (111 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/agentic-access/visier-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/agentic-access/visier-agentic-access.yml
summary_line: 366 operations · 184 acting · 10 human-in-the-loop
tags:
- Company
- People Analytics
- Workforce Analytics
- Human Resources
- HR Technology
- Workforce Planning
- Analytics
- Business Intelligence
- Compensation
- Skills
- Artificial Intelligence
- Model Context Protocol
---
