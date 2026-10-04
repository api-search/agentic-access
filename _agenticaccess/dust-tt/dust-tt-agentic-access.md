---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 33
api_specs:
- filename: dust-tt-agents-api-openapi.yml
  format: yaml
  label: Dust Agents API
  slug: dust-tt-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-agents-api-openapi.yml
- filename: dust-tt-apps-api-openapi.yml
  format: yaml
  label: Dust Apps API
  slug: dust-tt-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-apps-api-openapi.yml
- filename: dust-tt-conversations-api-openapi.yml
  format: yaml
  label: Dust Conversations API
  slug: dust-tt-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-conversations-api-openapi.yml
- filename: dust-tt-datasourceviews-api-openapi.yml
  format: yaml
  label: Dust DatasourceViews API
  slug: dust-tt-datasourceviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-datasourceviews-api-openapi.yml
- filename: dust-tt-feedbacks-api-openapi.yml
  format: yaml
  label: Dust Feedbacks API
  slug: dust-tt-feedbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-feedbacks-api-openapi.yml
- filename: dust-tt-mcp-api-openapi.yml
  format: yaml
  label: Dust MCP API
  slug: dust-tt-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-mcp-api-openapi.yml
- filename: dust-tt-mentions-api-openapi.yml
  format: yaml
  label: Dust Mentions API
  slug: dust-tt-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-mentions-api-openapi.yml
- filename: dust-tt-search-api-openapi.yml
  format: yaml
  label: Dust Search API
  slug: dust-tt-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-search-api-openapi.yml
- filename: dust-tt-skills-api-openapi.yml
  format: yaml
  label: Dust Skills API
  slug: dust-tt-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-skills-api-openapi.yml
- filename: dust-tt-spaces-api-openapi.yml
  format: yaml
  label: Dust Spaces API
  slug: dust-tt-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-spaces-api-openapi.yml
- filename: dust-tt-tools-api-openapi.yml
  format: yaml
  label: Dust Tools API
  slug: dust-tt-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-tools-api-openapi.yml
- filename: dust-tt-triggers-api-openapi.yml
  format: yaml
  label: Dust Triggers API
  slug: dust-tt-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-triggers-api-openapi.yml
- filename: dust-tt-workspace-api-openapi.yml
  format: yaml
  label: Dust Workspace API
  slug: dust-tt-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-workspace-api-openapi.yml
- filename: dust-tt-data-sources-api-openapi.yml
  format: yaml
  label: Dust Data Sources API
  slug: dust-tt-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/openapi/dust-tt-data-sources-api-openapi.yml
consequence_counts:
  read: 33
  safety-critical: 1
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Dust Tt Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/w/{wId}/skills
operation_count: 64
overview: 'Dust exposes 64 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read, 30 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dust
provider_slug: dust-tt
slug: dust-tt-agentic-access
source_filename: dust-tt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/dust-tt-agents-api-openapi.yml, openapi/dust-tt-apps-api-openapi.yml, openapi/dust-tt-conversations-api-openapi.yml,\n  openapi/dust-tt-data-sources-api-openapi.yml, openapi/dust-tt-datasourceviews-api-openapi.yml,\n  openapi/dust-tt-feedbacks-api-openapi.yml, openapi/dust-tt-mcp-api-openapi.yml, openapi/dust-tt-mentions-api-openapi.yml,\n  openapi/dust-tt-search-api-openapi.yml, openapi/dust-tt-skills-api-openapi.yml, openapi/dust-tt-spaces-api-openapi.yml,\n  openapi/dust-tt-tools-api-openapi.yml, openapi/dust-tt-triggers-api-openapi.yml, openapi/dust-tt-workspace-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 64\n  by_action_class:\n    connected: 33\n    acting:\
  \ 31\n  by_consequence:\n    read: 33\n    write: 30\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/w/{wId}/assistant/agent_configurations\n  method: get\n  operationId: getApiV1WByWIdAssistantAgentConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/agent_configurations/{sId}/export/yaml\n  method: get\n  operationId: getApiV1WByWIdAssistantAgentConfigurationsBySIdExportYaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/agent_configurations/{sId}\n  method: get\n  operationId: getApiV1WByWIdAssistantAgentConfigurationsBySId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/w/{wId}/assistant/agent_configurations/{sId}\n  method: patch\n  operationId: patchApiV1WByWIdAssistantAgentConfigurationsBySId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/agent_configurations/{sId}\n  method: delete\n  operationId: deleteApiV1WByWIdAssistantAgentConfigurationsBySId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/agent_configurations/import\n  method: post\n  operationId: postApiV1WByWIdAssistantAgentConfigurationsImport\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/agent_configurations/search\n  method: get\n  operationId: getApiV1WByWIdAssistantAgentConfigurationsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/apps/{aId}/runs/{runId}\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdAppsByAIdRunsByRunId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/apps/{aId}/runs\n  method: post\n  operationId: postApiV1WByWIdSpacesBySpaceIdAppsByAIdRuns\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/apps\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/cancel\n  method: post\n  operationId: postApiV1WByWIdAssistantConversationsByCIdCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/content_fragments\n  method:\
  \ post\n  operationId: postApiV1WByWIdAssistantConversationsByCIdContentFragments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/events\n  method: get\n  operationId: getApiV1WByWIdAssistantConversationsByCIdEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/files/{rel}\n  method: get\n  operationId: getApiV1WByWIdAssistantConversationsByCIdFilesByRel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}\n \
  \ method: get\n  operationId: getApiV1WByWIdAssistantConversationsByCId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}\n  method: patch\n  operationId: patchApiV1WByWIdAssistantConversationsByCId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/messages/{mId}/answer-question\n  method: post\n  operationId: postApiV1WByWIdAssistantConversationsByCIdMessagesByMIdAnswerQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/messages/{mId}/edit\n  method: post\n  operationId: postApiV1WByWIdAssistantConversationsByCIdMessagesByMIdEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/messages/{mId}/events\n  method: get\n  operationId: getApiV1WByWIdAssistantConversationsByCIdMessagesByMIdEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/messages/{mId}/validate-action\n  method: post\n  operationId: postApiV1WByWIdAssistantConversationsByCIdMessagesByMIdValidateAction\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/messages\n  method: post\n  operationId: postApiV1WByWIdAssistantConversationsByCIdMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/conversations\n  method: post\n  operationId: postApiV1WByWIdAssistantConversations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/files\n  method: post\n  operationId: postApiV1WByWIdFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/check_upsert_queue\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdCheckUpsertQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/documents/{documentId}\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdDocumentsByDocumentId\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/documents/{documentId}\n  method: post\n  operationId: postApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdDocumentsByDocumentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/documents/{documentId}\n  method: delete\n  operationId: deleteApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdDocumentsByDocumentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/documents/{documentId}/parents\n  method: post\n  operationId: postApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdDocumentsByDocumentIdParents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/documents\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/search\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdSearch\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/tables/{tId}\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdTablesByTId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/tables/{tId}\n  method: delete\n  operationId: deleteApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdTablesByTId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/tables/{tId}/rows/{rId}\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdTablesByTIdRowsByRId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/tables/{tId}/rows/{rId}\n  method: delete\n  operationId: deleteApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdTablesByTIdRowsByRId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/tables/{tId}/rows\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdTablesByTIdRows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/tables/{tId}/rows\n\
  \  method: post\n  operationId: postApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdTablesByTIdRows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/tables\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources/{dsId}/tables\n  method: post\n  operationId: postApiV1WByWIdSpacesBySpaceIdDataSourcesByDsIdTables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_sources\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_source_views/{dsvId}\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourceViewsByDsvId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_source_views/{dsvId}\n  method: patch\n  operationId: patchApiV1WByWIdSpacesBySpaceIdDataSourceViewsByDsvId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_source_views/{dsvId}\n  method: delete\n  operationId: deleteApiV1WByWIdSpacesBySpaceIdDataSourceViewsByDsvId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_source_views/{dsvId}/search\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourceViewsByDsvIdSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/data_source_views\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdDataSourceViews\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/feedbacks\n  method: get\n  operationId: getApiV1WByWIdAssistantConversationsByCIdFeedbacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/messages/{mId}/feedbacks\n  method: post\n  operationId: postApiV1WByWIdAssistantConversationsByCIdMessagesByMIdFeedbacks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/messages/{mId}/feedbacks\n  method: delete\n  operationId: deleteApiV1WByWIdAssistantConversationsByCIdMessagesByMIdFeedbacks\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/mcp/heartbeat\n  method: post\n  operationId: postApiV1WByWIdMcpHeartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/mcp/register\n  method: post\n  operationId: postApiV1WByWIdMcpRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/w/{wId}/mcp/requests\n  method: get\n  operationId: getApiV1WByWIdMcpRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/mcp/results\n  method: post\n  operationId: postApiV1WByWIdMcpResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/conversations/{cId}/mentions/suggestions\n  method: get\n  operationId: getApiV1WByWIdAssistantConversationsByCIdMentionsSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/assistant/mentions/parse\n\
  \  method: post\n  operationId: postApiV1WByWIdAssistantMentionsParse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/assistant/mentions/suggestions\n  method: get\n  operationId: getApiV1WByWIdAssistantMentionsSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/search\n  method: get\n  operationId: getApiV1WByWIdSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/search\n  method: post\n  operationId: postApiV1WByWIdSearch\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/search/tools/upload\n  method: post\n  operationId: postApiV1WByWIdSearchToolsUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/w/{wId}/skills\n  method: get\n  operationId: getApiV1WByWIdSkills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/skills\n  method: post\n  operationId: postApiV1WByWIdSkills\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/w/{wId}/spaces\n  method: get\n  operationId: getApiV1WByWIdSpaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/spaces/{spaceId}/mcp_server_views\n  method: get\n  operationId: getApiV1WByWIdSpacesBySpaceIdMcpServerViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/triggers/hooks/{webhookSourceId}\n  method: post\n  operationId: postApiV1WByWIdTriggersHooksByWebhookSourceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/w/{wId}/analytics/export\n  method: get\n  operationId: getApiV1WByWIdAnalyticsExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/w/{wId}/workspace-usage\n  method: get\n  operationId: getApiV1WByWIdWorkspaceUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dust-tt/refs/heads/main/agentic-access/dust-tt-agentic-access.yml
summary_line: 64 operations · 31 acting · 1 human-in-the-loop
tags:
- Agents
- Artificial Intelligence
- Custom Workflows
- Data Sources
- Dust
- Enterprise AI
- Knowledge Management
- LLM
- MCP
- Multi-Model
- RAG
---
