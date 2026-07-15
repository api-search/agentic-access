---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 21
api_specs:
- filename: overview
  format: yaml
  label: SAP Analytics Cloud API
  slug: sap-analytics-cloud-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/SACOpenAPI/overview
- filename: sap-analytics-cloud-data-export-api-openapi.yml
  format: yaml
  label: SAP Analytics Cloud Data Export API
  slug: sap-analytics-cloud-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-analytics-cloud-data-export-api-openapi.yml
- filename: overview
  format: yaml
  label: SAP HANA Cloud Data Lake Files REST API
  slug: sap-hana-cloud-data-lake-files-rest-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/HanaCloudDataLake/overview
- filename: overview
  format: yaml
  label: SAP Datasphere API
  slug: sap-datasphere-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/Datasphere/overview
consequence_counts:
  read: 21
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sap Bi Tools Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'SAP BI Tools exposes 32 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SAP BI Tools
provider_slug: sap-bi-tools
slug: sap-bi-tools-agentic-access
source_filename: sap-bi-tools-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sap-analytics-cloud-api-openapi.yml, openapi/sap-analytics-cloud-content-network-api-openapi.yml,\n  openapi/sap-analytics-cloud-data-export-api-openapi.yml, openapi/sap-businessobjects-bi-platform-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 21\n    acting: 11\n  by_consequence:\n    read: 21\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/stories\n  method: get\n  operationId: listStories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stories/{storyId}\n  method: get\n  operationId:\
  \ getStory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/Resources\n  method: get\n  operationId: listResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/scim/Users\n  method: get\n  operationId: listUsersScim1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/scim2/Users\n  method: get\n  operationId: listUsersScim2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/scim2/Users\n  method: post\n  operationId: createUserScim2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scim2/Users/{userId}\n  method: get\n  operationId: getUserScim2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/scim2/Users/{userId}\n  method: put\n  operationId: updateUserScim2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scim2/Users/{userId}\n  method: delete\n  operationId: deleteUserScim2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scim2/Groups\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/scim2/Groups\n  method: post\n  operationId: createTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calendars\n  method: get\n  operationId: listCalendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contentnetwork/items\n  method: get\n  operationId: listContentItems\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contentnetwork/items\n  method: post\n  operationId: publishContentItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contentnetwork/items/{itemId}\n  method: get\n  operationId: getContentItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contentnetwork/items/{itemId}\n  method: delete\n  operationId: deleteContentItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contentnetwork/items/{itemId}/import\n  method: post\n  operationId: importContentItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /administration/Namespaces\n  method: get\n  operationId: listNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /administration/Namespaces(NamespaceID='{namespaceId}')/Providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/sac/{modelId}/$metadata\n\
  \  method: get\n  operationId: getModelMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/sac/{modelId}/FactData\n  method: get\n  operationId: getFactData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/sac/{modelId}/MasterData\n  method: get\n  operationId: getMasterDataOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/sac/{modelId}/{dimensionName}Master\n  method: get\n  operationId: getDimensionMasterData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logon/long\n  method: post\n  operationId: logon\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logoff\n  method: post\n  operationId: logoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/infostore\n  method: get\n  operationId: getInfoStoreRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/infostore/{objectId}\n  method: get\n  operationId: getInfoStoreObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/infostore/{objectId}/children\n  method: get\n  operationId: getInfoStoreChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cmsquery\n  method: get\n  operationId: executeCmsQueryGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cmsquery\n  method: post\n  operationId: executeCmsQueryPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/infostore/{documentId}/scheduleForms/now\n  method: post\n  operationId: scheduleDocumentNow\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inbox\n  method: get\n  operationId: listInboxItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/agentic-access/sap-bi-tools-agentic-access.yml
summary_line: 32 operations · 11 acting
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
---
