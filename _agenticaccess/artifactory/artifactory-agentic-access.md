---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 34
api_specs:
- filename: artifactory-aql-search-api-openapi.yml
  format: yaml
  label: JFrog Artifactory AQL Search API
  slug: artifactory-aql-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-aql-search-api-openapi.yml
- filename: artifactory-artifactory-extensions-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Artifactory Extensions API
  slug: artifactory-artifactory-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-artifactory-extensions-api-openapi.yml
- filename: artifactory-artifacts-storage-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Artifacts & Storage API
  slug: artifactory-artifacts-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-artifacts-storage-api-openapi.yml
- filename: artifactory-base-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Base API
  slug: artifactory-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-base-api-openapi.yml
- filename: artifactory-blobs-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Blobs API
  slug: artifactory-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-blobs-api-openapi.yml
- filename: artifactory-build-diff-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Diff API
  slug: artifactory-build-diff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-diff-api-openapi.yml
- filename: artifactory-build-info-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Info API
  slug: artifactory-build-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-info-api-openapi.yml
- filename: artifactory-build-management-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Management API
  slug: artifactory-build-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-management-api-openapi.yml
- filename: artifactory-build-promotion-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Promotion API
  slug: artifactory-build-promotion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-promotion-api-openapi.yml
- filename: artifactory-catalog-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Catalog API
  slug: artifactory-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-catalog-api-openapi.yml
- filename: artifactory-manifests-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Manifests API
  slug: artifactory-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-manifests-api-openapi.yml
- filename: artifactory-replication-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Replication API
  slug: artifactory-replication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-replication-api-openapi.yml
- filename: artifactory-repositories-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Repositories API
  slug: artifactory-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-repositories-api-openapi.yml
- filename: artifactory-search-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Search API
  slug: artifactory-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-search-api-openapi.yml
- filename: artifactory-security-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Security API
  slug: artifactory-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-security-api-openapi.yml
- filename: artifactory-system-configuration-api-openapi.yml
  format: yaml
  label: JFrog Artifactory System & Configuration API
  slug: artifactory-system-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-system-configuration-api-openapi.yml
- filename: artifactory-tags-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Tags API
  slug: artifactory-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-tags-api-openapi.yml
consequence_counts:
  physical: 1
  read: 34
  safety-critical: 1
  write: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Artifactory Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/security/apiKey
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{repoKey}/{itemPath}
operation_count: 69
overview: 'JFrog Artifactory exposes 69 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 33 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: JFrog Artifactory
provider_slug: artifactory
slug: artifactory-agentic-access
source_filename: artifactory-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/artifactory-aql-api-openapi.yml, openapi/artifactory-build-integration-api-openapi.yml,\n  openapi/artifactory-docker-registry-api-openapi.yml, openapi/artifactory-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    acting: 35\n    connected: 34\n  by_consequence:\n    write: 33\n    read: 34\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/search/aql\n  method: post\n  operationId: executeAqlQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/build\n  method: put\n  operationId: publishBuildInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/build/{buildName}\n  method: get\n  operationId: getBuildRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/build/{buildName}\n  method: delete\n  operationId: deleteBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/build/{buildName}/{buildNumber}\n  method: get\n  operationId: getBuildInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/build/promote/{buildName}/{buildNumber}\n  method: post\n  operationId: promoteBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/build/rename/{buildName}\n  method: post\n  operationId: renameBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/build/diff/{buildName}/{buildNumber}\n\
  \  method: get\n  operationId: getBuildDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/build/retention/{buildName}\n  method: post\n  operationId: setBuildRetention\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/build/retention/{buildName}\n  method: get\n  operationId: getBuildRetention\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/\n  method: get\n  operationId: checkApiVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/_catalog\n  method: get\n  operationId: listRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{name}/tags/list\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{name}/manifests/{reference}\n  method: get\n  operationId: getManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{name}/manifests/{reference}\n  method: put\n  operationId: putManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/{name}/manifests/{reference}\n  method: delete\n  operationId: deleteManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{name}/blobs/{digest}\n  method: get\n  operationId: getBlob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{name}/blobs/{digest}\n  method: head\n  operationId: checkBlobExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{name}/blobs/{digest}\n  method: delete\n  operationId: deleteBlob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{name}/blobs/uploads/\n  method: post\n  operationId: initiateUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{name}/blobs/uploads/{uuid}\n  method: patch\n  operationId: uploadBlobChunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{name}/blobs/uploads/{uuid}\n  method: put\n  operationId: completeUpload\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{name}/blobs/uploads/{uuid}\n  method: delete\n  operationId: cancelUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/docker/{repoKey}/v2/promote\n  method: post\n  operationId: promoteDockerImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/system/ping\n  method: get\n  operationId: systemPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/system/version\n  method: get\n  operationId: getSystemVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/system/configuration\n  method: get\n  operationId: getSystemConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/system/configuration\n  method: patch\n  operationId: updateSystemConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /api/system/licenses\n  method: get\n  operationId: getLicenseInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/storage/{repoKey}/{itemPath}\n  method: get\n  operationId: getStorageInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repositories\n  method: get\n  operationId: listRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repositories/{repoKey}\n  method: get\n  operationId: getRepository\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repositories/{repoKey}\n\
  \  method: put\n  operationId: createOrReplaceRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repositories/{repoKey}\n  method: post\n  operationId: updateRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repositories/{repoKey}\n  method: delete\n  operationId: deleteRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{repoKey}/{itemPath}\n  method: get\n  operationId: retrieveArtifact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{repoKey}/{itemPath}\n  method: put\n  operationId: deployArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{repoKey}/{itemPath}\n  method: delete\n  operationId: deleteArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/copy/{srcRepoKey}/{srcItemPath}\n  method: post\n  operationId: copyArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/move/{srcRepoKey}/{srcItemPath}\n  method: post\n  operationId: moveArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/search/artifact\n  method: get\n  operationId: searchArtifactByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/search/gavc\n  method: get\n  operationId: searchByGAVC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/checksum\n  method: get\n  operationId: searchByChecksum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/prop\n  method: get\n  operationId: searchByProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/dates\n  method: get\n  operationId: searchByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/creation\n  method: get\n  operationId: searchByCreationDate\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/security/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/security/users/{username}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/security/users/{username}\n  method: put\n  operationId: createOrReplaceUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/security/users/{username}\n  method: delete\n  operationId:\
  \ deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/security/groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/security/groups/{groupName}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/security/groups/{groupName}\n  method: put\n  operationId: createOrReplaceGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/security/groups/{groupName}\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/security/permissions\n  method: get\n  operationId: listPermissionTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/security/permissions/{permissionName}\n  method: get\n  operationId: getPermissionTarget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/security/permissions/{permissionName}\n\
  \  method: put\n  operationId: createOrReplacePermissionTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/security/permissions/{permissionName}\n  method: delete\n  operationId: deletePermissionTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/security/token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/security/apiKey\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/security/apiKey\n  method: put\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/security/apiKey\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/storage/{repoKey}/{itemPath}?properties\n  method: get\n  operationId: getItemProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/storage/{repoKey}/{itemPath}?properties\n  method: put\n  operationId: setItemProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/storage/{repoKey}/{itemPath}?properties\n  method: delete\n  operationId: deleteItemProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/replications/{repoKey}\n  method: get\n  operationId: getReplicationConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/replications/{repoKey}\n  method: put\n  operationId: createOrReplaceReplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/replications/{repoKey}\n  method: delete\n  operationId: deleteReplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/system/storage\n  method: get\n  operationId: getStorageSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/agentic-access/artifactory-agentic-access.yml
summary_line: 69 operations · 35 acting · 1 human-in-the-loop
tags:
- Artifacts
- DevOps
- CI/CD
- docker-registry
- Maven
- Package Management
- Repository
---
