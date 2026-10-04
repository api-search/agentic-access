---
acting_count: 63
action_class_counts:
  acting: 63
  connected: 51
api_specs:
- filename: microsoft-azure-batch-jobs-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Jobs API
  slug: microsoft-azure-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-jobs-api-openapi.yml
- filename: microsoft-azure-batch-pools-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Pools API
  slug: microsoft-azure-batch-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-pools-api-openapi.yml
- filename: microsoft-azure-batch-tasks-api-openapi.yml
  format: yaml
  label: microsoft-azure-batch Tasks API
  slug: microsoft-azure-batch-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-tasks-api-openapi.yml
- filename: microsoft-azure-batch-application-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Application API
  slug: microsoft-azure-batch-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-application-api-openapi.yml
- filename: microsoft-azure-batch-applicationpackage-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Application Package API
  slug: microsoft-azure-batch-applicationpackage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-applicationpackage-api-openapi.yml
- filename: microsoft-azure-batch-applications-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Applications API
  slug: microsoft-azure-batch-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-applications-api-openapi.yml
- filename: microsoft-azure-batch-batchaccount-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Batch Account API
  slug: microsoft-azure-batch-batchaccount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-batchaccount-api-openapi.yml
- filename: microsoft-azure-batch-detectorresponses-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Detector Responses API
  slug: microsoft-azure-batch-detectorresponses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-detectorresponses-api-openapi.yml
- filename: microsoft-azure-batch-job-schedules-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Job Schedules API
  slug: microsoft-azure-batch-job-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-job-schedules-api-openapi.yml
- filename: microsoft-azure-batch-location-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Location API
  slug: microsoft-azure-batch-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-location-api-openapi.yml
- filename: microsoft-azure-batch-networksecurityperimeter-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Network Security Perimeter API
  slug: microsoft-azure-batch-networksecurityperimeter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-networksecurityperimeter-api-openapi.yml
- filename: microsoft-azure-batch-nodes-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Nodes API
  slug: microsoft-azure-batch-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-nodes-api-openapi.yml
- filename: microsoft-azure-batch-operations-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Operations API
  slug: microsoft-azure-batch-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-operations-api-openapi.yml
- filename: microsoft-azure-batch-pool-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Pool API
  slug: microsoft-azure-batch-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-pool-api-openapi.yml
- filename: microsoft-azure-batch-privatelinkresource-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Private Link Resource API
  slug: microsoft-azure-batch-privatelinkresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-privatelinkresource-api-openapi.yml
- filename: microsoft-azure-batch-private-endpoint-connection-api-openapi.yml
  format: yaml
  label: Microsoft Azure Batch Private Endpoint Connection API
  slug: microsoft-azure-batch-private-endpoint-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/openapi/microsoft-azure-batch-private-endpoint-connection-api-openapi.yml
consequence_counts:
  read: 51
  safety-critical: 11
  write: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Azure Batch Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /jobs/{jobId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /jobs/{jobId}/tasks/{taskId}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /jobs/{jobId}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /jobschedules/{jobScheduleId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /jobschedules/{jobScheduleId}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pools/{poolId}/disableautoscale
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pools/{poolId}/nodes/{nodeId}/disablescheduling
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pools/{poolId}/nodes/{nodeId}/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pools/{poolId}/stopresize
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/pools/{poolName}/disableAutoScale
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/pools/{poolName}/stopResize
operation_count: 114
overview: 'Microsoft Azure Batch exposes 114 API operations that an AI agent could call, of which 63 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 51 read, 52 write, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Azure Batch
provider_slug: microsoft-azure-batch
slug: microsoft-azure-batch-agentic-access
source_filename: microsoft-azure-batch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: generated\nsource: openapi/microsoft-azure-batch-application-api-openapi.yml, openapi/microsoft-azure-batch-applicationpackage-api-openapi.yml,\n  openapi/microsoft-azure-batch-applications-api-openapi.yml, openapi/microsoft-azure-batch-batchaccount-api-openapi.yml,\n  openapi/microsoft-azure-batch-detectorresponses-api-openapi.yml, openapi/microsoft-azure-batch-job-schedules-api-openapi.yml,\n  openapi/microsoft-azure-batch-jobs-api-openapi.yml, openapi/microsoft-azure-batch-location-api-openapi.yml,\n  openapi/microsoft-azure-batch-networksecurityperimeter-api-openapi.yml, openapi/microsoft-azure-batch-nodes-api-openapi.yml,\n  openapi/microsoft-azure-batch-operations-api-openapi.yml, openapi/microsoft-azure-batch-pool-api-openapi.yml,\n  openapi/microsoft-azure-batch-pools-api-openapi.yml, openapi/microsoft-azure-batch-private-endpoint-connection-api-openapi.yml,\n  openapi/microsoft-azure-batch-privatelinkresource-api-openapi.yml, openapi/microsoft-azure-batch-tasks-api-openapi.yml\n\
  description: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 114\n  by_action_class:\n    connected: 51\n    acting: 63\n  by_consequence:\n    read: 51\n    write: 52\n    safety-critical: 11\n  human_in_the_loop_required: 11\noperations:\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications\n  method: get\n  operationId: Application_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationName}\n\
  \  method: get\n  operationId: Application_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationName}\n  method: put\n  operationId: Application_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationName}\n  method: patch\n  operationId: Application_Update\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationName}\n  method: delete\n  operationId: Application_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationName}/versions\n  method: get\n  operationId:\
  \ ApplicationPackage_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationName}/versions/{versionName}\n  method: get\n  operationId: ApplicationPackage_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationName}/versions/{versionName}\n  method: put\n  operationId: ApplicationPackage_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationName}/versions/{versionName}\n  method: delete\n  operationId: ApplicationPackage_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationName}/versions/{versionName}/activate\n  method: post\n  operationId: ApplicationPackage_Activate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /applications\n  method: get\n  operationId: Applications_ListApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /applications/{applicationId}\n  method: get\n  operationId: Applications_GetApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /subscriptions/{subscriptionId}/providers/Microsoft.Batch/batchAccounts\n  method:\
  \ get\n  operationId: BatchAccount_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts\n  method: get\n  operationId: BatchAccount_ListByResourceGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}\n  method: get\n  operationId: BatchAccount_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}\n\
  \  method: put\n  operationId: BatchAccount_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}\n  method: patch\n  operationId: BatchAccount_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}\n  method:\
  \ delete\n  operationId: BatchAccount_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/listKeys\n  method: post\n  operationId: BatchAccount_GetKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/outboundNetworkDependenciesEndpoints\n\
  \  method: get\n  operationId: BatchAccount_ListOutboundNetworkDependenciesEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/regenerateKeys\n  method: post\n  operationId: BatchAccount_RegenerateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/syncAutoStorageKeys\n  method: post\n  operationId: BatchAccount_SynchronizeAutoStorageKeys\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/detectors\n  method: get\n  operationId: BatchAccount_ListDetectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/detectors/{detectorId}\n  method: get\n  operationId: BatchAccount_GetDetector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /jobschedules\n  method: get\n  operationId: JobSchedules_ListJobSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules\n  method: post\n  operationId: JobSchedules_CreateJobSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules/{jobScheduleId}\n  method: get\n  operationId: JobSchedules_GetJobSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules/{jobScheduleId}\n  method: put\n  operationId: JobSchedules_ReplaceJobSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules/{jobScheduleId}\n  method: patch\n  operationId: JobSchedules_UpdateJobSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules/{jobScheduleId}\n\
  \  method: delete\n  operationId: JobSchedules_DeleteJobSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules/{jobScheduleId}\n  method: head\n  operationId: JobSchedules_JobScheduleExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules/{jobScheduleId}/disable\n  method: post\n  operationId: JobSchedules_DisableJobSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules/{jobScheduleId}/enable\n  method: post\n  operationId: JobSchedules_EnableJobSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules/{jobScheduleId}/terminate\n  method: post\n  operationId: JobSchedules_TerminateJobSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs\n  method: get\n  operationId: Jobs_ListJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs\n  method: post\n  operationId: Jobs_CreateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs/{jobId}\n  method: get\n  operationId: Jobs_GetJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs/{jobId}\n  method: put\n  operationId: Jobs_ReplaceJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs/{jobId}\n  method: patch\n  operationId: Jobs_UpdateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs/{jobId}\n  method: delete\n  operationId: Jobs_DeleteJob\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs/{jobId}/disable\n  method: post\n  operationId: Jobs_DisableJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs/{jobId}/enable\n  method: post\n  operationId: Jobs_EnableJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs/{jobId}/jobpreparationandreleasetaskstatus\n  method: get\n  operationId: Jobs_ListJobPreparationAndReleaseTaskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs/{jobId}/taskcounts\n  method: get\n  operationId: Jobs_GetJobTaskCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobs/{jobId}/terminate\n  method: post\n  operationId: Jobs_TerminateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /jobschedules/{jobScheduleId}/jobs\n  method: get\n  operationId: Jobs_ListJobsFromSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /subscriptions/{subscriptionId}/providers/Microsoft.Batch/locations/{locationName}/checkNameAvailability\n  method: post\n  operationId: Location_CheckNameAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  \    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/providers/Microsoft.Batch/locations/{locationName}/quotas\n  method: get\n  operationId: Location_GetQuotas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/providers/Microsoft.Batch/locations/{locationName}/virtualMachineSkus\n  method: get\n  operationId: Location_ListSupportedVirtualMachineSkus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/networkSecurityPerimeterConfigurations\n  method: get\n  operationId: NetworkSecurityPerimeter_ListConfigurations\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/networkSecurityPerimeterConfigurations/{networkSecurityPerimeterConfigurationName}\n  method: get\n  operationId: NetworkSecurityPerimeter_GetConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/networkSecurityPerimeterConfigurations/{networkSecurityPerimeterConfigurationName}/reconcile\n  method: post\n  operationId: NetworkSecurityPerimeter_ReconcileConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /pools/{poolId}/nodes\n  method: get\n  operationId: Nodes_ListNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}\n  method: get\n  operationId: Nodes_GetNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/deallocate\n  method: post\n  operationId: Nodes_DeallocateNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/disablescheduling\n  method: post\n  operationId: Nodes_DisableNodeScheduling\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/enablescheduling\n  method: post\n  operationId: Nodes_EnableNodeScheduling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/extensions\n  method: get\n  operationId: Nodes_ListNodeExtensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/extensions/{extensionName}\n  method: get\n  operationId: Nodes_GetNodeExtension\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/files\n  method: get\n  operationId: Nodes_ListNodeFiles\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/files/{filePath}\n  method: get\n  operationId: Nodes_GetNodeFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/files/{filePath}\n  method: delete\n  operationId: Nodes_DeleteNodeFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/files/{filePath}\n  method: head\n  operationId:\
  \ Nodes_GetNodeFileProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/reboot\n  method: post\n  operationId: Nodes_RebootNode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/reimage\n  method: post\n  operationId: Nodes_ReimageNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/remoteloginsettings\n  method: get\n  operationId: Nodes_GetNodeRemoteLoginSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/start\n  method: post\n  operationId: Nodes_StartNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/uploadbatchservicelogs\n  method: post\n  operationId: Nodes_UploadNodeLogs\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/users\n  method: post\n  operationId: Nodes_CreateNodeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/users/{userName}\n  method: put\n  operationId: Nodes_ReplaceNodeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /pools/{poolId}/nodes/{nodeId}/users/{userName}\n  method: delete\n  operationId: Nodes_DeleteNodeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://batch.core.windows.net//.default\n- path: /providers/Microsoft.Batch/operations\n  method: get\n  operationId: Operations_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/pools\n\
  \  method: get\n  operationId: Pool_ListByBatchAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/pools/{poolName}\n  method: get\n  operationId: Pool_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/pools/{poolName}\n  method: put\n  operationId: Pool_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/pools/{poolName}\n  method: patch\n  operationId: Pool_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/pools/{poolName}\n  method: delete\n  operationId: Pool_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n\n\n# --- truncated at 32 KB (45 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/agentic-access/microsoft-azure-batch-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-batch/refs/heads/main/agentic-access/microsoft-azure-batch-agentic-access.yml
summary_line: 114 operations · 63 acting · 11 human-in-the-loop
tags:
- Batch
- Compute
- Job Scheduling
- High Performance Computing
- Cloud
- Microsoft
- Azure
- Parallel Processing
- Scheduling
- Infrastructure
---
