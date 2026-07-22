---
acting_count: 759
action_class_counts:
  acting: 759
  connected: 543
api_specs:
- filename: spectro-cloud-palette-openapi.json
  format: json
  label: Palette APIs
  slug: palette-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/openapi/spectro-cloud-palette-openapi.json
- filename: spectro-cloud-edge-management-openapi.json
  format: json
  label: Edge Local Management APIs
  slug: edge-local-management-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/openapi/spectro-cloud-edge-management-openapi.json
consequence_counts:
  physical: 14
  read: 543
  safety-critical: 29
  write: 716
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 29
kind: agentic-access
layout: agentic-access
method: generated
name: Spectro Cloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/apiKeys/{uid}/state
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/auth/password/{passwordToken}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/user/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/clouds/cloudTypes/{cloudType}/content/controlPlane
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/clouds/cloudTypes/{cloudType}/content/controlPlane
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/clouds/cloudTypes/{cloudType}/content/templates/controlPlanePoolTemplate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/clouds/cloudTypes/{cloudType}/content/templates/controlPlanePoolTemplate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/edge-mgmt/edgehosts/current/actions/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/edge-mgmt/edgehosts/current/actions/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/edge-mgmt/edgehosts/current/actions/shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/edgehosts/tokens/{uid}/state
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/edgehosts/{uid}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/overlords/{uid}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/spectroclusters/{uid}/clusterConfig/controlPlaneHealthCheckTimeout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/spectroclusters/{uid}/edge/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/spectroclusters/{uid}/features/backup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/spectroclusters/{uid}/k8certificates/renew
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/spectroclusters/{uid}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/spectroclusters/{uid}/vms/{vmName}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/system/admin/email
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/system/admin/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/system/admins/{uid}/passwordResetLink
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/system/users/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/system/users/password/{passwordToken}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/tenants/{tenantUid}/preferences/clusterGroup
operation_count: 1302
overview: 'Spectro Cloud exposes 1302 API operations that an AI agent could call, of which 759 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 543 read, 716 write, 14 physical, and 29 safety-critical.


  29 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spectro Cloud
provider_slug: spectro-cloud
slug: spectro-cloud-agentic-access
source_filename: spectro-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/spectro-cloud-edge-management-openapi.json, openapi/spectro-cloud-palette-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1302\n  by_action_class:\n    connected: 543\n    acting: 759\n  by_consequence:\n    read: 543\n    write: 716\n    safety-critical: 29\n    physical: 14\n  human_in_the_loop_required: 29\noperations:\n- path: /v1/edge-mgmt/cluster\n  method: get\n  operationId: v1ClusterConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/cluster\n  method: post\n  operationId: v1CreateCluster\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster\n  method: delete\n  operationId: v1DeleteCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster\n  method: patch\n  operationId: v1PatchCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster/applications\n  method: get\n\
  \  operationId: v1ClusterApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/cluster/certificates\n  method: get\n  operationId: v1CertificateDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/cluster/details\n  method: get\n  operationId: v1ClusterGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/cluster/events\n  method: get\n  operationId: v1GetClusterEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/cluster/pair\n  method: post\n  operationId: v1ClusterPair\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster/pair/details\n  method: get\n  operationId: v1ClusterPairDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/cluster/pair/reject\n  method: post\n  operationId: v1ClusterPairReject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster/pair/verify-connection\n  method: post\n  operationId: v1ClusterPairVerifyConnection\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster/profiles\n  method: put\n  operationId: v1UpdateClusterProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster/profiles/variables/validate\n  method: post\n  operationId: v1ValidateClusterProfileVariables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/edge-mgmt/cluster/registry/content/details\n  method: get\n  operationId: v1HarborContentsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/cluster/registry/content/sync-status/details\n  method: get\n  operationId: v1HarborContentsSyncStatusDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/cluster/registry/health\n  method: get\n  operationId: V1HarborHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/cluster/renew-certificates\n  method: post\n  operationId: v1RenewCerts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster/settings\n  method: put\n  operationId: v1EdgeNativeClusterSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster/{clusterName}\n  method: put\n  operationId: v1UpdateClusterConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/cluster/{clusterName}\n  method: patch\n  operationId: v1PatchClusterConfig\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/clusters/archive/embedded/details\n  method: get\n  operationId: V1ClusterConfigArchiveEmbedded\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/clusters/archive/overridden/details\n  method: get\n  operationId: v1ClusterConfigArchiveOverriden\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/clusters/archive/update\n  method: delete\n  operationId: v1DeleteClusterUpdateArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/clusters/archive/update/details\n  method: get\n  operationId: v1ClusterConfigArchiveUpdate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/clusters/current/machinepools\n  method: get\n  operationId: v1MachinePoolDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/clusters/current/machinepools\n  method: post\n  operationId: v1ClusterMachinePoolCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/clusters/current/machinepools/{poolName}\n  method: put\n  operationId: v1ClusterMachinePoolUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/clusters/current/machinepools/{poolName}\n  method: delete\n  operationId: v1ClusterMachinePoolDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/clusters/current/machinepools/{poolName}\n  method: patch\n  operationId: v1ClusterMachinePoolPatch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/clusters/current/machinepools/{poolName}/nodes/{nodeName}\n  method: delete\n  operationId: v1ClusterMachinePoolNodeDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/clusters/current/nodes\n  method: get\n  operationId: v1ClusterNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/connectivity/ping\n  method:\
  \ get\n  operationId: v1PingHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/connectivity/traceroute\n  method: get\n  operationId: v1TraceRouteHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current\n  method: get\n  operationId: v1EdgeHostInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/actions/content/signing-public-key\n  method: get\n  operationId: V1GetContentSigningPublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/actions/reboot\n\
  \  method: post\n  operationId: v1EdgeHostActionReboot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/actions/reset\n  method: post\n  operationId: v1EdgeHostActionReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/actions/shutdown\n  method: post\n  operationId: v1EdgeHostActionShutdown\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/actions/upload-clusterconfig\n  method: post\n  operationId: V1ClusterConfigUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/actions/upload-content\n  method: post\n  operationId: V1ContentUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/edge-mgmt/edgehosts/current/audits\n  method: get\n  operationId: v1Audits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/audits/download\n  method: get\n  operationId: v1AuditDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/audits/filters\n  method: get\n  operationId: v1AuditFilter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/configurations\n  method: get\n  operationId: V1EdgeHostConfigurationsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/edge-mgmt/edgehosts/current/configurations\n  method: put\n  operationId: V1EdgeHostConfigurationsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/configurations/status\n  method: get\n  operationId: v1EdgeHostConfigurationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/download-logs\n  method: get\n  operationId: v1EdgeHostDownloadLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/error-logs\n  method: get\n  operationId:\
  \ V1EdgeHostErrorLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/file-download/files\n  method: get\n  operationId: v1EdgeHostListCustomFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/file-download/{filePath}\n  method: get\n  operationId: v1EdgeHostCustomFileDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/generate-logs\n  method: post\n  operationId: v1EdgeHostGenerateLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/generate-logs-status\n  method: get\n  operationId: v1EdgeHostGenerateLogsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/link\n  method: post\n  operationId: v1EdgeHostLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/link/generate-token\n  method: post\n  operationId: v1EdgeHostLinkGenerateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/link/status\n  method: get\n  operationId: v1EdgeHostLinkStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/unlink\n  method: post\n  operationId: v1EdgeHostUnlink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/uploaded-content/details\n  method: get\n  operationId: v1UploadedContentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/userdata\n  method: get\n  operationId: v1GetEdgeHostUserdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/edgehosts/current/userdata\n  method: put\n  operationId: v1PutEdgeHostUserdata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/edgehosts/current/userdata\n  method: post\n  operationId: v1PostEdgeHostUserdata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/edge-mgmt/events/lifecycle\n  method: get\n  operationId: v1GetLifecycleEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/bonds\n  method: get\n  operationId: V1NetworkBonds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/bonds/{name}\n  method: get\n  operationId: V1NetworkBond\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/bonds/{name}\n  method: put\n  operationId: V1NetworkBondUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/network/bonds/{name}\n  method: post\n  operationId: V1NetworkBondCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/network/bonds/{name}\n  method: delete\n  operationId: V1NetworkBondDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/network/bridges\n  method: get\n  operationId: V1NetworkBridges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/bridges/{name}\n  method: get\n  operationId: V1NetworkBridge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/bridges/{name}\n  method: put\n  operationId: V1NetworkBridgeUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/network/bridges/{name}\n  method: post\n  operationId: V1NetworkBridgeCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/network/bridges/{name}\n  method: delete\n  operationId: V1NetworkBridgeDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/network/config-options\n  method: get\n  operationId: V1NetworkConfigOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/interfaces\n  method: get\n  operationId: V1NetworkInterfaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/interfaces/{name}\n  method: get\n  operationId:\
  \ V1NetworkInterface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/interfaces/{name}/config\n  method: put\n  operationId: V1NetworkInterfaceUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/network/management-interface\n  method: get\n  operationId: V1ManagementInterface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/management-interface\n  method: put\n  operationId: V1ManagementInterfaceUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/network/vlans\n  method: get\n  operationId: V1NetworkVLANs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/vlans/{name}\n  method: get\n  operationId: V1NetworkVLAN\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/edge-mgmt/network/vlans/{name}\n  method: put\n  operationId: V1NetworkVLANUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/edge-mgmt/network/vlans/{name}\n  method: post\n  operationId: V1NetworkVLANCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/network/vlans/{name}\n  method: delete\n  operationId: V1NetworkVLANDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/edge-mgmt/settings\n  method: get\n  operationId: v1Settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ping\n\
  \  method: get\n  operationId: V1Ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/current\n  method: get\n  operationId: V1CurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/current\n  method: patch\n  operationId: v1PatchCurrentUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/default/login\n  method: post\n  operationId: V1UserLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/default/logout\n  method: post\n  operationId: V1UserLogout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/default/password/reset\n  method: post\n  operationId: V1UserPasswordReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/users/default/token/renewal\n  method: post\n  operationId: V1UserTokenRenewal\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/activations/system\n  method: get\n  operationId: v1ActivationsSystemGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apiKeys\n  method: get\n  operationId: v1ApiKeysList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apiKeys\n  method: post\n  operationId: v1ApiKeysCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/apiKeys/{uid}\n  method: delete\n  operationId: v1ApiKeysUidDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apiKeys/{uid}\n  method: get\n  operationId: v1ApiKeysUidGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apiKeys/{uid}\n  method: patch\n  operationId: v1ApiKeysUidActiveState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apiKeys/{uid}\n  method: put\n\
  \  operationId: v1ApiKeysUidUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apiKeys/{uid}/state\n  method: put\n  operationId: v1ApiKeysUidState\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/appDeployments\n  method: post\n  operationId: v1AppDeploymentsVirtualClusterCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appDeployments/clusterGroup\n  method: post\n  operationId: v1AppDeploymentsClusterGroupCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appDeployments/{uid}\n  method: delete\n  operationId: v1AppDeploymentsUidDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/appDeployments/{uid}\n  method: get\n  operationId: v1AppDeploymentsUidGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appDeployments/{uid}/profile\n  method: get\n  operationId: v1AppDeploymentsUidProfileGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appDeployments/{uid}/profile\n  method: put\n  operationId: v1AppDeploymentsUidProfileUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appDeployments/{uid}/profile/apply\n  method: patch\n  operationId:\
  \ v1AppDeploymentsUidProfileApply\n  x-agentic-access:\n    action-class: acting\n   \n\n# --- truncated at 32 KB (407 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/agentic-access/spectro-cloud-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spectro-cloud/refs/heads/main/agentic-access/spectro-cloud-agentic-access.yml
summary_line: 1302 operations · 759 acting · 29 human-in-the-loop
tags:
- Company
- Infrastructure
- Kubernetes
- Cloud Native
- Cluster Management
- Edge Computing
- Multi-Cloud
- DevOps
- AI Infrastructure
---
