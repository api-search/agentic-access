---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 21
api_specs:
- filename: outscale-clusters-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Clusters API
  slug: outscale-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outscale/refs/heads/main/openapi/outscale-clusters-api-openapi.yml
- filename: outscale-myip-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE My Ip API
  slug: outscale-myip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outscale/refs/heads/main/openapi/outscale-myip-api-openapi.yml
- filename: outscale-projects-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Projects API
  slug: outscale-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outscale/refs/heads/main/openapi/outscale-projects-api-openapi.yml
- filename: outscale-quotas-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Quotas API
  slug: outscale-quotas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outscale/refs/heads/main/openapi/outscale-quotas-api-openapi.yml
- filename: outscale-templates-api-openapi.yml
  format: yaml
  label: 3DS OUTSCALE Templates API
  slug: outscale-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outscale/refs/heads/main/openapi/outscale-templates-api-openapi.yml
consequence_counts:
  read: 21
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Outscale Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: '3DS OUTSCALE exposes 28 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 3DS OUTSCALE
provider_slug: outscale
slug: outscale-agentic-access
source_filename: outscale-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/outscale-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 7\n    connected: 21\n  by_consequence:\n    write: 7\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /projects\n  method: post\n  operationId: CreateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: get\n  operationId: ListProjects\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: get\n  operationId: GetProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: patch\n  operationId: UpdateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: delete\n  operationId: DeleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /projects/{project_id}/quotas\n  method: get\n  operationId: GetProjectQuotas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/snapshots\n  method: get\n  operationId: GetProjectSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/public_ips\n  method: get\n  operationId: GetProjectPublicIps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/nets\n  method: get\n  operationId: GetProjectNets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters\n  method: post\n  operationId:\
  \ CreateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters\n  method: get\n  operationId: ListClustersByProjectID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/all\n  method: get\n  operationId: ListAllClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{cluster_id}\n  method: get\n  operationId: GetCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{cluster_id}\n  method: patch\n\
  \  operationId: UpdateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/{cluster_id}\n  method: delete\n  operationId: DeleteCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/{cluster_id}/kubeconfig\n  method: get\n  operationId: GetKubeconfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{cluster_id}/kubeconfig\n  method: post\n  operationId: GetKubeconfigWithPubkeyNACL\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{cluster_id}/upgrade\n  method: patch\n  operationId: UpgradeCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/limits/kubernetes_versions\n  method: get\n  operationId: GetKubernetesVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/limits/cp_subregions\n  method: get\n  operationId: GetCPSubregions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/limits/control_plane_plans\n\
  \  method: get\n  operationId: GetControlPlanePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/project\n  method: get\n  operationId: GetProjectTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/cluster\n  method: get\n  operationId: GetClusterTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/nodepool\n  method: get\n  operationId: GetNodepoolTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/netpeeringrequest\n  method: get\n  operationId: GetNetPeeringRequestTemplate\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/netpeeringacceptance\n  method: get\n  operationId: GetNetPeeringAcceptanceTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotas\n  method: get\n  operationId: GetQuotas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myip\n  method: get\n  operationId: GetClientIP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outscale/refs/heads/main/agentic-access/outscale-agentic-access.yml
summary_line: 28 operations · 7 acting
tags:
- Cloud
- IaaS
- Compute
- Storage
- Networking
---
