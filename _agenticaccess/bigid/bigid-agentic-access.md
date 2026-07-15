---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 18
api_specs:
- filename: bigid-authentication-api-openapi.yml
  format: yaml
  label: BigID Authentication API
  slug: bigid-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-authentication-api-openapi.yml
- filename: bigid-data-sources-api-openapi.yml
  format: yaml
  label: BigID Data Sources API
  slug: bigid-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-data-sources-api-openapi.yml
- filename: bigid-scans-api-openapi.yml
  format: yaml
  label: BigID Scans API
  slug: bigid-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-scans-api-openapi.yml
- filename: bigid-data-catalog-api-openapi.yml
  format: yaml
  label: BigID Data Catalog API
  slug: bigid-data-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-data-catalog-api-openapi.yml
- filename: bigid-cluster-analysis-api-openapi.yml
  format: yaml
  label: BigID Cluster Analysis API
  slug: bigid-cluster-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-cluster-analysis-api-openapi.yml
- filename: bigid-data-posture-api-openapi.yml
  format: yaml
  label: BigID Data Posture API
  slug: bigid-data-posture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-data-posture-api-openapi.yml
- filename: bigid-dsar-api-openapi.yml
  format: yaml
  label: BigID DSAR API
  slug: bigid-dsar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/openapi/bigid-dsar-api-openapi.yml
consequence_counts:
  read: 18
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bigid Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'BigID exposes 27 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BigID
provider_slug: bigid
slug: bigid-agentic-access
source_filename: bigid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bigid-authentication-api-openapi.yml, openapi/bigid-cluster-analysis-api-openapi.yml,\n  openapi/bigid-data-catalog-api-openapi.yml, openapi/bigid-data-posture-api-openapi.yml, openapi/bigid-data-sources-api-openapi.yml,\n  openapi/bigid-dsar-api-openapi.yml, openapi/bigid-scans-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 9\n    connected: 18\n  by_consequence:\n    write: 9\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refresh-access-token\n  method: post\n  operationId: refreshAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters\n  method: get\n  operationId: listClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-catalog\n  method: get\n  operationId: queryDataCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-catalog/object-details/columns\n  method: get\n  operationId:\
  \ getCatalogObjectColumns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-catalog/object-details/attributes\n  method: get\n  operationId: getCatalogObjectAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-catalog/column/cluster/similar\n  method: get\n  operationId: listSimilarClusterColumns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actionable-insights/all-cases\n  method: get\n  operationId: listActionableInsightsCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actionable-insights/cases:{actionType}\n  method: patch\n  operationId:\
  \ bulkUpdateActionableInsightsCases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actionable-insights/case-status/{caseId}\n  method: patch\n  operationId: updateActionableInsightsCaseStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ds-connections\n  method: get\n  operationId: listDataSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ds_connections\n  method: post\n  operationId: createDataSource\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ds-connection-test\n  method: post\n  operationId: testDataSourceConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ds-connections/file-download/export\n  method: get\n  operationId: exportDataSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ds-templates\n  method: get\n  operationId: listConnectorTemplates\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ds-templates/{type}\n  method: get\n  operationId: getConnectorTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sar/profiles\n  method: get\n  operationId: listDsarProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sar/attributes\n  method: get\n  operationId: listDsarAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sar/reports\n  method: post\n  operationId: createDsarReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sar/reports/{requestId}/status\n  method: get\n  operationId: getDsarReportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sar/reports/{requestId}/short-report\n  method: get\n  operationId: getDsarShortReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scanProfiles\n  method: post\n  operationId: createScanProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scanProfiles/{id}\n  method: get\n  operationId:\
  \ getScanProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans\n  method: get\n  operationId: listScans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans\n  method: post\n  operationId: startScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scans/parent-scans\n  method: get\n  operationId: listParentScans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{scan_id}/status\n  method: get\n  operationId: getScanStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/agentic-access/bigid-agentic-access.yml
summary_line: 27 operations · 9 acting
tags:
- Data Security
- DSPM
- DLP
- Privacy
- AI Security
- Data Catalog
- DSAR
- Data Discovery
- Compliance
---
