---
acting_count: 98
action_class_counts:
  acting: 98
  connected: 74
api_specs:
- filename: open-api-spec.yaml
  format: yaml
  label: WorkOS API
  slug: workos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/workos/openapi-spec/main/spec/open-api-spec.yaml
consequence_counts:
  read: 74
  safety-critical: 98
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 98
kind: agentic-access
layout: agentic-access
method: generated
name: Workos Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api_keys/validations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api_keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /audit_logs/actions/{actionName}/schemas
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /audit_logs/events
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /audit_logs/exports
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/challenges/{id}/verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/factors/enroll
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /auth/factors/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/factors/{id}/challenge
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /authkit/oauth2/complete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /authorization/organization_memberships/{organization_membership_id}/check
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /authorization/organization_memberships/{organization_membership_id}/role_assignments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /authorization/organization_memberships/{organization_membership_id}/role_assignments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /authorization/organization_memberships/{organization_membership_id}/role_assignments/{role_assignment_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /authorization/organizations/{organizationId}/roles
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /authorization/organizations/{organizationId}/roles/{slug}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /authorization/organizations/{organizationId}/roles/{slug}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /authorization/organizations/{organizationId}/roles/{slug}/permissions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /authorization/organizations/{organizationId}/roles/{slug}/permissions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /authorization/organizations/{organizationId}/roles/{slug}/permissions/{permissionSlug}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /authorization/organizations/{organization_id}/resources/{resource_type_slug}/{external_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /authorization/organizations/{organization_id}/resources/{resource_type_slug}/{external_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /authorization/permissions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /authorization/permissions/{slug}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /authorization/permissions/{slug}
operation_count: 172
overview: 'WorkOS exposes 172 API operations that an AI agent could call, of which 98 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 74 read and 98 safety-critical.


  98 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WorkOS
provider_slug: workos
slug: workos-agentic-access
source_filename: workos-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/workos-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 172\n  by_action_class:\n    acting: 98\n    connected: 74\n  by_consequence:\n    safety-critical: 98\n    read: 74\n  human_in_the_loop_required: 98\noperations:\n- path: /api_keys/validations\n  method: post\n  operationId: ApiKeysController_validateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api_keys/{id}\n  method: delete\n  operationId:\
  \ ApiKeysController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /audit_logs/actions\n  method: get\n  operationId: AuditLogValidatorsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit_logs/actions/{actionName}/schemas\n  method: post\n  operationId: AuditLogValidatorVersionsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /audit_logs/actions/{actionName}/schemas\n  method: get\n  operationId: AuditLogValidatorVersionsController_schemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit_logs/events\n  method: post\n  operationId: AuditLogEventsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /audit_logs/exports\n  method: post\n  operationId: AuditLogExportsController_exports\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /audit_logs/exports/{auditLogExportId}\n  method: get\n  operationId: AuditLogExportsController_export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/challenges/{id}/verify\n  method: post\n  operationId: AuthenticationChallengesController_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/factors/enroll\n  method: post\n  operationId: AuthenticationFactorsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/factors/{id}\n  method: get\n  operationId: AuthenticationFactorsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/factors/{id}\n  method: delete\n  operationId: AuthenticationFactorsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/factors/{id}/challenge\n  method: post\n  operationId: AuthenticationFactorsController_challenge\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authkit/oauth2/complete\n  method: post\n  operationId: ExternalAuthController_completeLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organization_memberships/{organization_membership_id}/check\n  method: post\n  operationId: AuthorizationController_check\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organization_memberships/{organization_membership_id}/resources\n  method: get\n  operationId: AuthorizationController_listResourcesForMembership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/organization_memberships/{organization_membership_id}/resources/{resource_id}/permissions\n  method: get\n  operationId: AuthorizationController_listEffectivePermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/organization_memberships/{organization_membership_id}/resources/{resource_type_slug}/{external_id}/permissions\n  method: get\n  operationId: AuthorizationController_listEffectivePermissionsByExternalId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/organization_memberships/{organization_membership_id}/role_assignments\n  method: get\n  operationId: AuthorizationRoleAssignmentsController_listRoleAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/organization_memberships/{organization_membership_id}/role_assignments\n  method: post\n  operationId: AuthorizationRoleAssignmentsController_assignRole\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organization_memberships/{organization_membership_id}/role_assignments\n\
  \  method: delete\n  operationId: AuthorizationRoleAssignmentsController_removeRoleByCriteria\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organization_memberships/{organization_membership_id}/role_assignments/{role_assignment_id}\n  method: delete\n  operationId: AuthorizationRoleAssignmentsController_removeRoleById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organizations/{organizationId}/roles\n  method: post\n\
  \  operationId: AuthorizationOrganizationRolesController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organizations/{organizationId}/roles\n  method: get\n  operationId: AuthorizationOrganizationRolesController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/organizations/{organizationId}/roles/{slug}\n  method: get\n  operationId: AuthorizationOrganizationRolesController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/organizations/{organizationId}/roles/{slug}\n\
  \  method: patch\n  operationId: AuthorizationOrganizationRolesController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organizations/{organizationId}/roles/{slug}\n  method: delete\n  operationId: AuthorizationOrganizationRolesController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organizations/{organizationId}/roles/{slug}/permissions\n  method: put\n  operationId: AuthorizationOrganizationRolePermissionsController_setPermissions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organizations/{organizationId}/roles/{slug}/permissions\n  method: post\n  operationId: AuthorizationOrganizationRolePermissionsController_addPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organizations/{organizationId}/roles/{slug}/permissions/{permissionSlug}\n  method: delete\n  operationId: AuthorizationOrganizationRolePermissionsController_removePermission\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organizations/{organization_id}/resources/{resource_type_slug}/{external_id}\n  method: get\n  operationId: AuthorizationResourcesByExternalIdController_getByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/organizations/{organization_id}/resources/{resource_type_slug}/{external_id}\n  method: patch\n  operationId: AuthorizationResourcesByExternalIdController_updateByExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organizations/{organization_id}/resources/{resource_type_slug}/{external_id}\n  method: delete\n  operationId: AuthorizationResourcesByExternalIdController_deleteByExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/organizations/{organization_id}/resources/{resource_type_slug}/{external_id}/organization_memberships\n  method: get\n  operationId: AuthorizationResourcesByExternalIdController_listOrganizationMembershipsForResourceByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/organizations/{organization_id}/resources/{resource_type_slug}/{external_id}/role_assignments\n  method: get\n  operationId: AuthorizationRoleAssignmentsController_listRoleAssignmentsForResourceByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/permissions\n  method: get\n  operationId: AuthorizationPermissionsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/permissions\n  method: post\n  operationId: AuthorizationPermissionsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/permissions/{slug}\n  method: get\n  operationId: AuthorizationPermissionsController_find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/permissions/{slug}\n  method: patch\n  operationId: AuthorizationPermissionsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/permissions/{slug}\n  method: delete\n  operationId: AuthorizationPermissionsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/resources\n  method: get\n  operationId: AuthorizationResourcesController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/resources\n  method: post\n  operationId: AuthorizationResourcesController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/resources/{resource_id}\n  method: get\n  operationId: AuthorizationResourcesController_findById\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/resources/{resource_id}\n  method: patch\n  operationId: AuthorizationResourcesController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/resources/{resource_id}\n  method: delete\n  operationId: AuthorizationResourcesController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n  \
  \  audit: required\n- path: /authorization/resources/{resource_id}/organization_memberships\n  method: get\n  operationId: AuthorizationResourcesController_listOrganizationMembershipsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/resources/{resource_id}/role_assignments\n  method: get\n  operationId: AuthorizationRoleAssignmentsController_listRoleAssignmentsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/roles\n  method: post\n  operationId: AuthorizationRolesController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /authorization/roles\n  method: get\n  operationId: AuthorizationRolesController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/roles/{slug}\n  method: get\n  operationId: AuthorizationRolesController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorization/roles/{slug}\n  method: patch\n  operationId: AuthorizationRolesController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/roles/{slug}/permissions\n\
  \  method: put\n  operationId: AuthorizationRolePermissionsController_setPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authorization/roles/{slug}/permissions\n  method: post\n  operationId: AuthorizationRolePermissionsController_addPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /connect/applications\n  method: get\n  operationId: ApplicationsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect/applications\n  method: post\n  operationId: ApplicationsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /connect/applications/{id}\n  method: get\n  operationId: ApplicationsController_find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect/applications/{id}\n  method: put\n  operationId: ApplicationsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /connect/applications/{id}\n  method: delete\n  operationId: ApplicationsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /connect/applications/{id}/client_secrets\n  method: get\n  operationId: ApplicationCredentialsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect/applications/{id}/client_secrets\n  method: post\n  operationId: ApplicationCredentialsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /connect/client_secrets/{id}\n  method: delete\n  operationId: ApplicationCredentialsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /connections\n  method: get\n  operationId: ConnectionsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{id}\n  method: get\n  operationId: ConnectionsController_find\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{id}\n  method: delete\n  operationId: ConnectionsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /data-integrations/{slug}/authorize\n  method: post\n  operationId: DataIntegrationsController_getDataIntegrationAuthorizeUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /data-integrations/{slug}/token\n\
  \  method: post\n  operationId: DataIntegrationsController_getUserlandUserToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /directories\n  method: get\n  operationId: DirectoriesController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directories/{id}\n  method: get\n  operationId: DirectoriesController_find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directories/{id}\n  method: delete\n  operationId: DirectoriesController_deleteDirectory\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /directory_groups\n  method: get\n  operationId: DirectoryGroupsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory_groups/{id}\n  method: get\n  operationId: DirectoryGroupsController_find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory_users\n  method: get\n  operationId: DirectoryUsersController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory_users/{id}\n\
  \  method: get\n  operationId: DirectoryUsersController_find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: EventsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feature-flags\n  method: get\n  operationId: FeatureFlagsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feature-flags/{slug}\n  method: get\n  operationId: FeatureFlagsController_findBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feature-flags/{slug}/disable\n  method: put\n  operationId: FeatureFlagsController_disableFlag\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /feature-flags/{slug}/enable\n  method: put\n  operationId: FeatureFlagsController_enableFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /feature-flags/{slug}/targets/{resourceId}\n  method: post\n  operationId: FlagTargetsController_createTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /feature-flags/{slug}/targets/{resourceId}\n  method: delete\n  operationId: FlagTargetsController_deleteTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organization_domains\n  method: post\n  operationId: OrganizationDomainsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /organization_domains/{id}\n  method: get\n  operationId: OrganizationDomainsController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization_domains/{id}\n  method: delete\n  operationId: OrganizationDomainsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organization_domains/{id}/verify\n  method: post\n  operationId: OrganizationDomainsController_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organizations\n  method: get\n  operationId: OrganizationsController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: post\n  operationId: OrganizationsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organizations/external_id/{external_id}\n  method: get\n  operationId: OrganizationsController_getByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /organizations/{id}\n  method: get\n  operationId: OrganizationsController_find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}\n  method: put\n  operationId: OrganizationsController_updateOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organizations/{id}\n  method: delete\n  operationId: OrganizationsController_deleteOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organizations/{id}/audit_log_configuration\n  method: get\n  operationId: OrganizationsController_getAuditLogConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/audit_logs_retention\n  method: get\n  operationId: AuditLogsRetentionController_auditLogsRetention\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/audit_logs_retention\n  method: put\n  operationId: AuditLogsRetentionControlle\n\n# --- truncated at 32 KB (59 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/workos/refs/heads/main/agentic-access/workos-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workos/refs/heads/main/agentic-access/workos-agentic-access.yml
summary_line: 172 operations · 98 acting · 98 human-in-the-loop
tags:
- Authentication
- Identity Provider
- SSO
- SAML
- OIDC
- SCIM
- Directory Sync
- Authorization
- FGA
- Audit Logs
- MFA
- B2B SaaS
- Agents
- MCP
---
