---
acting_count: 257
action_class_counts:
  acting: 257
  connected: 212
api_specs:
- filename: macrometa-gdn-openapi-original.json
  format: json
  label: Macrometa Global Data Network (GDN) API
  slug: macrometa-global-data-network-gdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-gdn-openapi-original.json
- filename: macrometa-photoniq-eds-openapi-original.json
  format: json
  label: PhotonIQ Event Delivery Service (EDS) API
  slug: photoniq-event-delivery-service-eds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-eds-openapi-original.json
- filename: macrometa-photoniq-est-openapi-original.json
  format: json
  label: PhotonIQ Edge Side Tagging (EST) API
  slug: photoniq-edge-side-tagging-est-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-est-openapi-original.json
- filename: macrometa-photoniq-faas-openapi-original.json
  format: json
  label: PhotonIQ Function as a Service (FaaS) API
  slug: photoniq-function-as-a-service-faas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-faas-openapi-original.json
- filename: macrometa-photoniq-fps-openapi-original.json
  format: json
  label: PhotonIQ Fingerprint (FPS) API
  slug: photoniq-fingerprint-fps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-fps-openapi-original.json
- filename: macrometa-photoniq-hss-openapi-original.json
  format: json
  label: PhotonIQ HyperSearch (HSS) API
  slug: photoniq-hypersearch-hss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-hss-openapi-original.json
- filename: macrometa-photoniq-prerender-openapi-original.json
  format: json
  label: PhotonIQ Prerender Service API
  slug: photoniq-prerender-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-prerender-openapi-original.json
- filename: macrometa-photoniq-vwrs-openapi-original.json
  format: json
  label: PhotonIQ Virtual Waiting Rooms (VWRS) API
  slug: photoniq-virtual-waiting-rooms-vwrs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-vwrs-openapi-original.json
consequence_counts:
  physical: 8
  read: 212
  safety-critical: 9
  write: 240
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 9
kind: agentic-access
layout: agentic-access
method: generated
name: Macrometa Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /_api/features/tenant/{tenant}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /_api/limits/defaults
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /_api/limits/plan/{attribution}/{name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /_api/limits/tenant/{tenant}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /_api/tenant/{tenant}/fabric/{fabric}/accept-local-collections-updates
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /_api/tenant/{tenant}/fabric/{fabric}/publish-local-collections
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /_fabric/{fabric}/_api/kms/managedkey/{id}/enable/{enable}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /_fabric/{fabric}/_api/streamapps/{appname}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /_fabric/{fabric}/_api/streamapps/{appname}/active
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /_api/_admin/_billing/usage/report
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /_api/billing/paymentsettings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /_fabric/{fabric}/_api/function/generate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /_fabric/{fabric}/_api/function/generate/publisher
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /_fabric/{fabric}/_api/function/generate/query
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /_fabric/{fabric}/_api/streamapps
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /_fabric/{fabric}/_api/streamapps/{appname}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/faas/v1/deploy
operation_count: 469
overview: 'Macrometa exposes 469 API operations that an AI agent could call, of which 257 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 212 read, 240 write, 8 physical, and 9 safety-critical.


  9 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Macrometa
provider_slug: macrometa
slug: macrometa-agentic-access
source_filename: macrometa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/macrometa-gdn-openapi-original.json, openapi/macrometa-photoniq-eds-openapi-original.json,\n  openapi/macrometa-photoniq-est-openapi-original.json, openapi/macrometa-photoniq-faas-openapi-original.json,\n  openapi/macrometa-photoniq-fps-openapi-original.json, openapi/macrometa-photoniq-hss-openapi-original.json,\n  openapi/macrometa-photoniq-prerender-openapi-original.json, openapi/macrometa-photoniq-vwrs-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 469\n  by_action_class:\n    acting: 257\n    connected: 212\n  by_consequence:\n    write: 240\n    read: 212\n    physical: 8\n    safety-critical: 9\n  human_in_the_loop_required: 9\noperations:\n- path: /_api/key/validate\n\
  \  method: post\n  operationId: ValidateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key\n  method: post\n  operationId: CreateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key\n  method: get\n  operationId: ListAvailableApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}\n  method: get\n  operationId: GetAvailableApiKey\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}\n  method: delete\n  operationId: RemoveApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database\n  method: get\n  operationId: ListTheAccessibleDatabasesForApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/database/{dbname}\n  method: get\n  operationId: GetTheDatabaseAccessLevelForApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/database/{dbname}\n\
  \  method: delete\n  operationId: ClearTheDatabaseAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database/{dbname}\n  method: put\n  operationId: SetTheDatabaseAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database/{dbname}/collection\n  method: get\n  operationId: GetTheApiKeyCollectionsAccessLevel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /_api/key/{keyid}/database/{dbname}/collection/{collection}\n  method: get\n  operationId: GetTheSpecificCollectionAccessLevelForApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/database/{dbname}/collection/{collection}\n  method: delete\n  operationId: ClearTheCollectionAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database/{dbname}/collection/{collection}\n  method: put\n  operationId: SetTheCollectionAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database/{dbname}/stream\n  method: get\n  operationId: ListTheAccessibleStreamsForApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/database/{dbname}/stream/{stream}\n  method: get\n  operationId: GetTheStreamAccessLevelForApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/database/{dbname}/stream/{stream}\n  method: delete\n  operationId: ClearTheStreamAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database/{dbname}/stream/{stream}\n  method: put\n  operationId: SetTheStreamAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database/{geofabric}/restql\n  method: get\n  operationId: GetApiKeyQueryWorkerAccessLevel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/database/{geofabric}/restql/{query-worker}\n  method: get\n  operationId: GetSpecificQueryWorkerAccessLevelForApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /_api/key/{keyid}/database/{geofabric}/restql/{query-worker}\n  method: delete\n  operationId: ClearQueryWorkerAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database/{geofabric}/restql/{query-worker}\n  method: put\n  operationId: SetQueryWorkerAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database/{geofabric}/managedkey\n  method: get\n  operationId: GetApiKeyManagedKeyAccessLevel\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/database/{geofabric}/managedkey/{managed-key-name}\n  method: get\n  operationId: GetSpecificManagedKeyAccessLevelForApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/database/{geofabric}/managedkey/{managed-key-name}\n  method: delete\n  operationId: ClearManagedKeyAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/database/{geofabric}/managedkey/{managed-key-name}\n  method: put\n  operationId: SetManagedKeyAccessLevelForApiKey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/billing\n  method: get\n  operationId: GetTheBillingAccessLevelForApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/billing\n  method: delete\n  operationId: ClearTheBillingAccessLevelForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/billing\n  method: put\n  operationId: SetTheBillingAccessLevelForApiKey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/attributes\n  method: get\n  operationId: GetTheAttributesForApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_api/key/{keyid}/attributes\n  method: put\n  operationId: UpdateTheAttributesForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/attributes/truncate\n  method: delete\n  operationId: ClearAllAttributesForApiKey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/key/{keyid}/attributes/{attributeid}\n  method: delete\n  operationId: ClearTheAttributesForApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_open/auth\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/kv/{collection}/count\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/kv/{collection}/keys\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/kv\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/kv/{collection}\n  method: post\n  operationId: CreateNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/kv/{collection}\n  method:\
  \ delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/kv/{collection}/value/{key}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/kv/{collection}/value/{key}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/kv/{collection}/values\n  method: post\n  operationId: GetValues\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/kv/{collection}/values\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/kv/{collection}/value\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/kv/{collection}/truncate\n  method: put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_api/dynamo\n  method: post\n  operationId: DynamoLikeInterfaceAPI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/redis/{collection}\n  method: post\n  operationId: RedisPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /_fabric/{fabric}/_api/redis/{collection}/{command}\n  method: get\n  operationId: RedisGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/document/{collection}\n  method: delete\n  operationId: removeDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/document/{collection}\n  method: patch\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /_fabric/{fabric}/_api/document/{collection}\n  method: post\n  operationId: insertDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/document/{collection}\n  method: put\n  operationId: replaceDocument:multiple\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/document/{collection}/{key}\n  method: delete\n  operationId: removeDocument2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/document/{collection}/{key}\n  method: get\n  operationId: readDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/document/{collection}/{key}\n  method: head\n  operationId: checkDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/document/{collection}/{key}\n  method: patch\n  operationId: updateDocument2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/document/{collection}/{key}\n  method: put\n  operationId: replaceDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/collection\n  method: get\n  operationId: handleCommandGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/collection\n  method: post\n  operationId: handleCommandPost:CreateCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/collection/{collection-name}\n  method: delete\n  operationId: handleCommandDelete:collection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/collection/{collection-name}\n  method: get\n  operationId: handleCommandGet:collectionGetProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/collection/{collection-name}/workflows\n  method: get\n  operationId: getWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/collection/{collection-name}/workflows\n\
  \  method: post\n  operationId: createWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/collection/{collection-name}/workflows/{workflow-name}\n  method: delete\n  operationId: deleteWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/collection/{collection-name}/metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /_fabric/{fabric}/_api/collection/{collection-name}/metadata\n  method: put\n  operationId: updateMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/collection/{collection-name}/reload\n  method: put\n  operationId: reloadCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/collection/{collection-name}/count\n  method: get\n  operationId: handleCommandGet:getCollectionCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/collection/{collection-name}/figures\n  method: get\n  operationId: handleCommandGet:collectionFigures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/collection/{collection-name}/truncate\n  method: put\n  operationId: handleCommandPut:truncateCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/collection/{collection-name}/properties\n  method: put\n  operationId: handleCommandPut:modifyProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/function\n  method: get\n  operationId: ListAllFunctionWorkerByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/function/generate\n  method: post\n  operationId: GenerateFunctionWorkerFromQueryWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/function/generate/publisher\n  method: post\n  operationId: GenerateFunctionWorkerFromStreamPublisher\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/function/generate/query\n  method: post\n  operationId: GenerateFunctionWorkerFromStreamQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/function/{fx-name}\n  method: get\n  operationId: GetFunctionWorkerByFunctionName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/function/{fx-name}\n  method: delete\n  operationId: DeleteFunctionWorkerByFunctionName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/function/invoke/{fx-name}\n  method: post\n  operationId: InvokeFunctionWorkerByFunctionName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/function/metadata\n  method: get\n  operationId: GetFunctionWorkerMetadata\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/function/metadata\n  method: put\n  operationId: ModifyFunctionWorkerMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/function/metadata\n  method: post\n  operationId: UpdateFunctionWorkerMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/function/metadata\n  method: delete\n  operationId: RemoveFunctionWorkerMetadata\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/cursor\n  method: post\n  operationId: createQueryCursor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/cursor/sql\n  method: post\n  operationId: createSqlQueryCursor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /_fabric/{fabric}/_api/cursor/{cursor-identifier}\n  method: delete\n  operationId: deleteQueryCursor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/cursor/{cursor-identifier}\n  method: put\n  operationId: modifyQueryCursor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/query\n  method: post\n  operationId: parseQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/query/explain\n  method: post\n  operationId: explainQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/restql\n  method: post\n  operationId: SaveRestqlByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/restql/import\n  method: post\n  operationId: ImportCustomRestQL\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/restql/execute/{name}\n  method: post\n  operationId: ExecuteRestqlByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/restql/fetch/{id}\n  method: put\n  operationId: fetchRestqlCursor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/restql/user\n\
  \  method: get\n  operationId: ListRestqlAssociatedWithCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/restql/{name}\n  method: delete\n  operationId: DeleteRestqlByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/restql/{name}\n  method: put\n  operationId: UpdateRestqlByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/index\n\
  \  method: get\n  operationId: getIndexes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /_fabric/{fabric}/_api/index/fulltext\n  method: post\n  operationId: createIndex:fulltext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/index/general\n  method: post\n  operationId: createIndex:general\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /_fabric/{fabric}/_api/index/g\n\n# --- truncated at\
  \ 32 KB (138 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/agentic-access/macrometa-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/agentic-access/macrometa-agentic-access.yml
summary_line: 469 operations · 257 acting · 9 human-in-the-loop
tags:
- Company
- Infrastructure
- Edge Computing
- Database
- NoSQL
- Serverless
- Streaming
- Stream Processing
- Real Time
- Web Performance
- CDN
- Search
- Artificial Intelligence
- API
---
