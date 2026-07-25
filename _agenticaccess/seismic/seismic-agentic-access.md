---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 37
api_specs:
- filename: seismic-content-analytics-api-openapi.yml
  format: yaml
  label: Seismic Content Analytics API
  slug: seismic-content-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-analytics-api-openapi.yml
- filename: seismic-content-api-openapi.yml
  format: yaml
  label: Seismic Content API
  slug: seismic-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-api-openapi.yml
- filename: seismic-content-profiles-api-openapi.yml
  format: yaml
  label: Seismic Content Profiles API
  slug: seismic-content-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-profiles-api-openapi.yml
- filename: seismic-content-properties-api-openapi.yml
  format: yaml
  label: Seismic Content Properties API
  slug: seismic-content-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-properties-api-openapi.yml
- filename: seismic-data-sources-api-openapi.yml
  format: yaml
  label: Seismic Data Sources API
  slug: seismic-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-data-sources-api-openapi.yml
- filename: seismic-delivery-analytics-api-openapi.yml
  format: yaml
  label: Seismic Delivery Analytics API
  slug: seismic-delivery-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-delivery-analytics-api-openapi.yml
- filename: seismic-delivery-api-openapi.yml
  format: yaml
  label: Seismic Delivery API
  slug: seismic-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-delivery-api-openapi.yml
- filename: seismic-folders-api-openapi.yml
  format: yaml
  label: Seismic Folders API
  slug: seismic-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-folders-api-openapi.yml
- filename: seismic-generation-jobs-api-openapi.yml
  format: yaml
  label: Seismic Generation Jobs API
  slug: seismic-generation-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-generation-jobs-api-openapi.yml
- filename: seismic-groups-api-openapi.yml
  format: yaml
  label: Seismic Groups API
  slug: seismic-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-groups-api-openapi.yml
- filename: seismic-livedocs-api-openapi.yml
  format: yaml
  label: Seismic LiveDocs API
  slug: seismic-livedocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-livedocs-api-openapi.yml
- filename: seismic-reports-api-openapi.yml
  format: yaml
  label: Seismic Reports API
  slug: seismic-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-reports-api-openapi.yml
- filename: seismic-roles-api-openapi.yml
  format: yaml
  label: Seismic Roles API
  slug: seismic-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-roles-api-openapi.yml
- filename: seismic-teams-api-openapi.yml
  format: yaml
  label: Seismic Teams API
  slug: seismic-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-teams-api-openapi.yml
- filename: seismic-templates-api-openapi.yml
  format: yaml
  label: Seismic Templates API
  slug: seismic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-templates-api-openapi.yml
- filename: seismic-user-analytics-api-openapi.yml
  format: yaml
  label: Seismic User Analytics API
  slug: seismic-user-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-user-analytics-api-openapi.yml
- filename: seismic-users-api-openapi.yml
  format: yaml
  label: Seismic Users API
  slug: seismic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-users-api-openapi.yml
consequence_counts:
  physical: 1
  read: 37
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Seismic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /users/{userId}/groups
operation_count: 57
overview: 'Seismic exposes 57 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 19 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Seismic
provider_slug: seismic
slug: seismic-agentic-access
source_filename: seismic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/seismic-analytics-openapi.yml, openapi/seismic-content-openapi.yml, openapi/seismic-livedocs-openapi.yml,\n  openapi/seismic-user-management-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 37\n    acting: 20\n  by_consequence:\n    read: 37\n    write: 19\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /analytics/content\n  method: get\n  operationId: getContentAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/content/{contentId}\n  method: get\n  operationId: getContentItemAnalytics\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/content/top\n  method: get\n  operationId: getTopContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/users\n  method: get\n  operationId: getUserAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/users/{userId}\n  method: get\n  operationId: getUserActivityAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/deliveries\n  method: get\n  operationId: getDeliveryAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/reports/{reportId}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/reports/{reportId}/export\n  method: post\n  operationId: exportReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content\n  method: get\n  operationId: listContentItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content\n  method: post\n  operationId: createContentItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content/{contentId}\n  method: get\n  operationId: getContentItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/{contentId}\n  method: patch\n  operationId: updateContentItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /content/{contentId}\n  method: delete\n  operationId: deleteContentItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content/{contentId}/file\n  method: get\n  operationId: downloadContentFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/{contentId}/file\n  method: put\n  operationId: replaceContentFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content/{contentId}/versions\n  method:\
  \ get\n  operationId: listContentVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/{contentId}/url\n  method: get\n  operationId: getContentUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders/{folderId}\n  method:\
  \ get\n  operationId: getFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders/{folderId}\n  method: patch\n  operationId: updateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders/{folderId}\n  method: delete\n  operationId: deleteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content-properties\n  method: get\n  operationId: listContentProperties\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content-properties/{propertyId}\n  method: get\n  operationId: getContentProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content-profiles\n  method: get\n  operationId: listContentProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content-profiles/{profileId}\n  method: get\n  operationId: getContentProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: searchContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /livedocs/generate\n  method: post\n  operationId: generateLiveDoc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /livedocs/templates\n  method: get\n  operationId: listLiveDocTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /livedocs/templates/{templateId}\n  method: get\n  operationId: getLiveDocTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /livedocs/templates/{templateId}/inputs\n\
  \  method: get\n  operationId: getLiveDocTemplateInputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /livedocs/templates/{templateId}/preview\n  method: post\n  operationId: previewLiveDocTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /livedocs/jobs\n  method: get\n  operationId: listGenerationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /livedocs/jobs/{jobId}\n  method: get\n  operationId: getGenerationJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /livedocs/datasources\n  method: get\n  operationId: listDataSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /livedocs/datasources/{dataSourceId}\n  method: get\n  operationId: getDataSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/groups\n  method: get\n  operationId: getUserGroups\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/groups\n  method: put\n  operationId: setUserGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}\n  method: patch\n  operationId: updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /groups/{groupId}/members\n  method: get\n  operationId: listGroupMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}/members\n  method: post\n  operationId: addGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/members/{userId}\n  method: delete\n  operationId: removeGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles\n  method: get\n  operationId:\
  \ listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles/{roleId}\n  method: get\n  operationId: getRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{teamId}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{teamId}/members\n  method: get\n  operationId: listTeamMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/agentic-access/seismic-agentic-access.yml
summary_line: 57 operations · 20 acting
tags: []
---
