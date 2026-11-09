---
acting_count: 36
action_class_counts:
  acting: 36
  connected: 32
api_specs:
- filename: past-dev-audiences-api-openapi.yml
  format: yaml
  label: past-dev Audiences API
  slug: past-dev-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-audiences-api-openapi.yml
- filename: past-dev-debugging-api-openapi.yml
  format: yaml
  label: past-dev Debugging API
  slug: past-dev-debugging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-debugging-api-openapi.yml
- filename: past-dev-identities-api-openapi.yml
  format: yaml
  label: past-dev Identities API
  slug: past-dev-identities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-identities-api-openapi.yml
- filename: past-dev-ingestion-api-openapi.yml
  format: yaml
  label: past-dev Ingestion API
  slug: past-dev-ingestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-ingestion-api-openapi.yml
- filename: past-dev-management-api-openapi.yml
  format: yaml
  label: past-dev Management API
  slug: past-dev-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-management-api-openapi.yml
- filename: past-dev-recall-api-openapi.yml
  format: yaml
  label: past-dev Recall API
  slug: past-dev-recall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-recall-api-openapi.yml
- filename: past-dev-webhooks-api-openapi.yml
  format: yaml
  label: past-dev Webhooks API
  slug: past-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 32
  safety-critical: 4
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Past Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/ingest/{ingestionId}/retry
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/ingest/{ingestionId}/retry
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/projects/{slug}/keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/projects/{slug}/keys/{keyId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/ingest/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/ingest/batch
operation_count: 68
overview: 'past-dev exposes 68 API operations that an AI agent could call, of which 36 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 30 write, 2 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: past-dev
provider_slug: past-dev
slug: past-dev-agentic-access
source_filename: past-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/past-dev-openapi.json, openapi/past-dev.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 68\n  by_action_class:\n    acting: 36\n    connected: 32\n  by_consequence:\n    write: 30\n    physical: 2\n    read: 32\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /api/v1/ingest\n  method: post\n  operationId: ingest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ingest/batch\n \
  \ method: post\n  operationId: ingestBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ingest/{ingestionId}\n  method: get\n  operationId: getIngestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ingest/{ingestionId}\n  method: delete\n  operationId: deleteIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recall\n  method: post\n  operationId: recall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/identities/{identity}\n  method: put\n  operationId: upsertIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identities/{identity}\n  method: patch\n  operationId: patchIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identities/{identity}\n  method: get\n  operationId: getIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/identities/{identity}\n  method: delete\n  operationId: deleteIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identities/bulk\n  method: post\n  operationId: bulkUpsertIdentities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identities\n  method: get\n  operationId: listIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/data-points/{sourceId}\n  method: delete\n  operationId: deleteDataPoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/data-points/delete\n  method: post\n  operationId: deleteDataPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{webhookId}/{token}\n  method: post\n  operationId: receiveWebhookEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audiences\n  method: get\n  operationId: listAudiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audiences/{slug}\n  method: get\n  operationId: getAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audiences/{slug}\n  method: put\n  operationId: putAudience\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audiences/{slug}\n  method: delete\n  operationId: deleteAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audiences/{slug}/recompute\n  method: post\n  operationId: recomputeAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/projects/{slug}/keys\n  method: post\n  operationId: createProjectKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/projects/{slug}/keys/{keyId}\n  method: delete\n  operationId:\
  \ revokeProjectKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/ingest/estimate\n  method: post\n  operationId: estimateIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ingest/{ingestionId}/retry\n  method: post\n  operationId: retryIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/ingest/{ingestionId}/explain\n  method: get\n  operationId: explainIngestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/requests\n  method: get\n  operationId: listRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/requests/histogram\n  method: get\n  operationId: requestHistogram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/requests/{requestId}\n  method: get\n  operationId:\
  \ getRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trace/roots\n  method: get\n  operationId: findTraceRoots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trace/nodes/{id}\n  method: get\n  operationId: getTraceNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trace/lineage/{rootId}\n  method: get\n  operationId: getLineage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trace/timeline/{rootId}\n \
  \ method: get\n  operationId: getTimeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ingest\n  method: post\n  operationId: ingest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ingest/batch\n  method: post\n  operationId: ingestBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ingest/{ingestionId}\n  method: get\n  operationId: getIngestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ingest/{ingestionId}\n  method: delete\n  operationId: deleteIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recall\n  method: post\n  operationId: recall\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/identities/{identity}\n  method: put\n  operationId: upsertIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identities/{identity}\n  method: patch\n  operationId: patchIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identities/{identity}\n  method: get\n\
  \  operationId: getIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/identities/{identity}\n  method: delete\n  operationId: deleteIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identities/bulk\n  method: post\n  operationId: bulkUpsertIdentities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /api/v1/identities\n  method: get\n  operationId: listIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/data-points/{sourceId}\n  method: delete\n  operationId: deleteDataPoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/data-points/delete\n  method: post\n  operationId: deleteDataPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{webhookId}/{token}\n\
  \  method: post\n  operationId: receiveWebhookEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audiences\n  method: get\n  operationId: listAudiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audiences/{slug}\n  method: get\n  operationId: getAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audiences/{slug}\n  method: put\n  operationId: putAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audiences/{slug}\n  method: delete\n  operationId: deleteAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audiences/{slug}/recompute\n  method: post\n  operationId: recomputeAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/projects/{slug}/keys\n  method: post\n  operationId: createProjectKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/projects/{slug}/keys/{keyId}\n  method: delete\n  operationId: revokeProjectKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/ingest/estimate\n  method: post\n  operationId: estimateIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - memory:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ingest/{ingestionId}/retry\n  method: post\n  operationId: retryIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - memory:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /api/v1/ingest/{ingestionId}/explain\n  method: get\n  operationId: explainIngestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/requests\n  method: get\n  operationId: listRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/requests/histogram\n  method: get\n  operationId: requestHistogram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/requests/{requestId}\n  method: get\n  operationId: getRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trace/roots\n  method: get\n  operationId: findTraceRoots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trace/nodes/{id}\n  method: get\n  operationId: getTraceNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trace/lineage/{rootId}\n  method: get\n  operationId: getLineage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trace/timeline/{rootId}\n  method: get\n  operationId: getTimeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - memory:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/past-dev/agentic-access/past-dev-agentic-access.yml
summary_line: 68 operations · 36 acting · 4 human-in-the-loop
tags:
- Artificial Intelligence
- Memory
- Platform
- Developers
---
