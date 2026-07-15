---
acting_count: 134
action_class_counts:
  acting: 134
  connected: 143
api_specs:
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Groups
  slug: rest-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Organizations
  slug: rest-organizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Projects
  slug: rest-projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Issues
  slug: rest-issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Targets
  slug: rest-targets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Integrations
  slug: rest-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Audit Logs
  slug: rest-audit-logs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - SBOMs
  slug: rest-sboms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Container Images
  slug: rest-container-images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Custom Base Images
  slug: rest-custom-base-images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Webhooks
  slug: rest-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Export
  slug: rest-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
consequence_counts:
  physical: 22
  read: 143
  safety-critical: 9
  write: 103
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 9
kind: agentic-access
layout: agentic-access
method: generated
name: Snyk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /groups/{group_id}/apps/installs/{install_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /orgs/{org_id}/app_bots/{bot_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /orgs/{org_id}/apps/installs/{install_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /orgs/{org_id}/settings/sast
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /orgs/{org_id}/slack_app/{bot_id}/projects/{project_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /orgs/{org_id}/slack_app/{bot_id}/projects/{project_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /self/apps/installs/{install_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /self/apps/{app_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /self/apps/{app_id}/sessions/{session_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /groups/{group_id}/memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /groups/{group_id}/memberships/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /groups/{group_id}/memberships/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orgs/{org_id}/collections/{collection_id}/relationships/projects
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{org_id}/collections/{collection_id}/relationships/projects
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{org_id}/memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orgs/{org_id}/memberships/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /orgs/{org_id}/memberships/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tenants/{tenant_id}/brokers/installs/{install_id}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /tenants/{tenant_id}/brokers/installs/{install_id}/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /tenants/{tenant_id}/brokers/installs/{install_id}/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /tenants/{tenant_id}/brokers/installs/{install_id}/deployments/{deployment_id}/connections
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tenants/{tenant_id}/brokers/installs/{install_id}/deployments/{deployment_id}/connections
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /tenants/{tenant_id}/brokers/installs/{install_id}/deployments/{deployment_id}/connections/{connection_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /tenants/{tenant_id}/brokers/installs/{install_id}/deployments/{deployment_id}/connections/{connection_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tenants/{tenant_id}/brokers/installs/{install_id}/deployments/{deployment_id}/connections/{connection_id}/bulk_migration
operation_count: 277
overview: 'Snyk exposes 277 API operations that an AI agent could call, of which 134 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 143 read, 103 write, 22 physical, and 9 safety-critical.


  9 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Snyk
provider_slug: snyk
slug: snyk-agentic-access
source_filename: snyk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/snyk-rest-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 277\n  by_action_class:\n    connected: 143\n    acting: 134\n  by_consequence:\n    read: 143\n    write: 103\n    safety-critical: 9\n    physical: 22\n  human_in_the_loop_required: 9\noperations:\n- path: /custom_base_images\n  method: get\n  operationId: getCustomBaseImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_base_images\n  method: post\n  operationId: createCustomBaseImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom_base_images/{custombaseimage_id}\n  method: delete\n  operationId: deleteCustomBaseImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom_base_images/{custombaseimage_id}\n  method: get\n  operationId: getCustomBaseImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_base_images/{custombaseimage_id}\n  method: patch\n  operationId: updateCustomBaseImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/apps/installs\n  method: get\n  operationId: getAppInstallsForGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/apps/installs\n  method: post\n  operationId: createGroupAppInstall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/apps/installs/{install_id}\n  method: delete\n  operationId: deleteGroupAppInstallById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /groups/{group_id}/apps/installs/{install_id}/secrets\n  method: post\n  operationId: updateGroupAppInstallSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /groups/{group_id}/assets/repository/aliases\n  method: delete\n  operationId: deleteAliasesInGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/assets/repository/aliases\n  method: get\n  operationId: listRepositoryAliasesInGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/assets/repository/aliases\n  method: post\n  operationId: createAliasInGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/assets/search\n  method: post\n  operationId: listAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/assets/{asset_id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/assets/{asset_id}\n  method: patch\n  operationId: updateAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /groups/{group_id}/assets/{asset_id}/relationships/assets\n  method: get\n  operationId: listRelatedAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/assets/{asset_id}/relationships/projects\n  method: get\n  operationId: listAssetProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/audit_logs/search\n  method: get\n  operationId: listGroupAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/export\n  method: post\n  operationId: createGroupExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/export/{export_id}\n  method: get\n  operationId: getGroupExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/inventory/assets\n  method: get\n  operationId: listAssetsGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/inventory/assets\n  method: patch\n  operationId: updateAssetsBulkGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /groups/{group_id}/inventory/assets/filters\n  method: get\n  operationId: getFilterFieldsGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/inventory/assets/filters/{filter_id}/values\n  method: get\n  operationId: getFilterValuesGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/inventory/assets/groups\n  method: get\n  operationId: getGroupFieldsGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/inventory/assets/groups/{group_field_id}/values\n  method: get\n  operationId: getGroupValuesGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/inventory/assets/searches\n  method: post\n  operationId: createAssetSearchGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/inventory/assets/searches/{search_id}/results\n  method: get\n  operationId: getAssetSearchResultsGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/inventory/assets/{asset_id}\n  method: get\n  operationId: getAssetGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/inventory/assets/{asset_id}\n\
  \  method: patch\n  operationId: updateAssetGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/inventory/assets/{asset_id}/relationships/projects\n  method: get\n  operationId: listAssetProjectsGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/inventory/assets/{asset_id}/relationships/targets\n  method: get\n  operationId: listAssetTargetsGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/issues\n  method: get\n  operationId: listGroupIssues\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/issues/{issue_id}\n  method: get\n  operationId: getGroupIssueByIssueID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/jobs/export/{export_id}\n  method: get\n  operationId: getGroupExportJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/memberships\n  method: get\n  operationId: listGroupMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/memberships\n  method: post\n  operationId: createGroupMembership\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/memberships/{membership_id}\n  method: delete\n  operationId: deleteGroupMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/memberships/{membership_id}\n  method: patch\n  operationId: updateGroupUserMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/org_memberships\n  method: get\n  operationId: listGroupUserOrgMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/orgs\n  method: get\n  operationId: listOrgsInGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/policies\n  method: get\n  operationId: listGroupPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/policies\n  method: post\n  operationId: createGroupPolicy\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/policies/{policy_id}\n  method: delete\n  operationId: deleteGroupPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/policies/{policy_id}\n  method: patch\n  operationId: updateGroupPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/service_accounts\n\
  \  method: get\n  operationId: getManyGroupServiceAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/service_accounts\n  method: post\n  operationId: createGroupServiceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/service_accounts/{serviceaccount_id}\n  method: delete\n  operationId: deleteOneGroupServiceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/service_accounts/{serviceaccount_id}\n\
  \  method: get\n  operationId: getOneGroupServiceAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/service_accounts/{serviceaccount_id}\n  method: patch\n  operationId: updateGroupServiceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/service_accounts/{serviceaccount_id}/secrets\n  method: post\n  operationId: updateServiceAccountSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /groups/{group_id}/settings/iac\n  method: get\n  operationId: getIacSettingsForGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/settings/iac\n  method: patch\n  operationId: updateIacSettingsForGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/settings/opensource/broker\n  method: delete\n  operationId: deleteOpensourceBrokerSettingForGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /groups/{group_id}/settings/opensource/broker\n  method: get\n  operationId: getOpensourceBrokerSettingForGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/settings/opensource/broker\n  method: post\n  operationId: enableOpensourceBrokerForGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/settings/pull_request_template\n  method: delete\n  operationId: deletePullRequestTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/settings/pull_request_template\n  method: get\n  operationId: getPullRequestTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/settings/pull_request_template\n  method: post\n  operationId: createOrUpdatePullRequestTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/sso_connections\n  method: get\n  operationId: listGroupSsoConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /groups/{group_id}/sso_connections/{sso_id}/users\n  method: get\n  operationId: listGroupSsoConnectionUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}/sso_connections/{sso_id}/users/{user_id}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/users/{id}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /learn/catalog\n  method: get\n  operationId: listLearnCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi\n  method: get\n  operationId: listAPIVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/{version}\n  method: get\n  operationId: getAPIVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs\n  method: get\n  operationId: listOrgs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}\n  method: get\n  operationId: getOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}\n  method: patch\n  operationId: updateOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/ai_bom_jobs/{job_id}\n  method: get\n  operationId: getAiBomJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/ai_boms\n  method: post\n  operationId: createAiBom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/ai_boms/upload\n\
  \  method: post\n  operationId: createAndUploadAiBom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/ai_boms/{ai_bom_id}\n  method: get\n  operationId: getAiBom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/app_bots\n  method: get\n  operationId: getAppBots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/app_bots/{bot_id}\n  method: delete\n  operationId: deleteAppBot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /orgs/{org_id}/apps\n  method: get\n  operationId: getApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/apps\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/creations\n  method: get\n  operationId: getOrgApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/apps/creations\n\
  \  method: post\n  operationId: createOrgApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/creations/{app_id}\n  method: delete\n  operationId: deleteAppByID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/creations/{app_id}\n  method: get\n  operationId: getAppByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/apps/creations/{app_id}\n  method: patch\n  operationId:\
  \ updateAppCreationByID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/creations/{app_id}/secrets\n  method: post\n  operationId: manageAppCreationSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/installs\n  method: get\n  operationId: getAppInstallsForOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/apps/installs\n  method: post\n  operationId: createOrgAppInstall\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/installs/{install_id}\n  method: delete\n  operationId: deleteAppOrgInstallById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /orgs/{org_id}/apps/installs/{install_id}/secrets\n  method: post\n  operationId: updateOrgAppInstallSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{client_id}\n  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{client_id}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/apps/{client_id}\n  method: patch\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{client_id}/secrets\n  method: post\n  operationId: manageSecrets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/assets/repository/aliases\n  method: delete\n  operationId: deleteAliasesInOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/assets/repository/aliases\n  method: get\n  operationId: listRepositoryAliasesInOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/assets/repository/aliases\n  method: post\n  operationId: createAliasInOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/audit_logs/search\n  method: get\n  operationId: listOrgAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/brokers/connections\n  method: get\n  operationId: listBrokerConnectionsForOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/cloud/environments\n  method: get\n  operationId: listEnvironments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/cloud/environments\n  method: post\n  operationId: createEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/cloud/environments/{environment_id}\n  method: delete\n  operationId: deleteEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/cloud/environments/{environment_id}\n  method: patch\n  operationId: updateEnvironment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/cloud/permissions\n  method: post\n  operationId: getPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/cloud/resources\n  method: get\n  operationId: listResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/cloud/scans\n  method: get\n  operationId: listScan\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/cloud/scans\n  method: post\n  operationId: createScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/cloud/scans/{scan_id}\n  method: get\n  operationId: getScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/collections\n  method: get\n  operationId: getCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/collections\n  method: post\n  operationId: createCollectio\n\n#\
  \ --- truncated at 32 KB (83 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/agentic-access/snyk-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/agentic-access/snyk-agentic-access.yml
summary_line: 277 operations · 134 acting · 9 human-in-the-loop
tags:
- Security
- DevSecOps
- Vulnerability Management
- Application Security
- SCA
- SAST
- Container Security
- IaC
---
