---
acting_count: 179
action_class_counts:
  acting: 179
  connected: 242
api_specs:
- filename: zededa-node_service-openapi.json
  format: json
  label: ZEDEDA Edge Node Service
  slug: zededa-edge-node-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-node_service-openapi.json
- filename: zededa-app_service-openapi.json
  format: json
  label: ZEDEDA Edge Application Service
  slug: zededa-edge-application-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-app_service-openapi.json
- filename: zededa-app_profile_service-openapi.json
  format: json
  label: ZEDEDA App Profiles Service
  slug: zededa-app-profiles-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-app_profile_service-openapi.json
- filename: zededa-network_service-openapi.json
  format: json
  label: ZEDEDA Edge Network Service
  slug: zededa-edge-network-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-network_service-openapi.json
- filename: zededa-storage_service-openapi.json
  format: json
  label: ZEDEDA Storage Service
  slug: zededa-storage-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-storage_service-openapi.json
- filename: zededa-kubernetes_service-openapi.json
  format: json
  label: ZEDEDA Kubernetes Service (ZKS)
  slug: zededa-kubernetes-service-zks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-kubernetes_service-openapi.json
- filename: zededa-node_cluster_service-openapi.json
  format: json
  label: ZEDEDA Edge-Node Cluster Service
  slug: zededa-edge-node-cluster-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-node_cluster_service-openapi.json
- filename: zededa-user_service-openapi.json
  format: json
  label: ZEDEDA IAM Service
  slug: zededa-iam-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-user_service-openapi.json
- filename: zededa-job_service-openapi.json
  format: json
  label: ZEDEDA Job Service
  slug: zededa-job-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-job_service-openapi.json
- filename: zededa-diag_service-openapi.json
  format: json
  label: ZEDEDA Diagnostics Service
  slug: zededa-diagnostics-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-diag_service-openapi.json
consequence_counts:
  physical: 11
  read: 242
  safety-critical: 5
  write: 163
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Zededa Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/devices/id/{id}/debug/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/devices/id/{id}/edgeview/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/devices/id/{id}/preparepoweroff
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/devices/id/{id}/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/login/forgot
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/cluster/instances/kubernetes/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/cluster/instances/kubernetes/deployments/id/{deploymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/cluster/instances/kubernetes/deployments/id/{deploymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/jobs/devices/deployment/tags
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/profiledeployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/profiledeployments/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/profiledeployments/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/projects/id/{projectId}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/projects/id/{projectId}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/projects/id/{projectId}/deployments/id/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/projects/id/{projectId}/deployments/id/{id}
operation_count: 421
overview: 'Zededa exposes 421 API operations that an AI agent could call, of which 179 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 242 read, 163 write, 11 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zededa
provider_slug: zededa
slug: zededa-agentic-access
source_filename: zededa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/zededa-app_profile_service-openapi.json, openapi/zededa-app_service-openapi.json,\n  openapi/zededa-diag_service-openapi.json, openapi/zededa-job_service-openapi.json, openapi/zededa-kubernetes_service-openapi.json,\n  openapi/zededa-network_service-openapi.json, openapi/zededa-node_cluster_service-openapi.json,\n  openapi/zededa-node_service-openapi.json, openapi/zededa-storage_service-openapi.json, openapi/zededa-user_service-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 421\n  by_action_class:\n    connected: 242\n    acting: 179\n  by_consequence:\n    read: 242\n    write: 163\n    physical: 11\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n\
  - path: /v1/appprofiles\n  method: get\n  operationId: AppProfileService_QueryAppProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appprofiles\n  method: post\n  operationId: AppProfileService_CreateAppProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appprofiles/id/{id}\n  method: get\n  operationId: AppProfileService_GetAppProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appprofiles/id/{id}\n  method: delete\n  operationId: AppProfileService_DeleteAppProfile\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appprofiles/id/{id}\n  method: put\n  operationId: AppProfileService_UpdateAppProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/appprofiles/id/{id}/version\n  method: get\n  operationId: AppProfileService_QueryAppProfileRevisionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appprofiles/name/{name}\n  method: get\n  operationId: AppProfileService_GetAppProfileByName\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/appprofiles/name/{name}/version\n  method: get\n  operationId: AppProfileService_QueryAppProfileRevisionByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assetgroups\n  method: get\n  operationId: AssetGroupService_QueryAssetGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assetgroups\n  method: post\n  operationId: AssetGroupService_CreateAssetGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/assetgroups/id/{id}\n  method: get\n  operationId: AssetGroupService_GetAssetGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assetgroups/id/{id}\n  method: delete\n  operationId: AssetGroupService_DeleteAssetGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/assetgroups/id/{id}\n  method: put\n  operationId: AssetGroupService_UpdateAssetGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/assetgroups/name/{name}\n  method: get\n  operationId: AssetGroupService_GetAssetGroupByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiledeployments\n  method: get\n  operationId: ProfileDeploymentService_QueryProfileDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiledeployments\n  method: post\n  operationId: ProfileDeploymentService_CreateProfileDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiledeployments/id/{id}\n  method: get\n\
  \  operationId: ProfileDeploymentService_GetProfileDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiledeployments/id/{id}\n  method: delete\n  operationId: ProfileDeploymentService_DeleteProfileDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiledeployments/id/{id}\n  method: put\n  operationId: ProfileDeploymentService_UpdateProfileDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiledeployments/id/{id}/resourcestatus\n  method: get\n  operationId: ProfileDeploymentService_QueryProfileDeploymentResourceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiledeployments/name/{name}\n  method: get\n  operationId: ProfileDeploymentService_GetProfileDeploymentByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beta/apps\n  method: get\n  operationId: EdgeApplicationConfiguration_QueryBetaEdgeApplicationBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps\n  method: get\n  operationId: EdgeApplicationConfiguration_QueryEdgeApplicationBundles\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps\n  method: post\n  operationId: EdgeApplicationConfiguration_CreateEdgeApplicationBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/global\n  method: get\n  operationId: EdgeApplicationConfiguration_QueryGlobalEdgeApplicationBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/global/id/{id}\n  method: get\n  operationId: EdgeApplicationConfiguration_GetGlobalEdgeApplicationBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/global/name/{name}\n  method: get\n  operationId: EdgeApplicationConfiguration_GetGlobalEdgeApplicationBundleByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/id/{id}\n  method: get\n  operationId: EdgeApplicationConfiguration_GetEdgeApplicationBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/id/{id}\n  method: delete\n  operationId: EdgeApplicationConfiguration_DeleteEdgeApplicationBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/apps/id/{id}\n  method: put\n  operationId: EdgeApplicationConfiguration_UpdateEdgeApplicationBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/id/{id}/projects\n  method: get\n  operationId: EdgeApplicationConfiguration_QueryEdgeApplicationBundleProjectList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances\n  method: get\n  operationId: EdgeApplicationInstanceConfiguration_QueryEdgeApplicationInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances\n  method: post\n  operationId: EdgeApplicationInstanceConfiguration_CreateEdgeApplicationInstance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/id/{appInstanceId}/snapshot/name/{name}\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetAppInstanceSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/id/{appInstanceId}/snapshot/name/{name}\n  method: delete\n  operationId: EdgeApplicationInstanceStatus_DeleteAppInstanceSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/apps/instances/id/{id}\n  method: get\n  operationId: EdgeApplicationInstanceConfiguration_GetEdgeApplicationInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/id/{id}\n  method: delete\n  operationId: EdgeApplicationInstanceConfiguration_DeleteEdgeApplicationInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/id/{id}\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_UpdateEdgeApplicationInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/id/{id}/activate\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_ActivateEdgeApplicationInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/id/{id}/console/remote\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_ConnectToEdgeApplicationInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/id/{id}/deactivate\n\
  \  method: put\n  operationId: EdgeApplicationInstanceConfiguration_DeActivateEdgeApplicationInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/id/{id}/flowlog/classification\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceTrafficFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/id/{id}/flowlog/toptalkers\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceTopTalkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/id/{id}/logs\n\
  \  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/id/{id}/opaque-status\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceOpaqueStatusById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/id/{id}/refresh\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_RefreshEdgeApplicationInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/id/{id}/refresh/purge\n\
  \  method: put\n  operationId: EdgeApplicationInstanceConfiguration_RefreshPurgeEdgeApplicationInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/id/{id}/restart\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_RestartEdgeApplicationInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/id/{id}/snapshots\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetAppInstanceSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/id/{id}/status\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/id/{objid}/events\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/id/{objid}/timeSeries/{mType}\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceResourceMetricsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/name/{name}\n\
  \  method: get\n  operationId: EdgeApplicationInstanceConfiguration_GetEdgeApplicationInstanceByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/name/{name}/flowlog/classification\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceTrafficFlows2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/name/{name}/flowlog/toptalkers\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceTopTalkers2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/name/{name}/opaque-status\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceOpaqueStatusByName\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/name/{name}/status\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceStatusByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/name/{objname}/events\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceEventsByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/name/{objname}/timeSeries/{mType}\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceResourceMetricsByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/patch-reference-update\n  method: post\n  operationId: EdgeApplicationInstanceConfiguration_UpdatePatchEnvelopeReferencetoAppInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/instances/snapshot/id/{id}\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetAppInstanceSnapshotByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/snapshot/id/{id}/state\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetAppInstanceSnapshotState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/status\n  method: get\n  operationId: EdgeApplicationInstanceStatus_QueryEdgeApplicationInstanceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/status-config\n  method: get\n  operationId: EdgeApplicationInstanceStatus_QueryEdgeApplicationInstanceStatusConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/instances/tags\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetApplicationInterfaceTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/name/{name}\n  method: get\n  operationId: EdgeApplicationConfiguration_GetEdgeApplicationBundleByName\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patch-envelope\n  method: get\n  operationId: PatchEnvelopeConfiguration_GetPatchEnvelope\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patch-envelope\n  method: post\n  operationId: PatchEnvelopeConfiguration_CreatePatchEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patch-envelope/id/{id}\n  method: get\n  operationId: PatchEnvelopeConfiguration_GetPatchEnvelopeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/patch-envelope/id/{id}\n  method: delete\n  operationId: PatchEnvelopeConfiguration_DeleteAppInstanceSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patch-envelope/id/{id}\n  method: put\n  operationId: PatchEnvelopeConfiguration_UpdatePatchEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patch-envelope/name/{name}\n  method: get\n  operationId: PatchEnvelopeConfiguration_GetPatchEnvelopeByName\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/patch-envelope/status\n  method: get\n  operationId: PatchEnvelopeConfiguration_GetPatchEnvelopeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances\n  method: get\n  operationId: EdgeApplicationInstanceConfiguration_QueryEdgeApplicationInstancesV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances\n  method: post\n  operationId: EdgeApplicationInstanceConfiguration_CreateEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /v2/apps/instances/id/{id}\n  method: get\n  operationId: EdgeApplicationInstanceConfiguration_GetEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/id/{id}\n  method: delete\n  operationId: EdgeApplicationInstanceConfiguration_DeleteEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apps/instances/id/{id}\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_UpdateEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apps/instances/id/{id}/activate\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_ActivateEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apps/instances/id/{id}/console/remote\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_ConnectToEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/apps/instances/id/{id}/deactivate\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_DeActivateEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apps/instances/id/{id}/flowlog/classification\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceTrafficFlowsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/id/{id}/flowlog/toptalkers\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceTopTalkersV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/id/{id}/logs\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceLogsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/id/{id}/opaque-status\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceOpaqueStatusByIdV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/id/{id}/refresh\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_RefreshEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/apps/instances/id/{id}/refresh/purge\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_RefreshPurgeEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apps/instances/id/{id}/restart\n  method: put\n  operationId: EdgeApplicationInstanceConfiguration_RestartEdgeApplicationInstanceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apps/instances/id/{id}/status\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceStatusV2\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/id/{objid}/events\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceEventsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/id/{objid}/timeSeries/{mType}\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceResourceMetricsByIdV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/name/{name}\n  method: get\n  operationId: EdgeApplicationInstanceConfiguration_GetEdgeApplicationInstanceByNameV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/name/{name}/flowlog/classification\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceTrafficFlowsV22\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/name/{name}/flowlog/toptalkers\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceTopTalkersV22\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/name/{name}/opaque-status\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceOpaqueStatusByNameV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/name/{name}/status\n\
  \  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceStatusByNameV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/name/{objname}/events\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceEventsByNameV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/name/{objname}/timeSeries/{mType}\n  method: get\n  operationId: EdgeApplicationInstanceStatus_GetEdgeApplicationInstanceResourceMetricsByNameV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/patch-reference-update\n  method: post\n  operationId: EdgeApplicationInstanceConfiguration_UpdatePatchEnvelopeReferencetoAppInstanceV2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apps/instances/status\n  method: get\n  operationId: EdgeApplicationInstanceStatus_QueryEdgeApplicationInstanceStatusV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps/instances/status-config\n  method: get\n  operationId: EdgeApplicationInstanceStatus_QueryEdgeApplicationInstanceStatusConfigV2\n  x-agentic-access:\n    action-class: connected\n    conseq\n\n# --- truncated at 32 KB (126 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/agentic-access/zededa-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/agentic-access/zededa-agentic-access.yml
summary_line: 421 operations · 179 acting · 5 human-in-the-loop
tags:
- Company
- Edge Computing
- Edge Intelligence
- IoT
- Kubernetes
- Device Management
- Orchestration
- AI at the Edge
---
