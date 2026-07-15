---
acting_count: 74
action_class_counts:
  acting: 74
  connected: 69
api_specs:
- filename: oracle-weblogic-management-openapi.yml
  format: yaml
  label: WebLogic RESTful Management Services API
  slug: weblogic-restful-management-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/openapi/oracle-weblogic-management-openapi.yml
- filename: oracle-weblogic-monitoring-openapi.yml
  format: yaml
  label: WebLogic Monitoring and Diagnostics API
  slug: weblogic-monitoring-and-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/openapi/oracle-weblogic-monitoring-openapi.yml
- filename: oracle-weblogic-deployment-openapi.yml
  format: yaml
  label: WebLogic Deployment API
  slug: weblogic-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/openapi/oracle-weblogic-deployment-openapi.yml
consequence_counts:
  physical: 17
  read: 69
  safety-critical: 5
  write: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Oracle Weblogic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /domainRuntime/appDeploymentRuntimes/{appName}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /domainRuntime/appDeploymentRuntimes/{appName}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /domainRuntime/domainPartitionRuntimes/{partitionName}/partitionLifeCycleRuntime/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /domainRuntime/serverLifeCycleRuntimes/{serverName}/forceShutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /domainRuntime/serverLifeCycleRuntimes/{serverName}/shutdown
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainRuntime/appDeploymentRuntimes/{appName}/redeploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainRuntime/appDeploymentRuntimes/{appName}/start
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainRuntime/appDeploymentRuntimes/{appName}/start
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainRuntime/appDeploymentRuntimes/{appName}/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/JMSSystemResources/{jmsResourceName}/subDeployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/appDeployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/appDeployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/appDeployments/{appName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /edit/appDeployments/{appName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/appDeployments/{appName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /edit/appDeployments/{appName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/appDeployments/{appName}/subDeployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/changeManager/activate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/changeManager/startEdit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/libDeployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/libDeployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /edit/libDeployments/{libName}
operation_count: 143
overview: 'Oracle WebLogic Server exposes 143 API operations that an AI agent could call, of which 74 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 69 read, 52 write, 17 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oracle WebLogic Server
provider_slug: oracle-weblogic
slug: oracle-weblogic-agentic-access
source_filename: oracle-weblogic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/oracle-weblogic-deployment-openapi.yml, openapi/oracle-weblogic-management-openapi.yml,\n  openapi/oracle-weblogic-monitoring-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 143\n  by_action_class:\n    acting: 74\n    connected: 69\n  by_consequence:\n    physical: 17\n    read: 69\n    safety-critical: 5\n    write: 52\n  human_in_the_loop_required: 5\noperations:\n- path: /edit/changeManager/startEdit\n  method: post\n  operationId: startEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/changeManager/activate\n  method: post\n  operationId: activateDeploymentChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeployments\n  method: get\n  operationId: listAppDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments\n  method: post\n  operationId: deployApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n   \
  \   purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeploymentCreateForm\n  method: get\n  operationId: getAppDeploymentCreateForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments/{appName}\n  method: get\n  operationId: getAppDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments/{appName}\n  method: post\n  operationId: updateAppDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeployments/{appName}\n  method: delete\n  operationId: undeployApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/libDeployments\n  method: get\n  operationId: listLibDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/libDeployments\n  method: post\n  operationId: deployLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/libDeployments/{libName}\n  method: get\n  operationId: getLibDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/libDeployments/{libName}\n  method: delete\n  operationId: undeployLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/appDeploymentRuntimes\n  method: get\n  operationId: listDeploymentRuntimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /domainRuntime/appDeploymentRuntimes/{appName}/start\n  method: post\n  operationId: startApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/appDeploymentRuntimes/{appName}/stop\n  method: post\n  operationId: stopApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /domainRuntime/appDeploymentRuntimes/{appName}/redeploy\n  method: post\n  operationId: redeployApplication\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/appDeploymentRuntimes/{appName}/update\n  method: post\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/appDeploymentRuntimes/{appName}/tasks/{taskId}\n  method: get\n  operationId: getDeploymentTaskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainRuntime/serverRuntimes/{serverName}/applicationRuntimes\n  method: get\n  operationId: listServerApplicationRuntimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments/{appName}/subDeployments\n  method: get\n  operationId: listAppSubDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments/{appName}/subDeployments\n  method: post\n  operationId: createAppSubDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /edit/changeManager/startEdit\n  method: post\n  operationId: startEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/changeManager/activate\n  method: post\n  operationId: activateChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/changeManager/cancelEdit\n  method: post\n  operationId: cancelEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/changeManager/undoUnactivatedChanges\n  method: post\n  operationId: undoUnactivatedChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/servers\n  method: get\n  operationId: listServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/servers\n  method: post\n  operationId: createServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /edit/serverCreateForm\n  method: get\n  operationId: getServerCreateForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/servers/{serverName}\n  method: get\n  operationId: getServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/servers/{serverName}\n  method: post\n  operationId: updateServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/servers/{serverName}\n  method: delete\n  operationId: deleteServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/servers/{serverName}/SSL\n  method: get\n  operationId: getServerSSL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/servers/{serverName}/SSL\n  method: post\n  operationId: updateServerSSL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/servers/{serverName}/serverStart\n  method: get\n  operationId: getServerStart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /edit/servers/{serverName}/serverStart\n  method: post\n  operationId: updateServerStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/servers/{serverName}/networkAccessPoints\n  method: get\n  operationId: listNetworkAccessPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/servers/{serverName}/networkAccessPoints\n  method: post\n  operationId: createNetworkAccessPoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /edit/clusters\n  method: get\n  operationId: listClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/clusters\n  method: post\n  operationId: createCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/clusterCreateForm\n  method: get\n  operationId: getClusterCreateForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/clusters/{clusterName}\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/clusters/{clusterName}\n  method: post\n  operationId: updateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/clusters/{clusterName}\n  method: delete\n  operationId: deleteCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/clusters/{clusterName}/dynamicServers\n  method: get\n  operationId: getDynamicServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /edit/clusters/{clusterName}/dynamicServers\n  method: post\n  operationId: updateDynamicServers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/machines\n  method: get\n  operationId: listMachines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/machines\n  method: post\n  operationId: createMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/machines/{machineName}\n\
  \  method: get\n  operationId: getMachine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/machines/{machineName}\n  method: post\n  operationId: updateMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/machines/{machineName}\n  method: delete\n  operationId: deleteMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/machines/{machineName}/nodeManager\n  method: get\n  operationId: getNodeManager\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/machines/{machineName}/nodeManager\n  method: post\n  operationId: updateNodeManager\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/serverTemplates\n  method: get\n  operationId: listServerTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/serverTemplates\n  method: post\n  operationId: createServerTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/serverTemplates/{templateName}\n  method: get\n  operationId: getServerTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/serverTemplates/{templateName}\n  method: post\n  operationId: updateServerTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/serverTemplates/{templateName}\n  method: delete\n  operationId: deleteServerTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JDBCSystemResources\n  method: get\n  operationId: listJDBCSystemResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JDBCSystemResources\n  method: post\n  operationId: createJDBCSystemResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JDBCSystemResources/{resourceName}\n  method: get\n  operationId: getJDBCSystemResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JDBCSystemResources/{resourceName}\n\
  \  method: delete\n  operationId: deleteJDBCSystemResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JDBCSystemResources/{resourceName}/JDBCResource\n  method: get\n  operationId: getJDBCResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JDBCSystemResources/{resourceName}/JDBCResource\n  method: post\n  operationId: updateJDBCResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JDBCSystemResources/{resourceName}/JDBCResource/JDBCDataSourceParams\n\
  \  method: get\n  operationId: getJDBCDataSourceParams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JDBCSystemResources/{resourceName}/JDBCResource/JDBCDataSourceParams\n  method: post\n  operationId: updateJDBCDataSourceParams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JDBCSystemResources/{resourceName}/JDBCResource/JDBCDriverParams\n  method: get\n  operationId: getJDBCDriverParams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JDBCSystemResources/{resourceName}/JDBCResource/JDBCDriverParams\n  method: post\n  operationId:\
  \ updateJDBCDriverParams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JDBCSystemResources/{resourceName}/JDBCResource/JDBCDriverParams/properties/properties\n  method: get\n  operationId: listJDBCProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JDBCSystemResources/{resourceName}/JDBCResource/JDBCDriverParams/properties/properties\n  method: post\n  operationId: createJDBCProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /edit/JMSServers\n  method: get\n  operationId: listJMSServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JMSServers\n  method: post\n  operationId: createJMSServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JMSServers/{jmsServerName}\n  method: get\n  operationId: getJMSServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JMSServers/{jmsServerName}\n  method: delete\n  operationId: deleteJMSServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JMSSystemResources\n  method: get\n  operationId: listJMSSystemResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JMSSystemResources\n  method: post\n  operationId: createJMSSystemResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JMSSystemResources/{jmsResourceName}/JMSResource/connectionFactories\n  method: get\n  operationId: listJMSConnectionFactories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JMSSystemResources/{jmsResourceName}/JMSResource/connectionFactories\n  method: post\n  operationId: createJMSConnectionFactory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JMSSystemResources/{jmsResourceName}/JMSResource/uniformDistributedQueues\n  method: get\n  operationId: listJMSDistributedQueues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JMSSystemResources/{jmsResourceName}/JMSResource/uniformDistributedQueues\n  method: post\n  operationId: createJMSDistributedQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JMSSystemResources/{jmsResourceName}/subDeployments\n  method: get\n  operationId: listJMSSubDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JMSSystemResources/{jmsResourceName}/subDeployments\n  method: post\n  operationId: createJMSSubDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/fileStores\n  method: get\n  operationId: listFileStores\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/fileStores\n  method: post\n  operationId: createFileStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeployments\n  method: get\n  operationId: listAppDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments\n  method: post\n  operationId: createAppDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeployments/{appName}\n  method: get\n  operationId: getAppDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments/{appName}\n  method: post\n  operationId: updateAppDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeployments/{appName}\n  method: delete\n  operationId: deleteAppDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/libDeployments\n  method: get\n  operationId: listLibDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/libDeployments\n  method: post\n  operationId: createLibDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/securityConfiguration/realms\n  method: get\n  operationId: listSecurityRealms\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/securityConfiguration/realms\n  method: post\n  operationId: createSecurityRealm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/securityConfiguration/realms/{realmName}\n  method: get\n  operationId: getSecurityRealm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/securityConfiguration/realms/{realmName}\n  method: post\n  operationId: updateSecurityRealm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/securityConfiguration/realms/{realmName}/authenticationProviders\n  method: get\n  operationId: listAuthenticationProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/securityConfiguration/realms/{realmName}/authenticationProviders\n  method: post\n  operationId: createAuthenticationProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serverConfig/securityConfiguration/realms/{realmName}/authenticationProviders/{providerName}/createUser\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serverConfig/securityConfiguration/realms/{realmName}/authenticationProviders/{providerName}/addMemberToGroup\n  method: post\n  operationId: addMemberToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit\n  method: get\n  operationId: getEditRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverConfig\n  method: get\n  operationId: getServerConfig\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainConfig\n  method: get\n  operationId: getDomainConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/search\n  method: post\n  operationId: searchEditTree\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainConfig/search\n  method: post\n  operationId: searchDomainConfigTree\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: req\n\n# --- truncated at 32 KB (43 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/agentic-access/oracle-weblogic-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/agentic-access/oracle-weblogic-agentic-access.yml
summary_line: 143 operations · 74 acting · 5 human-in-the-loop
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
---
