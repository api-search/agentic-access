---
acting_count: 137
action_class_counts:
  acting: 137
  connected: 139
api_specs:
- filename: netcracker-qubership-apihub-registry-openapi.yml
  format: yaml
  label: Qubership APIHUB Registry API
  slug: qubership-apihub-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-apihub-registry-openapi.yml
- filename: netcracker-qubership-apihub-admin-openapi.yml
  format: yaml
  label: Qubership APIHUB System Administrators API
  slug: qubership-apihub-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-apihub-admin-openapi.yml
- filename: netcracker-qubership-maas-swagger.yml
  format: yaml
  label: Qubership MaaS (Messaging as a Service) API
  slug: qubership-maas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-maas-swagger.yml
- filename: netcracker-qubership-dbaas-openapi.json
  format: json
  label: Qubership DBaaS Aggregator API
  slug: qubership-dbaas-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/openapi/netcracker-qubership-dbaas-openapi.json
consequence_counts:
  physical: 3
  read: 139
  safety-critical: 36
  write: 98
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 36
kind: agentic-access
layout: agentic-access
method: generated
name: Netcracker Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/bluegreen/v1/operation/commit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/bluegreen/v1/operation/destroy-domain
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/bluegreen/v1/operation/init-domain
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/bluegreen/v1/operation/orphans
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/bluegreen/v1/operation/orphans
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/bluegreen/v1/operation/promote
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/bluegreen/v1/operation/rollback
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/bluegreen/v1/operation/warmup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/bluegreen/v1/operation/{trackingId}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/composite/v1/structures
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/composite/v1/structures/{compositeId}/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/dbaas/declarative/namespaces/{namespace}/service/{serviceName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/declarations/v1/apply
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/declarations/v1/operation/{trackingId}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/dbaas/databases/marked-for-drop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v3/dbaas/databases/marked-for-drop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/dbaas/databases/update-host
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v3/dbaas/migration/databases
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v3/dbaas/migration/databases/with-user-creation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/dbaas/namespaces/{namespace}/databases/link
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/dbaas/namespaces/{namespace}/databases/recreate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v3/dbaas/namespaces/{namespace}/databases/update-classifier/{type}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v3/dbaas/namespaces/{namespace}/databases/update-connection/{type}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/dbaas/namespaces/{namespace}/password-changes
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v3/dbaas/users
operation_count: 276
overview: 'Netcracker exposes 276 API operations that an AI agent could call, of which 137 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 139 read, 98 write, 3 physical, and 36 safety-critical.


  36 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Netcracker
provider_slug: netcracker
slug: netcracker-agentic-access
source_filename: netcracker-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/netcracker-qubership-apihub-admin-openapi.yml, openapi/netcracker-qubership-apihub-registry-openapi.yml,\n  openapi/netcracker-qubership-dbaas-openapi.json, openapi/netcracker-qubership-maas-swagger.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 276\n  by_action_class:\n    acting: 137\n    connected: 139\n  by_consequence:\n    write: 98\n    read: 139\n    physical: 3\n    safety-critical: 36\n  human_in_the_loop_required: 36\noperations:\n- path: /api/v2/admin/transition/move\n  method: post\n  operationId: movePackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/admin/transition/move/{id}\n  method: get\n  operationId: getMoveStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/admin/transition/activity\n  method: get\n  operationId: listActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/admin/transition\n  method: get\n  operationId: listPackageTransitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/roles\n  method: post\n  operationId: postRoles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/roles/{roleId}\n  method: patch\n  operationId: patchRolesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/roles/{roleId}\n  method: delete\n  operationId: deleteRolesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/roles/changeOrder\n  method: post\n  operationId: postRolesChangeOrder\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/admins\n  method: get\n  operationId: getAdmins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/admins\n  method: post\n  operationId: postAdmins\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/admins/{userId}\n  method: delete\n  operationId: deleteAdminsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/builds\n  method: get\n  operationId: listBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/builds/{buildId}\n  method: get\n  operationId: getBuild\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/admin/builds/{buildId}/result\n  method: get\n  operationId: getBuildResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/admin/builds/{buildId}/sources\n  method: get\n  operationId: getBuildSources\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/internal/migrate/operations\n  method: post\n  operationId: startOpsMigration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/internal/migrate/operations/{migrationId}\n  method: get\n  operationId: getMigrationReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/internal/migrate/operations/{migrationId}/suspiciousBuilds\n  method: get\n  operationId: getSuspiciousBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/internal/migrate/operations/{migrationId}/perf\n  method: get\n  operationId: getMigrationPerfReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/internal/migrate/operations/cancel\n  method: post\n  operationId: cancelRunningMigrations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/system/info\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/system/configuration\n  method: get\n  operationId: getSystemConfiguration\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/system/configuration\n  method: get\n  operationId: getSystemConfigurationV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/logout\n  method: post\n  operationId: logoutUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/export\n  method: post\n  operationId: postExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/export/{exportId}/status\n  method: get\n  operationId: getExportIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/activity\n  method: get\n  operationId: getActivityV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages\n  method: post\n  operationId: postPackages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/packages\n  method: get\n  operationId: getPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}\n  method: get\n  operationId: getPackagesId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}\n  method: patch\n  operationId: patchPackagesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/packages/{packageId}\n  method: delete\n  operationId: deletePackagesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /api/v1/packages/{packageId}/exportConfig\n  method: get\n  operationId: getPackageIdExportConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/exportConfig\n  method: patch\n  operationId: patchPackagesIdExportConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/packages/{packageId}/activity\n  method: get\n  operationId: getPackageIdActivityV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/packages/{packageId}/apiKeys\n  method: post\n  operationId: postPackagesIdApiKeysV4\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/packages/{packageId}/apiKeys\n  method: get\n  operationId: getPackagesIdApiKeysV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/apiKeys/{id}\n  method: delete\n  operationId: deletePackagesIdApiKeysId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/personalAccessToken\n  method: post\n  operationId: postPersonalAccessToken\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/personalAccessToken\n  method: get\n  operationId: getPersonalAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/personalAccessToken/{id}\n  method: delete\n  operationId: deletePersonalAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/packages/{packageId}/favor\n  method: post\n  operationId: postPackagesIdFavor\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/packages/{packageId}/disfavor\n  method: post\n  operationId: postPackagesIdDisfavor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/packages/{packageId}/publish\n  method: post\n  operationId: postPackagesIdPublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v2/packages/{packageId}/publish/{publishId}/status\n  method: get\n  operationId: getPackagesIdPublishIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/publish/withOperationsGroup\n  method: post\n  operationId: DashboardPublishWithOperationsGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/packages/{packageId}/publish/{publishId}/withOperationsGroup/status\n  method: get\n  operationId: getDashboardPublishWithOperationsGroupStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/publish/{publishId}/withOperationsGroup/status/report\n\
  \  method: get\n  operationId: getDashboardPublishWithOperationsGroupStatusReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/publish/withOperationsGroup/{apiType}\n  method: post\n  operationId: DashboardPublishWithOperationsGroupV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/packages/{packageId}/versions\n  method: get\n  operationId: getPackagesIdVersionsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}\n  method: patch\n  operationId: patchPackagesIdVersionsIdV2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/packages/{packageId}/versions/{version}\n  method: delete\n  operationId: deletePackagesIdVersionsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/packages/{packageId}/versions/{version}\n  method: get\n  operationId: getPackagesIdVersionsIdV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/changes/summary\n\
  \  method: get\n  operationId: getPackageIdVersionChangesSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/packages/{packageId}/versions/{version}/{apiType}/changes\n  method: get\n  operationId: getPackagesIdVersionsIdApiTypeChangesV4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/packages/{packageId}/versions/{version}/{apiType}/export/changes\n  method: get\n  operationId: getPackageIdVersionIdChangesExportV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/changes/export\n  method: get\n  operationId: getPackageIdVersionIdChangesExport\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/sources\n  method: get\n  operationId: getPackagesIdVersionsIdSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/config\n  method: get\n  operationId: getPackagesIdVersionsIdConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/copy\n  method: post\n  operationId: getPackageIdVersionIdCopy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v2/compare\n  method: post\n  operationId: postCompare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/packages/{packageId}/versions/{version}/{apiType}/build/groups/{groupName}/buildType/{buildType}\n  method: post\n  operationId: postGenerateDocumentV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/packages/{packageId}/versions/{version}/{apiType}/export/groups/{groupName}/buildType/{buildType}\n  method: get\n  operationId: getPackagesIdVersionsIdExportGroupNameV3\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/files/{slug}/raw\n  method: get\n  operationId: getPackagesIdVersionsIdFilesSlugRaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/files/{slug}/doc\n  method: get\n  operationId: getPackagesIdVersionsIdFilesSlugDoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/sourceData\n  method: get\n  operationId: getPackageVersionSourcesWithBuildConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v2/packages/{packageId}/versions/{version}/doc\n  method: get\n  operationId: getPackagesIdVersionsIdDoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/version-internal-documents/{hash}\n  method: get\n  operationId: getVersionInternalDocumentsHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/comparison-internal-documents/{hash}\n  method: get\n  operationId: getComparisonInternalDocumentsHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/permissions\n  method: get\n  operationId: getPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v2/roles\n  method: get\n  operationId: getRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/availableRoles\n  method: get\n  operationId: getPackagesIdAvailableRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/members\n  method: post\n  operationId: postPackagesIdMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/packages/{packageId}/members\n  method: get\n  operationId: getPackagesIdMembers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/members/{userId}\n  method: patch\n  operationId: patchPackagesIdMembersId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/packages/{packageId}/members/{userId}\n  method: delete\n  operationId: deletePackagesIdMembersId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sharedFiles\n  method: post\n  operationId: postSharedFiles\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sharedFiles/{sharedFileId}\n  method: get\n  operationId: getSharedFilesId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user\n  method: get\n  operationId: getExtendedUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/user\n  method: get\n  operationId: getExtendedUserV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/operations\n  method: get\n  operationId: getPackagesIdVersionsIdApiTypeOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/ddl/entities\n  method: get\n  operationId: getPackageVersionDdlEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/ddl/entities/{ddlEntityId}\n  method: get\n  operationId:\
  \ getPackageVersionDdlEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/ddl/entities/{ddlEntityId}/changes\n  method: get\n  operationId: getPackageVersionDdlEntityChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/ddl/changes\n  method: get\n  operationId: getPackageVersionDdlChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/ddl/entities/{ddlEntityId}/changes/summary\n  method: get\n  operationId: getPackageVersionDdlEntityChangesSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/ddl/export/entities\n  method: get\n  operationId: getPackageVersionDdlEntitiesExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/ddl/export/changes\n  method: get\n  operationId: getPackageVersionDdlChangesExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/mcp/{entity}\n  method: get\n  operationId: getPackageVersionMcpEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/mcp/{entity}/{mcpEntityId}\n\
  \  method: get\n  operationId: getPackageVersionMcpEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/{packageId}/versions/{version}/mcp/export/{entity}\n  method: get\n  operationId: getPackageVersionMcpEntitiesExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/deprecated/summary\n  method: get\n  operationId: getPackageIdVersionDeprecatedSummaryV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/deprecated\n  method: get\n  operationId: getPackagesIdVersionsIdApiTypeDeprecations\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/operations/{operationId}/deprecatedItems\n  method: get\n  operationId: getPackagesIdVersionsApiTypeOperationsIddeprecatedItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/operations/{operationId}/models/{modelName}/usages\n  method: get\n  operationId: getPackagesIdVersionsApiTypeOperationsIdModelsModelName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/export/operations\n  method: get\n  operationId: getPackagesIdVersionsIdApiTypeOperationsExport\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/export/operations/deprecated\n  method: get\n  operationId: getPackagesIdVersionsIdApiTypeDeprecatedOperationsExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/operations/{operationId}\n  method: get\n  operationId: getPackagesIdVersionsIdApiTypeOperationsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/operations/{operationId}/changes\n  method: get\n  operationId: getPackagesIdVersionsApiTypeOperationsIdChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/operations/{operationId}/changes/summary\n  method: get\n  operationId: getPackagesIdVersionsApiTypeOperationsIdChangesSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/tags\n  method: get\n  operationId: getPackagesIdVersionsIdApiTypeTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/packages/{packageId}/versions/{version}/{apiType}/groups\n  method: post\n  operationId: PostPackageIdVersionApiTypeGroupsV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/groups/{groupName}\n  method: get\n  operationId: getPackagesIdVersionsIdApiTypeGroupsGroupName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/versions/{version}/{apiType}/groups/{groupName}\n  method: delete\n  operationId: getPackagesIdVersionsIdApiTypeGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/packages/{packageId}/versions/{version}/{apiType}/groups/{groupName}\n  method: patch\n  operationId: patchPackageIdVersionApiTypeGroupName\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/packages/{packageId}/versions/{version}/{apiType}/groups/{groupName}/template\n  method: get\n  operationId: getPackageIdVersionApiTypeGroupNameTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/calculateGroups\n  method: get\n  operationId: postPackagesIdCalculateGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/packages/{packageId}/recalculateGroups\n  method: post\n  operationId: postPac\n\n# --- truncated at 32 KB (85 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/agentic-access/netcracker-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netcracker/refs/heads/main/agentic-access/netcracker-agentic-access.yml
summary_line: 276 operations · 137 acting · 36 human-in-the-loop
tags:
- Telecommunications
- United States
- BSS
- OSS
- Network Vendor
- API Management
- TM Forum
- OpenAPI
- CAMARA
- Standards
- Orchestration
- Monetization
- Open-Source
---
