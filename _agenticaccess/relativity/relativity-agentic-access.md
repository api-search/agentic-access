---
acting_count: 421
action_class_counts:
  acting: 421
  connected: 312
api_specs:
- filename: relativity-object-manager-openapi.yml
  format: yaml
  label: Relativity Object Manager API
  slug: relativity-object-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-object-manager-openapi.yml
- filename: relativity-import-openapi.yml
  format: yaml
  label: Relativity Import Service API
  slug: relativity-import-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-import-openapi.yml
- filename: relativity-export-openapi.yml
  format: yaml
  label: Relativity Export Service API
  slug: relativity-export-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-export-openapi.yml
- filename: relativity-workspace-openapi.yml
  format: yaml
  label: Relativity Workspace Manager API
  slug: relativity-workspace-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-workspace-openapi.yml
- filename: relativity-productions-openapi.yml
  format: yaml
  label: Relativity Production Manager API
  slug: relativity-production-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-productions-openapi.yml
- filename: relativity-legal-hold-openapi.yml
  format: yaml
  label: Relativity Legal Hold API
  slug: relativity-legal-hold-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-legal-hold-openapi.yml
- filename: relativity-automated-workflows-openapi.yml
  format: yaml
  label: Relativity Automated Workflows API
  slug: relativity-automated-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-automated-workflows-openapi.yml
- filename: relativity-permissions-openapi.yml
  format: yaml
  label: Relativity Audit API
  slug: relativity-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-permissions-openapi.yml
- filename: relativity-identity-openapi.yml
  format: yaml
  label: Relativity User and Permission Manager API
  slug: relativity-user-and-permission-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-identity-openapi.yml
- filename: relativity-billing-v2-openapi.yml
  format: yaml
  label: Relativity Billing Insights API
  slug: relativity-billing-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-billing-v2-openapi.yml
consequence_counts:
  physical: 5
  read: 312
  safety-critical: 21
  write: 395
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 21
kind: agentic-access
layout: agentic-access
method: generated
name: Relativity Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Relativity-Identity/v1/auth-provider-types
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /Relativity-Identity/v1/users/{userID}/login-profile/set/password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /access-control/public/v1/role-assignments/instance
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /access-control/public/v1/role-assignments/{nodeType}/{nodeKey}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /collect-services/v1/CollectAPI/{workspaceId}/collection/{collectionArtifactId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/begin/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/cancel/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/documents-configurations/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/end/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/pause/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/rdos-configurations/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/resume/
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/sources/{sourceID}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /import-service/v1/workspaces/{workspaceID}/import-jobs/{importJobID}/sources/{sourceID}/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /relativity-arm/v1/jobs/{jobID}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /relativity-imaging/v1/workspaces/{workspaceID}/jobs/{imagingJobID}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /relativity-infrastructure/v1/workspaces/-1/worker-servers/{serverID}/disable-processing-license
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /relativity-infrastructure/v1/workspaces/-1/worker-servers/{serverID}/stop-worker
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/transfer/jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/transfer/jobs/{jobId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Relativity-Identity/v1/Users/bulk-invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Relativity-Identity/v1/users/bulk-invitation/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Relativity-Identity/v1/users/{userID}/Invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Relativity-Identity/v1/workspaces/{workspaceID}/query-users
operation_count: 733
overview: 'Relativity exposes 733 API operations that an AI agent could call, of which 421 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 312 read, 395 write, 5 physical, and 21 safety-critical.


  21 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Relativity
provider_slug: relativity
slug: relativity-agentic-access
source_filename: relativity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/relativity-analytics-conceptual-openapi.yml, openapi/relativity-arm-openapi.yml,\n  openapi/relativity-arm-v3-openapi.yml, openapi/relativity-automated-workflows-openapi.yml,\n  openapi/relativity-collect-openapi.yml, openapi/relativity-data-visualization-openapi.yml,\n  openapi/relativity-dtsearch-openapi.yml, openapi/relativity-environment-openapi.yml, openapi/relativity-glacier-openapi.yml,\n  openapi/relativity-identity-openapi.yml, openapi/relativity-imaging-openapi.yml, openapi/relativity-import-openapi.yml,\n  openapi/relativity-infrastructure-openapi.yml, openapi/relativity-legal-hold-openapi.yml,\n  openapi/relativity-mass-operations-openapi.yml, openapi/relativity-notifications-openapi.yml,\n  openapi/relativity-object-manager-openapi.yml, openapi/relativity-permissions-openapi.yml,\n  openapi/relativity-pivot-openapi.yml, openapi/relativity-processing-v1-openapi.yml, openapi/relativity-processing-v2-openapi.yml,\n\
  \  openapi/relativity-productions-openapi.yml, openapi/relativity-review-service-openapi.yml,\n  openapi/relativity-rie-openapi.yml, openapi/relativity-staging-reports-openapi.yml, openapi/relativity-structured-analytics-openapi.yml,\n  openapi/relativity-telemetry-openapi.yml, openapi/relativity-transfer-openapi.yml, openapi/relativity-usage-reports-openapi.yml,\n  openapi/relativity-workspace-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 733\n  by_action_class:\n    acting: 421\n    connected: 312\n  by_consequence:\n    write: 395\n    read: 312\n    safety-critical: 21\n    physical: 5\n  human_in_the_loop_required: 21\noperations:\n- path: /conceptual-analytics/v1/workspaces/{workspaceID}/indexes/\n  method: post\n  operationId: Analytics.Conceptual.Service.Interfaces.Public.v1.IConceptualIndexService.CreateAsync\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conceptual-analytics/v1/workspaces/{workspaceID}/indexes/{indexID}\n  method: get\n  operationId: Analytics.Conceptual.Service.Interfaces.Public.v1.IConceptualIndexService.ReadAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conceptual-analytics/v1/workspaces/{workspaceID}/indexes/{indexID}\n  method: put\n  operationId: Analytics.Conceptual.Service.Interfaces.Public.v1.IConceptualIndexService.UpdateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conceptual-analytics/v1/workspaces/{workspaceID}/indexes/{indexID}\n  method: delete\n  operationId: Analytics.Conceptual.Service.Interfaces.Public.v1.IConceptualIndexService.DeleteAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conceptual-analytics/v1/workspaces/{workspaceID}/indexes/{indexID}/status\n  method: get\n  operationId: Analytics.Conceptual.Service.Interfaces.Public.v1.IConceptualIndexService.GetStatusAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conceptual-analytics/v1/workspaces/{workspaceID}/indexes/{indexID}/job\n  method: post\n \
  \ operationId: Analytics.Conceptual.Service.Interfaces.Public.v1.IConceptualIndexService.SubmitJobAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conceptual-analytics/v1/workspaces/{workspaceID}/indexes/{indexID}/job\n  method: delete\n  operationId: Analytics.Conceptual.Service.Interfaces.Public.v1.IConceptualIndexService.CancelJobAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v3/restore-jobs\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V3.Restore.IArmRestoreJobManager.CreateAsync\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v3/restore-jobs/{jobID}\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V3.Restore.IArmRestoreJobManager.ReadAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v3/restore-jobs/{jobID}\n  method: put\n  operationId: Relativity.ARM.Services.Interfaces.V3.Restore.IArmRestoreJobManager.UpdateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /relativity-arm/v3/restore-jobs/{jobID}\n  method: delete\n  operationId: Relativity.ARM.Services.Interfaces.V3.Restore.IArmRestoreJobManager.DeleteAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v3/jobs/{jobID}/status\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V3.JobInformation.IArmJobInformationManager.GetJobStatusAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v3/jobs/{jobID}/cancel\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V3.JobAction.IArmJobActionManager.CancelAsync\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v3/jobs/{jobID}/run\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V3.JobAction.IArmJobActionManager.RunAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v3/archive-jobs\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V3.Archive.IArmArchiveJobManager.CreateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v3/archive-jobs/{jobID}\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V3.Archive.IArmArchiveJobManager.ReadAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v3/archive-jobs/{jobID}\n  method: put\n  operationId: Relativity.ARM.Services.Interfaces.V3.Archive.IArmArchiveJobManager.UpdateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v3/archive-jobs/{jobID}\n  method: delete\n  operationId: Relativity.ARM.Services.Interfaces.V3.Archive.IArmArchiveJobManager.DeleteAsync\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/tasks/{taskId}/retry\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V1.TaskAction.IArmTaskActionManager.RetryFailedTaskAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/restore-jobs\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V1.Restore.IArmRestoreJobManager.CreateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/restore-jobs/{jobID}\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V1.Restore.IArmRestoreJobManager.ReadAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v1/restore-jobs/{jobID}\n  method: put\n  operationId: Relativity.ARM.Services.Interfaces.V1.Restore.IArmRestoreJobManager.UpdateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/restore-jobs/{jobID}\n  method: delete\n  operationId: Relativity.ARM.Services.Interfaces.V1.Restore.IArmRestoreJobManager.DeleteAsync\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/move-jobs\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V1.Move.IArmMoveJobManager.CreateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/move-jobs/{jobID}\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V1.Move.IArmMoveJobManager.ReadAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /relativity-arm/v1/move-jobs/{jobID}\n  method: put\n  operationId: Relativity.ARM.Services.Interfaces.V1.Move.IArmMoveJobManager.UpdateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/move-jobs/{jobID}\n  method: delete\n  operationId: Relativity.ARM.Services.Interfaces.V1.Move.IArmMoveJobManager.DeleteAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/jobs/{jobID}/status\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V1.JobStatus.IArmJobStatusManager.ReadAsync\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v1/jobs/{jobID}/logs\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V1.JobInformation.IArmJobInformationManager.DownloadLogAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v1/jobs/{jobExecutionId}/statistics\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V1.JobInformation.IArmJobInformationManager.GetJobStatisticsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v1/jobs/{jobExecutionID}/qualityCheckResult\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V1.JobInformation.IArmJobInformationManager.GetQualityCheckResultAsync\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v1/jobs/{jobID}/cancel\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V1.JobAction.IArmJobActionManager.CancelAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/jobs/{jobID}/pause\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V1.JobAction.IArmJobActionManager.PauseAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /relativity-arm/v1/jobs/{jobID}/run\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V1.JobAction.IArmJobActionManager.RunAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/jobs/{jobID}/terminate\n  method: delete\n  operationId: Relativity.ARM.Services.Interfaces.V1.JobAction.IArmJobActionManager.TerminateJobAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /relativity-arm/v1/health-check\n  method: get\n  operationId:\
  \ Relativity.ARM.Services.Interfaces.V1.HealthCheck.IArmHealthCheckManager.HealthCheckAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v1/database-restore-jobs\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V1.DatabaseRestore.IArmDatabaseRestoreJobManager.CreateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/database-restore-jobs/{jobID}\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V1.DatabaseRestore.IArmDatabaseRestoreJobManager.ReadAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /relativity-arm/v1/database-restore-jobs/{jobID}\n  method: put\n  operationId: Relativity.ARM.Services.Interfaces.V1.DatabaseRestore.IArmDatabaseRestoreJobManager.UpdateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/database-restore-jobs/{jobID}\n  method: delete\n  operationId: Relativity.ARM.Services.Interfaces.V1.DatabaseRestore.IArmDatabaseRestoreJobManager.DeleteAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/archive-information\n\
  \  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V1.ArchiveInformation.IArmArchiveInformationManager.ReadAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/archive-information/additional-files-directories/{workspaceId}\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V1.ArchiveInformation.IArmArchiveInformationManager.GetAdditionalFilesDirectoriesAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v1/archive-jobs\n  method: post\n  operationId: Relativity.ARM.Services.Interfaces.V1.Archive.IArmArchiveJobManager.CreateAsync\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/archive-jobs/{jobID}\n  method: get\n  operationId: Relativity.ARM.Services.Interfaces.V1.Archive.IArmArchiveJobManager.ReadAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-arm/v1/archive-jobs/{jobID}\n  method: put\n  operationId: Relativity.ARM.Services.Interfaces.V1.Archive.IArmArchiveJobManager.UpdateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-arm/v1/archive-jobs/{jobID}\n\
  \  method: delete\n  operationId: Relativity.ARM.Services.Interfaces.V1.Archive.IArmArchiveJobManager.DeleteAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/archive-jobs\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/archive-jobs/{jobID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/archive-jobs/{jobID}\n  method: put\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/archive-jobs/{jobID}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/jobs/{jobID}/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/jobs/{jobID}/run\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/jobs/{jobID}/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/restore-jobs\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/restore-jobs/{jobID}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/restore-jobs/{jobID}\n  method: put\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/restore-jobs/{jobID}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-automated-workflows/v2/workspaces/{workspaceID}/notifiers/trigger\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-automated-workflows/v2/workspaces/{workspaceID}/actions\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-automated-workflows/v2/workspaces/{workspaceID}/actions\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-automated-workflows/v2/workspaces/{workspaceID}/triggers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-automated-workflows/v2/workspaces/{workspaceID}/triggers\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-automated-workflows/v2/language/expressions/run\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect-services/v1/CollectAPI/{workspaceId}/collection\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /collect-services/v1/CollectAPI/{workspaceId}/collection/{collectionArtifactId}/start-target-generation\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /collect-services/v1/CollectAPI/{workspaceArtifactId}/collection/{collectionArtifactId}/target-generation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /collect-services/v1/CollectAPI/{workspaceArtifactId}/collection/{collectionArtifactId}/start-collection\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /collect-services/v1/CollectAPI/{workspaceArtifactId}/collection/{collectionArtifactId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /collect-services/v1/CollectAPI/{workspaceId}/collection/{collectionArtifactId}/stop\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /Relativity.Rest/api/Relativity.ObjectManager/v1/workspace/-1/object/queryslim\n  method:\
  \ post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /Relativity.Rest/api/Relativity.ObjectManager/v1/workspace/{workspaceId}/object/queryslim\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /relativity-data-visualization/v1/workspaces/{workspaceID}/tabs\n  method: post\n  operationId: Relativity.Services.Interfaces.DataVisualization.V1.Tab.ITabManager.CreateAsync\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-data-visualization/v1/workspaces/{workspaceID}/tabs/{tabArtifactID}\n  method: get\n  operationId: Relativity.Services.Interfaces.DataVisualization.V1.Tab.ITabManager.ReadAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-data-visualization/v1/workspaces/{workspaceID}/tabs/{tabArtifactID}\n  method: put\n  operationId: Relativity.Services.Interfaces.DataVisualization.V1.Tab.ITabManager.UpdateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /relativity-data-visualization/v1/workspaces/{workspaceID}/tabs/{tabArtifactID}\n  method: delete\n  operationId: Relativity.Services.Interfaces.DataVisualization.V1.Tab.ITabManager.DeleteAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /relativity-data-visualization/v1/workspaces/{workspaceID}/tabs/meta\n  method: get\n  operationId: Relativity.Services.Interfaces.DataVisualization.V1.Tab.ITabManager.GetMetaAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-data-visualization/v1/workspaces/{workspaceID}/tabs/eligible-parents\n  method: get\n  operationId: Relativity.Services.Interfaces.DataVisualization.V1.Tab.ITabManager.GetEligibleParentTabsAsync\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-data-visualization/v1/workspaces/{workspaceID}/tabs/eligible-object-types\n  method: get\n  operationId: Relativity.Services.Interfaces.DataVisualization.V1.Tab.ITabManager.GetEligibleObjectTypesAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-data-visualization/v1/workspaces/{workspaceID}/tabs/view-order-list\n  method: get\n  operationId: Relativity.Services.Interfaces.DataVisualization.V1.Tab.ITabManager.GetViewOrderListAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-data-visualization/v1/workspaces/{workspaceID}/tabs/navigation\n  method: get\n  operationId: Relativity.Services.Interfaces.DataVisualization.V1.Tab.ITabManager.GetAllNavigationTabsAsync\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-dtsearch/v1/workload-discovery/{agentGuid}/workload\n  method: get\n  operationId: Relativity.DTSearch.V1.WorkloadDiscoveryManager.IWorkloadDiscoveryManager.GetWorkloadAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-dtsearch/v1/workspaces/{workspaceID}/dtsearch-indexes/{dtSearchArtifactID}/consistency-check-is-affected\n  method: get\n  operationId: Relativity.DTSearch.V1.ConsistencyCheckManager.IConsistencyCheckManager.GetIsAffectedAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-dtsearch/v1/GetArchiveLocationAsync\n  method: get\n  operationId: Relativity.DTSearch.V1.ArmTestService.IArmTestService.GetArchiveLocationAsync\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /relativity-dtsearch/v1/SetDtSearchIndexLocationToNullAsync\n  method: post\n  operationId: Relativity.DTSearch.V1.ArmTestService.IArmTestService.SetDtSearchIndexLocationToNullAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escal\n\n# --- truncated at 32 KB (290 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/agentic-access/relativity-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/agentic-access/relativity-agentic-access.yml
summary_line: 733 operations · 421 acting · 21 human-in-the-loop
tags:
- eDiscovery
- Legal
- Document Review
- Legal Technology
- Data Processing
- AI Review
- Litigation
- Compliance
---
