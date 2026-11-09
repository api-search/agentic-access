---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 29
api_specs:
- filename: quickbase-apps-api-openapi.yml
  format: yaml
  label: Quickbase Apps API
  slug: quickbase-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-apps-api-openapi.yml
- filename: quickbase-audit-api-openapi.yml
  format: yaml
  label: Quickbase Audit API
  slug: quickbase-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-audit-api-openapi.yml
- filename: quickbase-auth-api-openapi.yml
  format: yaml
  label: Quickbase Auth API
  slug: quickbase-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-auth-api-openapi.yml
- filename: quickbase-document-templates-api-openapi.yml
  format: yaml
  label: Quickbase Document Templates API
  slug: quickbase-document-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-document-templates-api-openapi.yml
- filename: quickbase-fields-api-openapi.yml
  format: yaml
  label: Quickbase Fields API
  slug: quickbase-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-fields-api-openapi.yml
- filename: quickbase-files-api-openapi.yml
  format: yaml
  label: Quickbase Files API
  slug: quickbase-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-files-api-openapi.yml
- filename: quickbase-formulas-api-openapi.yml
  format: yaml
  label: Quickbase Formulas API
  slug: quickbase-formulas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-formulas-api-openapi.yml
- filename: quickbase-groups-api-openapi.yml
  format: yaml
  label: Quickbase Groups API
  slug: quickbase-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-groups-api-openapi.yml
- filename: quickbase-platform-analytics-api-openapi.yml
  format: yaml
  label: Quickbase Platform Analytics API
  slug: quickbase-platform-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-platform-analytics-api-openapi.yml
- filename: quickbase-records-api-openapi.yml
  format: yaml
  label: Quickbase Records API
  slug: quickbase-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-records-api-openapi.yml
- filename: quickbase-reports-api-openapi.yml
  format: yaml
  label: Quickbase Reports API
  slug: quickbase-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-reports-api-openapi.yml
- filename: quickbase-solutions-api-openapi.yml
  format: yaml
  label: Quickbase Solutions API
  slug: quickbase-solutions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-solutions-api-openapi.yml
- filename: quickbase-tables-api-openapi.yml
  format: yaml
  label: Quickbase Tables API
  slug: quickbase-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-tables-api-openapi.yml
- filename: quickbase-trustees-api-openapi.yml
  format: yaml
  label: Quickbase Trustees API
  slug: quickbase-trustees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-trustees-api-openapi.yml
- filename: quickbase-users-api-openapi.yml
  format: yaml
  label: Quickbase Users API
  slug: quickbase-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-users-api-openapi.yml
- filename: quickbase-user-token-api-openapi.yml
  format: yaml
  label: Quickbase User Token API
  slug: quickbase-user-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-user-token-api-openapi.yml
consequence_counts:
  physical: 4
  read: 29
  write: 34
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Quickbase Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tables/{tableId}/relationship
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tables/{tableId}/relationship/{relationshipId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /tables/{tableId}/relationship/{relationshipId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /usertoken/transfer
operation_count: 67
overview: 'Quickbase exposes 67 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 34 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Quickbase
provider_slug: quickbase
slug: quickbase-agentic-access
source_filename: quickbase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/quickbase-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 67\n  by_action_class:\n    acting: 38\n    connected: 29\n  by_consequence:\n    write: 34\n    read: 29\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /apps\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appId}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appId}\n  method: post\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appId}\n  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appId}/events\n  method: get\n  operationId: getAppEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appId}/copy\n\
  \  method: post\n  operationId: copyApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appId}/roles\n  method: get\n  operationId: getRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables\n  method: get\n  operationId: getAppTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables\n  method: post\n  operationId: createTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableId}\n  method: get\n  operationId: getTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables/{tableId}\n  method: post\n  operationId: updateTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableId}\n  method: delete\n  operationId: deleteTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableId}/relationships\n\
  \  method: get\n  operationId: getRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tables/{tableId}/relationship\n  method: post\n  operationId: createRelationship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableId}/relationship/{relationshipId}\n  method: post\n  operationId: updateRelationship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /tables/{tableId}/relationship/{relationshipId}\n  method: delete\n  operationId: deleteRelationship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports\n  method: get\n  operationId: getTableReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{reportId}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{reportId}/run\n  method: post\n  operationId: runReport\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields\n  method: get\n  operationId: getFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields\n  method: post\n  operationId: createField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields\n  method: delete\n  operationId: deleteFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields/{fieldId}\n  method: get\n  operationId: getField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields/{fieldId}\n  method: post\n  operationId: updateField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields/usage\n  method: get\n  operationId: getFieldsUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields/usage/{fieldId}\n  method: get\n  operationId:\
  \ getFieldUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /formula/run\n  method: post\n  operationId: runFormula\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /records\n  method: post\n  operationId: upsert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /records\n  method: delete\n  operationId: deleteRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /records/query\n  method: post\n  operationId: runQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records/modifiedSince\n  method: post\n  operationId: recordsModifiedSince\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/temporary/{dbid}\n  method: get\n  operationId: getTempTokenDBID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/token\n  method: post\n  operationId: exchangeSsoToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usertoken/clone\n  method: post\n  operationId: cloneUserToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usertoken/transfer\n  method: post\n  operationId: transferUserToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usertoken/deactivate\n\
  \  method: post\n  operationId: deactivateUserToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usertoken\n  method: delete\n  operationId: deleteUserToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{tableId}/{recordId}/{fieldId}/{versionNumber}\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{tableId}/{recordId}/{fieldId}/{versionNumber}\n  method:\
  \ delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: post\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/deny\n  method: put\n  operationId: denyUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/deny/{shouldDeleteFromGroups}\n  method: put\n  operationId: denyUsersAndGroups\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/undeny\n  method: put\n  operationId: undenyUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/apps\n  method: get\n  operationId: getUserApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{gid}/members\n  method: post\n  operationId: addMembersToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{gid}/members\n  method: delete\n  operationId: removeMembersFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{gid}/managers\n  method: post\n  operationId: addManagersToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{gid}/managers\n  method: delete\n  operationId: removeManagersFromGroup\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{gid}/subgroups\n  method: post\n  operationId: addSubgroupsToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{gid}/subgroups\n  method: delete\n  operationId: removeSubgroupsFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audit\n  method: post\n\
  \  operationId: audit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/reads\n  method: get\n  operationId: platformAnalyticReads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/events/summaries\n  method: post\n  operationId: platformAnalyticEventSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docTemplates/{templateId}/generate\n  method: get\n  operationId: generateDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solutions/{solutionId}\n  method: get\n  operationId: exportSolution\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solutions/{solutionId}\n  method: put\n  operationId: updateSolution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /solutions\n  method: post\n  operationId: createSolution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /solutions/{solutionId}/torecord\n  method: get\n  operationId: exportSolutionToRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /solutions/fromrecord\n  method: get\n  operationId: createSolutionFromRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solutions/{solutionId}/fromrecord\n  method: get\n  operationId: updateSolutionFromRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solutions/{solutionId}/changeset\n  method: put\n  operationId: changesetSolution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /solutions/{solutionId}/changeset/fromrecord\n  method: get\n  operationId: changesetSolutionFromRecord\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /solutions/{solutionId}/resources\n  method: get\n  operationId: getSolutionPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/{appId}/trustees\n  method: get\n  operationId: getTrustees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/{appId}/trustees\n  method: post\n  operationId: addTrustees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/{appId}/trustees\n  method: delete\n\
  \  operationId: removeTrustees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/{appId}/trustees\n  method: patch\n  operationId: updateTrustees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/quickbase/agentic-access/quickbase-agentic-access.yml
summary_line: 67 operations · 38 acting
tags:
- Company
- Low-Code
- No-Code
- Application Development
- Project Management
- Workflow Automation
- Database
---
