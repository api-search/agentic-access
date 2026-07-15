---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 57
api_specs:
- filename: weblogic-restful-management-services-openapi.yml
  format: yaml
  label: WebLogic RESTful Management Services API
  slug: weblogic-restful-management-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-restful-management-services-openapi.yml
- filename: weblogic-monitoring-diagnostics-openapi.yml
  format: yaml
  label: WebLogic Monitoring and Diagnostics API
  slug: weblogic-monitoring-and-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-monitoring-diagnostics-openapi.yml
- filename: weblogic-deployment-openapi.yml
  format: yaml
  label: WebLogic Deployment API
  slug: weblogic-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/openapi/weblogic-deployment-openapi.yml
consequence_counts:
  physical: 12
  read: 57
  safety-critical: 4
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Weblogic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /domainRuntime/deploymentManager/stopApplication
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
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /lifecycle/latest/servers/{serverName}/shutdown
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainRuntime/deploymentManager/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainRuntime/deploymentManager/redeploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainRuntime/deploymentManager/startApplication
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainRuntime/deploymentManager/undeploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /domainRuntime/deploymentManager/upload
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
  method: DELETE
  path: /edit/appDeployments/{appName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edit/libraries
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /edit/libraries/{libraryName}
operation_count: 95
overview: 'Oracle WebLogic Server APIs exposes 95 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 57 read, 22 write, 12 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oracle WebLogic Server APIs
provider_slug: weblogic
slug: weblogic-agentic-access
source_filename: weblogic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/weblogic-deployment-openapi.yml, openapi/weblogic-monitoring-diagnostics-openapi.yml,\n  openapi/weblogic-restful-management-services-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 95\n  by_action_class:\n    connected: 57\n    acting: 38\n  by_consequence:\n    read: 57\n    physical: 12\n    safety-critical: 4\n    write: 22\n  human_in_the_loop_required: 4\noperations:\n- path: /edit/appDeployments\n  method: get\n  operationId: listAppDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments\n  method: post\n  operationId: createAppDeployment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeployments/{appName}\n  method: get\n  operationId: getAppDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments/{appName}\n  method: post\n  operationId: updateAppDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeployments/{appName}\n\
  \  method: delete\n  operationId: deleteAppDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/libraries\n  method: get\n  operationId: listLibraries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/libraries\n  method: post\n  operationId: createLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /edit/libraries/{libraryName}\n  method: get\n  operationId: getLibrary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/libraries/{libraryName}\n  method: delete\n  operationId: deleteLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/deploymentManager/deploy\n  method: post\n  operationId: deploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/deploymentManager/undeploy\n  method: post\n  operationId: undeploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/deploymentManager/redeploy\n  method: post\n  operationId: redeploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/deploymentManager/startApplication\n  method: post\n  operationId: startApplication\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/deploymentManager/stopApplication\n  method: post\n  operationId: stopApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /domainRuntime/deploymentManager/deploymentProgressObjects\n  method: get\n  operationId: listDeploymentProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /domainRuntime/deploymentManager/deploymentProgressObjects/{taskId}\n  method: get\n  operationId: getDeploymentProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainRuntime/deploymentManager/upload\n  method: post\n  operationId: uploadApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers\n  method: get\n  operationId: getServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{serverName}\n  method: get\n  operationId: getServer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{serverName}/health\n  method: get\n  operationId: getServerHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{serverName}/jvm\n  method: get\n  operationId: getServerJVM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{serverName}/threadPool\n  method: get\n  operationId: getServerThreadPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{serverName}/workManagers\n  method: get\n  operationId: getServerWorkManagers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters\n  method: get\n  operationId: getClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{clusterName}\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataSources\n  method: get\n  operationId: getDataSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataSources/{dataSourceName}\n  method: get\n  operationId: getDataSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataSources/{dataSourceName}/test\n \
  \ method: post\n  operationId: testDataSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /JMSServers\n  method: get\n  operationId: getJMSServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /JMSServers/{jmsServerName}\n  method: get\n  operationId: getJMSServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /JMSServers/{jmsServerName}/destinations\n  method: get\n  operationId: getJMSDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /deployments\n  method: get\n  operationId: getDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/{appName}\n  method: get\n  operationId: getDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/{appName}/servlets\n  method: get\n  operationId: getDeploymentServlets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/WLDFSystemResources\n  method: get\n  operationId: getWLDFResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/WLDFSystemResources/{resourceName}\n  method: get\n  operationId:\
  \ getWLDFResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/dataAccessRuntimes\n  method: get\n  operationId: getDataAccessRuntimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /diagnostics/dataAccessRuntimes/{runtimeName}/query\n  method: post\n  operationId: queryDiagnosticData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit\n  method: get\n  operationId: getEditRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /edit/changeManager/startEdit\n  method: post\n  operationId: startEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/changeManager/activate\n  method: post\n  operationId: activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/changeManager/cancelEdit\n  method: post\n  operationId: cancelEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/changeManager/undoUnactivatedChanges\n  method: post\n  operationId: undoUnactivatedChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/servers\n  method: get\n  operationId: getEditServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/servers\n  method: post\n  operationId: createEditServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /edit/servers/{serverName}\n  method: get\n  operationId: getEditServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/servers/{serverName}\n  method: post\n  operationId: updateEditServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/servers/{serverName}\n  method: delete\n  operationId: deleteEditServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/clusters\n\
  \  method: get\n  operationId: getEditClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/clusters\n  method: post\n  operationId: createEditCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/clusters/{clusterName}\n  method: get\n  operationId: getEditCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/clusters/{clusterName}\n  method: post\n  operationId: updateEditCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/clusters/{clusterName}\n  method: delete\n  operationId: deleteEditCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JDBCSystemResources\n  method: get\n  operationId: getEditDataSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JDBCSystemResources\n  method: post\n  operationId: createEditDataSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JDBCSystemResources/{dataSourceName}\n  method: get\n  operationId: getEditDataSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JDBCSystemResources/{dataSourceName}\n  method: delete\n  operationId: deleteEditDataSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/JMSSystemResources\n  method: get\n  operationId: getEditJMSResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/JMSSystemResources\n  method: post\n\
  \  operationId: createEditJMSResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeployments\n  method: get\n  operationId: getEditAppDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments\n  method: post\n  operationId: createEditAppDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edit/appDeployments/{appName}\n\
  \  method: get\n  operationId: getEditAppDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edit/appDeployments/{appName}\n  method: delete\n  operationId: deleteEditAppDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainConfig\n  method: get\n  operationId: getDomainConfigRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainConfig/servers\n  method: get\n  operationId: getDomainConfigServers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainConfig/servers/{serverName}\n  method: get\n  operationId: getDomainConfigServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainConfig/clusters\n  method: get\n  operationId: getDomainConfigClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainConfig/securityConfiguration\n  method: get\n  operationId: getDomainSecurityConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainRuntime\n  method: get\n  operationId: getDomainRuntimeRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /domainRuntime/serverLifeCycleRuntimes\n  method: get\n  operationId: getServerLifecycleRuntimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainRuntime/serverLifeCycleRuntimes/{serverName}\n  method: get\n  operationId: getServerLifecycleRuntime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainRuntime/serverLifeCycleRuntimes/{serverName}/start\n  method: post\n  operationId: startServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/serverLifeCycleRuntimes/{serverName}/shutdown\n\
  \  method: post\n  operationId: shutdownServer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /domainRuntime/serverLifeCycleRuntimes/{serverName}/forceShutdown\n  method: post\n  operationId: forceShutdownServer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /domainRuntime/serverLifeCycleRuntimes/{serverName}/suspend\n  method: post\n  operationId: suspendServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/serverLifeCycleRuntimes/{serverName}/resume\n  method: post\n  operationId: resumeServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/serverLifeCycleRuntimes/{serverName}/restartSSL\n  method: post\n  operationId: restartSSL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainRuntime/serverRuntimes\n\
  \  method: get\n  operationId: getDomainServerRuntimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainRuntime/serverRuntimes/{serverName}\n  method: get\n  operationId: getDomainServerRuntime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainRuntime/deploymentManager/deploymentProgressObjects\n  method: get\n  operationId: getDeploymentProgressObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverConfig\n  method: get\n  operationId: getServerConfigRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime\n  method: get\n  operationId:\
  \ getServerRuntimeRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime/JVMRuntime\n  method: get\n  operationId: getJVMRuntime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime/threadPoolRuntime\n  method: get\n  operationId: getThreadPoolRuntime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime/JDBCServiceRuntime\n  method: get\n  operationId: getJDBCServiceRuntime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime/JDBCServiceRuntime/JDBCDataSourceRuntimeMBeans\n  method: get\n  operationId: getJDBCDataSourceRuntimes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime/JDBCServiceRuntime/JDBCDataSourceRuntimeMBeans/{dataSourceName}\n  method: get\n  operationId: getJDBCDataSourceRuntime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime/JMSRuntime\n  method: get\n  operationId: getJMSRuntime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime/JMSRuntime/JMSServers\n  method: get\n  operationId: getJMSServerRuntimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime/applicationRuntimes\n  method: get\n  operationId: getApplicationRuntimes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverRuntime/applicationRuntimes/{appName}\n  method: get\n  operationId: getApplicationRuntime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lifecycle/latest/servers/{serverName}/shutdown\n  method: post\n  operationId: lifecycleShutdownServer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /lifecycle/latest/servers/{serverName}/start\n  method: post\n  operationId: lifecycleStartServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lifecycle/latest/servers/{serverName}/suspend\n  method: post\n  operationId: lifecycleSuspendServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lifecycle/latest/servers/{serverName}/resume\n  method: post\n  operationId: lifecycleResumeServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/agentic-access/weblogic-agentic-access.yml
summary_line: 95 operations · 38 acting · 4 human-in-the-loop
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
- WebLogic
---
