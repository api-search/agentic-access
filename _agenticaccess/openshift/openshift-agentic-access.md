---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 20
api_specs:
- filename: swagger.json
  format: json
  label: OpenShift REST API
  slug: openshift-rest-api
  spec_type: OpenAPI
  url: https://api.openshift.com/api/swagger.json
consequence_counts:
  physical: 7
  read: 20
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openshift Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}/rollback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}/scale
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}/status
operation_count: 42
overview: 'OpenShift exposes 42 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 15 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenShift
provider_slug: openshift
slug: openshift-agentic-access
source_filename: openshift-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openshift-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 20\n    acting: 22\n  by_consequence:\n    read: 20\n    write: 15\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /apis/route.openshift.io/v1/routes\n  method: get\n  operationId: listRouteForAllNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/route.openshift.io/v1/namespaces/{namespace}/routes\n  method: get\n  operationId: listNamespacedRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/route.openshift.io/v1/namespaces/{namespace}/routes\n  method: post\n  operationId: createNamespacedRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/route.openshift.io/v1/namespaces/{namespace}/routes/{name}\n  method: get\n  operationId: readNamespacedRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/route.openshift.io/v1/namespaces/{namespace}/routes/{name}\n  method: put\n  operationId: replaceNamespacedRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/route.openshift.io/v1/namespaces/{namespace}/routes/{name}\n  method: patch\n  operationId: patchNamespacedRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/route.openshift.io/v1/namespaces/{namespace}/routes/{name}\n  method: delete\n  operationId: deleteNamespacedRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/route.openshift.io/v1/namespaces/{namespace}/routes/{name}/status\n\
  \  method: get\n  operationId: readNamespacedRouteStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/route.openshift.io/v1/namespaces/{namespace}/routes/{name}/status\n  method: put\n  operationId: replaceNamespacedRouteStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/build.openshift.io/v1/builds\n  method: get\n  operationId: listBuildForAllNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/builds\n  method: get\n  operationId: listNamespacedBuild\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/builds\n  method: post\n  operationId: createNamespacedBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/builds/{name}\n  method: get\n  operationId: readNamespacedBuild\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/builds/{name}\n  method: put\n  operationId: replaceNamespacedBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/builds/{name}\n  method: delete\n  operationId: deleteNamespacedBuild\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/builds/{name}/log\n  method: get\n  operationId: readNamespacedBuildLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/build.openshift.io/v1/buildconfigs\n  method: get\n  operationId: listBuildConfigForAllNamespaces\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/buildconfigs\n  method: get\n  operationId: listNamespacedBuildConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/buildconfigs\n  method: post\n  operationId: createNamespacedBuildConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/buildconfigs/{name}\n  method: get\n  operationId: readNamespacedBuildConfig\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/buildconfigs/{name}\n  method: put\n  operationId: replaceNamespacedBuildConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/buildconfigs/{name}\n  method: delete\n  operationId: deleteNamespacedBuildConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/build.openshift.io/v1/namespaces/{namespace}/buildconfigs/{name}/instantiate\n\
  \  method: post\n  operationId: createNamespacedBuildConfigInstantiate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.openshift.io/v1/deploymentconfigs\n  method: get\n  operationId: listDeploymentConfigForAllNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs\n  method: get\n  operationId: listNamespacedDeploymentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs\n  method: post\n  operationId:\
  \ createNamespacedDeploymentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}\n  method: get\n  operationId: readNamespacedDeploymentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}\n  method: put\n  operationId: replaceNamespacedDeploymentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}\n  method: patch\n  operationId: patchNamespacedDeploymentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}\n  method: delete\n  operationId: deleteNamespacedDeploymentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}/status\n  method: get\n  operationId: readNamespacedDeploymentConfigStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}/status\n  method: put\n  operationId: replaceNamespacedDeploymentConfigStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}/scale\n  method: get\n  operationId:\
  \ readNamespacedDeploymentConfigScale\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}/scale\n  method: put\n  operationId: replaceNamespacedDeploymentConfigScale\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}/rollback\n  method: post\n  operationId: createNamespacedDeploymentConfigRollback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.openshift.io/v1/namespaces/{namespace}/deploymentconfigs/{name}/log\n  method: get\n  operationId: readNamespacedDeploymentConfigLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/project.openshift.io/v1/projects\n  method: get\n  operationId: listProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/project.openshift.io/v1/projects/{name}\n  method: get\n  operationId: readProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/project.openshift.io/v1/projects/{name}\n\
  \  method: put\n  operationId: replaceProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/project.openshift.io/v1/projects/{name}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/project.openshift.io/v1/projectrequests\n  method: get\n  operationId: listProjectRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/project.openshift.io/v1/projectrequests\n\
  \  method: post\n  operationId: createProjectRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/agentic-access/openshift-agentic-access.yml
summary_line: 42 operations · 22 acting
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
---
