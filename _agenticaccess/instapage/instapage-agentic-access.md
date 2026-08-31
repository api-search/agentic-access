---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 16
api_specs:
- filename: instapage-workspaces-api-openapi.yml
  format: yaml
  label: Instapage Workspaces API
  slug: instapage-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-workspaces-api-openapi.yml
- filename: instapage-analytics-api-openapi.yml
  format: yaml
  label: Instapage Analytics API
  slug: instapage-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-analytics-api-openapi.yml
- filename: instapage-assets-api-openapi.yml
  format: yaml
  label: Instapage Assets API
  slug: instapage-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-assets-api-openapi.yml
- filename: instapage-collections-api-openapi.yml
  format: yaml
  label: Instapage Collections API
  slug: instapage-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-collections-api-openapi.yml
- filename: instapage-domains-api-openapi.yml
  format: yaml
  label: Instapage Domains API
  slug: instapage-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-domains-api-openapi.yml
- filename: instapage-experiments-api-openapi.yml
  format: yaml
  label: Instapage Experiments API
  slug: instapage-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-experiments-api-openapi.yml
- filename: instapage-form-submissions-api-openapi.yml
  format: yaml
  label: Instapage Form Submissions API
  slug: instapage-form-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-form-submissions-api-openapi.yml
- filename: instapage-groups-api-openapi.yml
  format: yaml
  label: Instapage Groups API
  slug: instapage-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-groups-api-openapi.yml
- filename: instapage-pages-api-openapi.yml
  format: yaml
  label: Instapage Pages API
  slug: instapage-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-pages-api-openapi.yml
- filename: instapage-personalizations-api-openapi.yml
  format: yaml
  label: Instapage Personalizations API
  slug: instapage-personalizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-personalizations-api-openapi.yml
- filename: instapage-team-members-api-openapi.yml
  format: yaml
  label: Instapage Team Members API
  slug: instapage-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-team-members-api-openapi.yml
consequence_counts:
  read: 16
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Instapage Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 39
overview: 'Instapage exposes 39 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 23 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Instapage
provider_slug: instapage
slug: instapage-agentic-access
source_filename: instapage-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/instapage-analytics-openapi.yml, openapi/instapage-assets-openapi.yml, openapi/instapage-collections-openapi.yml,\n  openapi/instapage-domains-openapi.yml, openapi/instapage-experiments-openapi.yml, openapi/instapage-form-submissions-openapi.yml,\n  openapi/instapage-groups-openapi.yml, openapi/instapage-pages-openapi.yml, openapi/instapage-personalizations-openapi.yml,\n  openapi/instapage-team-members-openapi.yml, openapi/instapage-workspaces-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 23\n    connected: 16\n  by_consequence:\n    write: 23\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /workspaces/{workspaceId}/analytics\n\
  \  method: post\n  operationId: getAnalytics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/assets/images/folders\n  method: get\n  operationId: listImageFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/assets/images/folders/{folderId}/items\n  method: get\n  operationId: listImagesInFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/assets/images/folders/{folderId}/items\n  method: post\n  operationId: uploadImage\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/collections/{collectionId}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/collections/{collectionId}/collection-pages\n  method: get\n  operationId: listCollectionPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /workspaces/{workspaceId}/collections/{collectionId}/collection-pages\n  method: post\n  operationId: createCollectionPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/collections/{collectionId}/collection-pages/{collectionPageId}/publication\n  method: post\n  operationId: publishCollectionPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/collections/{collectionId}/collection-pages/{collectionPageId}/publication\n  method: delete\n  operationId:\
  \ unpublishCollectionPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/collections/{collectionId}/collection-pages/{collectionPageId}\n  method: delete\n  operationId: deleteCollectionPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/experiments\n\
  \  method: get\n  operationId: listExperiments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/submissions\n  method: post\n  operationId: retrieveFormSubmissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/submissions\n  method: delete\n  operationId: deleteFormSubmissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/groups\n  method:\
  \ get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/groups/{groupId}\n  method: put\n  operationId: updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/groups/{groupId}\n  method: delete\n  operationId:\
  \ deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/pages/{pageId}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/pages/{pageId}\n  method: patch\n  operationId: updatePage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/pages/{pageId}\n  method: delete\n  operationId: deletePage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/pages/{pageId}/publication\n  method: post\n  operationId: publishPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/pages/{pageId}/publication\n  method: put\n  operationId: updatePublishedPageUrl\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/pages/{pageId}/publication\n  method: delete\n  operationId: unpublishPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pages/search\n  method: get\n  operationId: searchPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/pages/json\n  method: post\n  operationId: createPageFromJson\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/pages/{pageId}/json\n  method: get\n  operationId: exportPageAsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/pages/{pageId}/personalizations\n  method: get\n  operationId: listPersonalizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/team-members\n  method: get\n  operationId: listTeamMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/team-members\n\
  \  method: post\n  operationId: inviteTeamMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/team-members\n  method: put\n  operationId: updateTeamMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/team-members\n  method: delete\n  operationId: removeTeamMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}\n  method: patch\n  operationId: renameWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}\n  method: delete\n  operationId: deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/agentic-access/instapage-agentic-access.yml
summary_line: 39 operations · 23 acting
tags:
- Landing Pages
- Conversion Optimization
- Marketing
- A/B Testing
- Post-Click Optimization
- Lead Generation
---
