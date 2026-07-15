---
acting_count: 43
action_class_counts:
  acting: 43
  connected: 35
api_specs:
- filename: postman-webhooks-asyncapi.yml
  format: yaml
  label: Postman
  slug: postman
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/asyncapi/postman-webhooks-asyncapi.yml
- filename: postman-collections-api-openapi.yml
  format: yaml
  label: Postman Collections API
  slug: collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-collections-api-openapi.yml
- filename: postman-workspaces-api-openapi.yml
  format: yaml
  label: Postman Workspaces API
  slug: workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-workspaces-api-openapi.yml
- filename: postman-environments-api-openapi.yml
  format: yaml
  label: Postman Environments API
  slug: environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-environments-api-openapi.yml
- filename: postman-mock-servers-api-openapi.yml
  format: yaml
  label: Postman Mock Servers API
  slug: mock-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-mock-servers-api-openapi.yml
- filename: postman-monitors-api-openapi.yml
  format: yaml
  label: Postman Monitors API
  slug: monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-monitors-api-openapi.yml
- filename: postman-apis-api-openapi.yml
  format: yaml
  label: Postman APIs / Spec Hub API
  slug: apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-apis-api-openapi.yml
- filename: postman-private-api-network-api-openapi.yml
  format: yaml
  label: Postman Private API Network API
  slug: private-api-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-private-api-network-api-openapi.yml
- filename: postman-webhooks-api-openapi.yml
  format: yaml
  label: Postman Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-webhooks-api-openapi.yml
- filename: postman-collection-runs-api-openapi.yml
  format: yaml
  label: Postman Collection Runs API
  slug: collection-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-collection-runs-api-openapi.yml
- filename: postman-tags-api-openapi.yml
  format: yaml
  label: Postman Tags API
  slug: tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-tags-api-openapi.yml
- filename: postman-audit-logs-api-openapi.yml
  format: yaml
  label: Postman Audit Logs API
  slug: audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-audit-logs-api-openapi.yml
- filename: postman-secret-scanner-api-openapi.yml
  format: yaml
  label: Postman Secret Scanner API
  slug: secret-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/openapi/postman-secret-scanner-api-openapi.yml
consequence_counts:
  read: 35
  write: 43
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Postman Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 78
overview: 'Postman exposes 78 API operations that an AI agent could call, of which 43 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read and 43 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Postman
provider_slug: postman
slug: postman-agentic-access
source_filename: postman-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/postman-apis-api-openapi.yml, openapi/postman-audit-logs-api-openapi.yml, openapi/postman-collection-runs-api-openapi.yml,\n  openapi/postman-collections-api-openapi.yml, openapi/postman-environments-api-openapi.yml,\n  openapi/postman-mock-servers-api-openapi.yml, openapi/postman-monitors-api-openapi.yml, openapi/postman-private-api-network-api-openapi.yml,\n  openapi/postman-secret-scanner-api-openapi.yml, openapi/postman-tags-api-openapi.yml, openapi/postman-webhooks-api-openapi.yml,\n  openapi/postman-workspaces-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 78\n  by_action_class:\n    connected: 35\n    acting: 43\n  by_consequence:\n    read: 35\n    write: 43\n\
  \  human_in_the_loop_required: 0\noperations:\n- path: /apis\n  method: get\n  operationId: getAllApis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis\n  method: post\n  operationId: createApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/{apiId}\n  method: get\n  operationId: getApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/{apiId}\n  method: put\n  operationId: updateApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/{apiId}\n  method: delete\n  operationId: deleteApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/{apiId}/versions\n  method: get\n  operationId: getApiVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/{apiId}/versions\n  method: post\n  operationId: createApiVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /apis/{apiId}/versions/{versionId}\n  method: get\n  operationId: getApiVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/{apiId}/versions/{versionId}\n  method: put\n  operationId: updateApiVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/{apiId}/versions/{versionId}\n  method: delete\n  operationId: deleteApiVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /apis/{apiId}/schemas\n  method: get\n  operationId: getApiSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/{apiId}/schemas\n  method: post\n  operationId: createApiSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/{apiId}/schemas/{schemaId}\n  method: get\n  operationId: getApiSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/{apiId}/schemas/{schemaId}/files\n  method: get\n  operationId: getApiSchemaFiles\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/{apiId}/comments\n  method: get\n  operationId: getApiComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/{apiId}/comments\n  method: post\n  operationId: createApiComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audit/logs\n  method: get\n  operationId: getAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/runs\n  method: get\n  operationId: getCollectionRuns\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/runs/{runId}\n  method: get\n  operationId: getCollectionRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: getAllCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collectionId}\n  method: get\n  operationId: getCollection\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}\n  method: put\n  operationId: updateCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collectionId}\n  method: delete\n  operationId: deleteCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collectionId}/requests\n  method: get\n  operationId: getCollectionRequests\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/folders\n  method: get\n  operationId: getCollectionFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/responses\n  method: get\n  operationId: getCollectionResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/fork/{collectionId}\n  method: post\n  operationId: forkCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/merge\n  method:\
  \ post\n  operationId: mergeCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments\n  method: get\n  operationId: getAllEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments\n  method: post\n  operationId: createEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}\n  method: get\n  operationId: getEnvironment\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}\n  method: put\n  operationId: updateEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}\n  method: delete\n  operationId: deleteEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mocks\n  method: get\n  operationId: getAllMocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /mocks\n  method: post\n  operationId: createMock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mocks/{mockId}\n  method: get\n  operationId: getMock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mocks/{mockId}\n  method: put\n  operationId: updateMock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mocks/{mockId}\n  method: delete\n  operationId: deleteMock\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mocks/{mockId}/publish\n  method: post\n  operationId: publishMock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mocks/{mockId}/unpublish\n  method: delete\n  operationId: unpublishMock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /mocks/{mockId}/serverResponses\n  method: get\n  operationId: getMockServerResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mocks/{mockId}/serverResponses\n  method: post\n  operationId: createServerResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mocks/{mockId}/serverResponses/{serverResponseId}\n  method: put\n  operationId: updateServerResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /mocks/{mockId}/serverResponses/{serverResponseId}\n  method: delete\n  operationId: deleteServerResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mocks/{mockId}/call-logs\n  method: get\n  operationId: getMockCallLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors\n  method: get\n  operationId: getAllMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors\n  method: post\n  operationId: createMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/{monitorId}\n  method: get\n  operationId: getMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitors/{monitorId}\n  method: put\n  operationId: updateMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/{monitorId}\n  method: delete\n  operationId: deleteMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitors/{monitorId}/run\n  method: post\n  operationId: runMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/private\n  method: get\n  operationId: getPrivateNetworkElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/private\n  method: post\n  operationId: addNetworkElement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /network/private/{elementType}/{elementId}\n  method: put\n  operationId: updateNetworkElement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/private/{elementType}/{elementId}\n  method: delete\n  operationId: removeNetworkElement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/private/network-folder\n  method: get\n  operationId: getNetworkFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /network/private/network-folder\n  method: post\n  operationId: createNetworkFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/private/network-folder/{folderId}\n  method: put\n  operationId: updateNetworkFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/private/network-folder/{folderId}\n  method: delete\n  operationId: deleteNetworkFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/private/network-request\n  method: get\n  operationId: getNetworkRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/private/network-request/{requestId}/approve\n  method: put\n  operationId: approveNetworkRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/private/network-request/{requestId}/deny\n  method: put\n  operationId: denyNetworkRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /secret-scanner/detected-secrets\n  method: get\n  operationId: getDetectedSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secret-scanner/detected-secrets/{secretId}\n  method: get\n  operationId: getDetectedSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secret-scanner/detected-secrets/{secretId}\n  method: put\n  operationId: resolveDetectedSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /secret-scanner/detected-secrets/{secretId}/locations\n  method: get\n  operationId: getSecretLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /secret-scanner/secret-types\n  method: get\n  operationId: getSecretTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{entityType}/{entityId}\n  method: get\n  operationId: getEntityTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{entityType}/{entityId}\n  method: put\n  operationId: updateEntityTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces\n  method: get\n  operationId: getAllWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /workspaces/{workspaceId}\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}\n  method: put\n  operationId: updateWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}\n  method: delete\n  operationId: deleteWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/global-variables\n\
  \  method: get\n  operationId: getWorkspaceGlobalVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/global-variables\n  method: put\n  operationId: updateWorkspaceGlobalVariables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/agentic-access/postman-agentic-access.yml
summary_line: 78 operations · 43 acting
tags:
- AI Agent Builder
- AI Agents
- API Catalog
- API Client
- API Design
- API Development
- API Documentation
- API Governance
- API Lifecycle
- API Monitoring
- API Network
- API Platform
- API Testing
- Audit Logs
- Automation
- CI/CD
- Collaboration
- Collections
- Compliance
- Discovery
- Environments
- Flows
- GraphQL
- gRPC
- HTTP
- Insights
- MCP
- MCP Generator
- Mock Servers
- Mocking
- Monitors
- Newman
- OpenAPI
- Platform
- Private API Network
- Public API Network
- Secret Scanning
- Spec Hub
- Specifications
- SSO
- Testing
- Vault
- WebSocket
- Workflows
- Workspaces
---
