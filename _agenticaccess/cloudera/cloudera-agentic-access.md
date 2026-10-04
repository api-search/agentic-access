---
acting_count: 556
action_class_counts:
  acting: 556
  connected: 222
api_specs:
- filename: cloudera-audit-api-openapi.yml
  format: yaml
  label: Cloudera Audit API
  slug: cloudera-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-audit-api-openapi.yml
- filename: cloudera-cdflocalrpcapiversion1-api-openapi.yml
  format: yaml
  label: Cloudera CDF Local RPCAPI Version1 API
  slug: cloudera-cdflocalrpcapiversion1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-cdflocalrpcapiversion1-api-openapi.yml
- filename: cloudera-cloudprivatelinks-api-openapi.yml
  format: yaml
  label: Cloudera Cloudprivatelinks API
  slug: cloudera-cloudprivatelinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-cloudprivatelinks-api-openapi.yml
- filename: cloudera-compute-api-openapi.yml
  format: yaml
  label: Cloudera Compute API
  slug: cloudera-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-compute-api-openapi.yml
- filename: cloudera-consumption-api-openapi.yml
  format: yaml
  label: Cloudera Consumption API
  slug: cloudera-consumption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-consumption-api-openapi.yml
- filename: cloudera-datalake-api-openapi.yml
  format: yaml
  label: Cloudera Datalake API
  slug: cloudera-datalake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-datalake-api-openapi.yml
- filename: cloudera-de-api-openapi.yml
  format: yaml
  label: Cloudera De API
  slug: cloudera-de-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-de-api-openapi.yml
- filename: cloudera-df-api-openapi.yml
  format: yaml
  label: Cloudera Df API
  slug: cloudera-df-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-df-api-openapi.yml
- filename: cloudera-drscp-api-openapi.yml
  format: yaml
  label: Cloudera Drscp API
  slug: cloudera-drscp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-drscp-api-openapi.yml
- filename: cloudera-dw-api-openapi.yml
  format: yaml
  label: Cloudera Dw API
  slug: cloudera-dw-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-dw-api-openapi.yml
- filename: cloudera-environments2-api-openapi.yml
  format: yaml
  label: Cloudera Environments2 API
  slug: cloudera-environments2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-environments2-api-openapi.yml
- filename: cloudera-iam-api-openapi.yml
  format: yaml
  label: Cloudera Iam API
  slug: cloudera-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-iam-api-openapi.yml
- filename: cloudera-imagecatalog-api-openapi.yml
  format: yaml
  label: Cloudera Imagecatalog API
  slug: cloudera-imagecatalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-imagecatalog-api-openapi.yml
- filename: cloudera-lakehouseopt-api-openapi.yml
  format: yaml
  label: Cloudera Lakehouseopt API
  slug: cloudera-lakehouseopt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-lakehouseopt-api-openapi.yml
- filename: cloudera-ml-api-openapi.yml
  format: yaml
  label: Cloudera Ml API
  slug: cloudera-ml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-ml-api-openapi.yml
- filename: cloudera-opdb-api-openapi.yml
  format: yaml
  label: Cloudera Opdb API
  slug: cloudera-opdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-opdb-api-openapi.yml
- filename: cloudera-replicationmanager-api-openapi.yml
  format: yaml
  label: Cloudera Replicationmanager API
  slug: cloudera-replicationmanager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-replicationmanager-api-openapi.yml
- filename: cloudera-data-catalog-api-openapi.yml
  format: yaml
  label: Cloudera Data Catalog API
  slug: cloudera-data-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-data-catalog-api-openapi.yml
- filename: cloudera-data-hub-api-openapi.yml
  format: yaml
  label: Cloudera Data Hub API
  slug: cloudera-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-data-hub-api-openapi.yml
consequence_counts:
  physical: 36
  read: 222
  safety-critical: 30
  write: 490
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 30
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudera Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/cloudprivatelinks/revokePrivateLinkServiceAccess
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/compute/retryOperation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/datacatalog/revokeExternalUserCredentials
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/datahub/startCluster
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/datahub/stopCluster
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/datahub/stopInstances
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/datalake/stopDatalake
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/de/disableService
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/df/disableService
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/df/resetService
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/df/revokeUserKubernetesAccess
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/drscp/createBackup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/drscp/deleteBackup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/dw/resetServerSettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/environments2/stopEnvironment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/ml/revokeMlServingAppAccess
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/ml/revokeModelRegistryAccess
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/ml/revokeWorkspaceAccess
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/opdb/stopDatabase
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/replicationmanager/suspendPolicy
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dfx/api/rpc-v1/deployed-flows/stop-flow-in-deployment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dfx/api/rpc-v1/deployed-flows/terminate-flow-in-deployment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dfx/api/rpc-v1/deployments/stop-all-flows-in-deployment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dfx/api/rpc-v1/deployments/stop-flow
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dfx/api/rpc-v1/deployments/terminate-deployment
operation_count: 778
overview: 'Cloudera exposes 778 API operations that an AI agent could call, of which 556 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 222 read, 490 write, 36 physical, and 30 safety-critical.


  30 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloudera
provider_slug: cloudera
slug: cloudera-agentic-access
source_filename: cloudera-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/cloudera-audit-api-openapi.yml, openapi/cloudera-cdflocalrpcapiversion1-api-openapi.yml,\n  openapi/cloudera-cloudprivatelinks-api-openapi.yml, openapi/cloudera-compute-api-openapi.yml,\n  openapi/cloudera-consumption-api-openapi.yml, openapi/cloudera-data-catalog-api-openapi.yml,\n  openapi/cloudera-data-hub-api-openapi.yml, openapi/cloudera-datalake-api-openapi.yml, openapi/cloudera-de-api-openapi.yml,\n  openapi/cloudera-df-api-openapi.yml, openapi/cloudera-drscp-api-openapi.yml, openapi/cloudera-dw-api-openapi.yml,\n  openapi/cloudera-environments2-api-openapi.yml, openapi/cloudera-iam-api-openapi.yml, openapi/cloudera-imagecatalog-api-openapi.yml,\n  openapi/cloudera-lakehouseopt-api-openapi.yml, openapi/cloudera-ml-api-openapi.yml, openapi/cloudera-opdb-api-openapi.yml,\n  openapi/cloudera-replicationmanager-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically\
  \ from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 778\n  by_action_class:\n    acting: 556\n    connected: 222\n  by_consequence:\n    write: 490\n    read: 222\n    physical: 36\n    safety-critical: 30\n  human_in_the_loop_required: 30\noperations:\n- path: /api/v1/audit/archiveAuditEvents\n  method: post\n  operationId: archiveAuditEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audit/batchEventsForArchiving\n  method: post\n  operationId: batchEventsForArchiving\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audit/configureArchiving\n  method: post\n  operationId: configureArchiving\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audit/getArchivingConfig\n  method: post\n  operationId: getArchivingConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/getArchivingStatus\n  method: post\n  operationId: getArchivingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/audit/getBatchEventsForArchivingStatus\n  method: post\n  operationId: getBatchEventsForArchivingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/listEvents\n  method: post\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/listEventsInArchiveBatch\n  method: post\n  operationId: listEventsInArchiveBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/listOutstandingArchiveBatches\n  method: post\n  operationId: listOutstandingArchiveBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/audit/listRecentArchiveRuns\n  method: post\n  operationId: listRecentArchiveRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audit/markArchiveBatchesAsSuccessful\n  method: post\n  operationId: markArchiveBatchesAsSuccessful\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/custom-nar-configurations/create-custom-nar-configuration\n  method: post\n  operationId: createCustomNarConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/custom-nar-configurations/delete-custom-nar-configuration\n  method: post\n  operationId: deleteCustomNarConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/custom-nar-configurations/get-custom-nar-configuration\n  method: post\n  operationId: getCustomNarConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/custom-nar-configurations/get-default-custom-nar-configuration\n  method: post\n  operationId: getDefaultCustomNarConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/custom-nar-configurations/update-custom-nar-configuration\n  method: post\n  operationId: updateCustomNarConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/custom-nar-configurations/validate-custom-nar-configuration\n  method: post\n  operationId: validateCustomNarConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/custom-python-configurations/create-custom-python-configuration\n  method:\
  \ post\n  operationId: createCustomPythonConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/custom-python-configurations/delete-custom-python-configuration\n  method: post\n  operationId: deleteCustomPythonConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/custom-python-configurations/get-custom-python-configuration\n  method: post\n  operationId: getCustomPythonConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/custom-python-configurations/update-custom-python-configuration\n  method: post\n  operationId: updateCustomPythonConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/custom-python-configurations/validate-custom-python-configuration\n  method: post\n  operationId: validateCustomPythonConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployed-flows/abort-flow-request-in-deployment\n  method: post\n\
  \  operationId: abortFlowRequestInDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployed-flows/add-flow-to-deployment\n  method: post\n  operationId: addFlowToDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployed-flows/cancel-change-flow-version-in-deployment\n  method: post\n  operationId: cancelChangeFlowVersionInDeployment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployed-flows/change-flow-version-in-deployment\n  method: post\n  operationId: changeFlowVersionInDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployed-flows/get-flow-configuration-in-deployment\n  method: post\n  operationId: getFlowConfigurationInDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/deployed-flows/get-flow-configuration-metadata-in-deployment\n  method: post\n  operationId: getFlowConfigurationMetadataInDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/deployed-flows/get-flow-request-details-in-deployment\n  method: post\n  operationId: getFlowRequestDetailsInDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/deployed-flows/import-flow-into-deployment\n  method: post\n  operationId: importFlowIntoDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployed-flows/start-flow-in-deployment\n  method: post\n  operationId: startFlowInDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployed-flows/stop-flow-in-deployment\n  method: post\n  operationId: stopFlowInDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dfx/api/rpc-v1/deployed-flows/terminate-flow-in-deployment\n\
  \  method: post\n  operationId: terminateFlowInDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dfx/api/rpc-v1/deployed-flows/update-flow-in-deployment\n  method: post\n  operationId: updateFlowInDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/abort-asset-update-request\n  method: post\n  operationId: abortAssetUpdateRequest\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/abort-deployment-request\n  method: post\n  operationId: abortDeploymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/cancel-change-flow-version\n  method: post\n  operationId: cancelChangeFlowVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/cancel-nifi-version-update\n  method: post\n  operationId: cancelNifiVersionUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/change-flow-version\n  method: post\n  operationId: changeFlowVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/create-asset-update-request\n  method: post\n  operationId: createAssetUpdateRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/create-deployment\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/create-reporting-task\n\
  \  method: post\n  operationId: createReportingTask\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/delete-reporting-task\n  method: post\n  operationId: deleteReportingTask\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/export-deployment\n  method: post\n  operationId: exportDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/get-deployment-configuration\n  method: post\n  operationId: getDeploymentConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/deployments/get-deployment-configuration-metadata\n  method: post\n  operationId: getDeploymentConfigurationMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/deployments/get-deployment-request-details\n  method: post\n  operationId: getDeploymentRequestDetails\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/deployments/import-deployment\n  method: post\n  operationId: importDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/list-deployment-archives\n  method: post\n  operationId: listDeploymentArchives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/deployments/list-reporting-tasks\n  method: post\n  operationId: listReportingTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/deployments/restart-deployment\n  method: post\n  operationId: restartDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/resume-deployment\n  method: post\n  operationId: resumeDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/start-all-flows-in-deployment\n  method:\
  \ post\n  operationId: startAllFlowsInDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/start-flow\n  method: post\n  operationId: startFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/stop-all-flows-in-deployment\n  method: post\n  operationId: stopAllFlowsInDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/stop-flow\n  method: post\n  operationId: stopFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/suspend-deployment\n  method: post\n  operationId: suspendDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/terminate-deployment\n  method: post\n  operationId: terminateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/update-deployment\n  method: post\n  operationId: updateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/update-nifi-version\n  method:\
  \ post\n  operationId: updateNifiVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/deployments/upload-asset\n  method: post\n  operationId: uploadAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/environments/list-nifi-versions\n  method: post\n  operationId: listNifiVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/fd-proxy/delete-flow-draft\n  method: post\n  operationId: deleteFlowDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/fd-proxy/list-flow-drafts\n  method: post\n  operationId: listFlowDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/fd-proxy/list-test-sessions\n  method: post\n  operationId: listTestSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/fd-proxy/restart-test-session\n  method: post\n  operationId: restartTestSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/fd-proxy/suspend-test-session\n  method: post\n  operationId: suspendTestSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/fd-proxy/terminate-test-session\n  method: post\n  operationId: terminateTestSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dfx/api/rpc-v1/inbound-connection-endpoint-certificates/download-client-certificates-encoded\n  method: post\n  operationId: getClientCertificatesEncoded\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/inbound-connection-endpoints/create-inbound-connection-endpoint\n  method: post\n  operationId: createInboundConnectionEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/inbound-connection-endpoints/delete-inbound-connection-endpoint\n\
  \  method: post\n  operationId: deleteInboundConnectionEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/inbound-connection-endpoints/describe-inbound-connection-endpoint\n  method: post\n  operationId: describeInboundConnectionEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/inbound-connection-endpoints/list-inbound-connection-endpoints\n  method: post\n  operationId: listInboundConnectionEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/inbound-connection-endpoints/renew-certificates\n  method: post\n  operationId: renewInboundConnectionEndpointCertificates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/parameter-groups/create-parameter-group\n  method: post\n  operationId: createParameterGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/parameter-groups/delete-parameter-group\n  method: post\n  operationId: deleteParameterGroup\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/parameter-groups/describe-parameter-group\n  method: post\n  operationId: describeParameterGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/parameter-groups/duplicate-parameter-group\n  method: post\n  operationId: duplicateParameterGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/parameter-groups/list-parameter-groups\n  method: post\n  operationId: listParameterGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dfx/api/rpc-v1/parameter-groups/update-parameter-group\n  method: post\n  operationId: updateParameterGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/parameter-groups/upload-parameter-asset\n  method: post\n  operationId: uploadParameterAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dfx/api/rpc-v1/workload-resources/reassign-resources\n  method: post\n  operationId: reassignResources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cloudprivatelinks/authorizePrivateLinkServiceAccess\n  method: post\n  operationId: authorizePrivateLinkServiceAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cloudprivatelinks/createPrivateLinkEndpoint\n  method:\
  \ post\n  operationId: createPrivateLinkEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cloudprivatelinks/deletePrivateLinkEndpoint\n  method: post\n  operationId: deletePrivateLinkEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (249 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/agentic-access/cloudera-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/agentic-access/cloudera-agentic-access.yml
summary_line: 778 operations · 556 acting · 30 human-in-the-loop
tags:
- Big Data
- Data Engineering
- Data Lakehouse
- Data Platform
- Data Warehouse
- Hadoop
- Hybrid Cloud
- Machine Learning
- Streaming
---
