---
acting_count: 137
action_class_counts:
  acting: 137
  connected: 144
api_specs:
- filename: oracle-goldengate-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate REST API
  slug: oracle-goldengate-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-rest-api-openapi.yml
- filename: oracle-goldengate-big-data-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate for Big Data REST API
  slug: oracle-goldengate-for-big-data-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-big-data-rest-api-openapi.yml
- filename: oracle-goldengate-veridata-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Veridata REST API
  slug: oracle-goldengate-veridata-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-veridata-rest-api-openapi.yml
- filename: oracle-goldengate-cloud-service-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Cloud Service API
  slug: oracle-goldengate-cloud-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-cloud-service-api-openapi.yml
- filename: oracle-goldengate-stream-analytics-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Stream Analytics REST API
  slug: oracle-goldengate-stream-analytics-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-stream-analytics-rest-api-openapi.yml
- filename: oracle-goldengate-data-streams-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Data Streams REST API
  slug: oracle-goldengate-data-streams-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-data-streams-rest-api-openapi.yml
consequence_counts:
  physical: 17
  read: 144
  safety-critical: 7
  write: 113
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Oracle Goldengate Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /20200407/deployments/{deploymentId}/actions/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /20200407/pipelines/{pipelineId}/actions/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /services/configuration/profiles/{Id}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /services/execution/jobs/{runId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /services/repair/jobs/{runId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /services/server/configuration/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /services/v2/currentuser
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /20200407/deploymentBackups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /20200407/deploymentBackups/{deploymentBackupId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /20200407/deploymentBackups/{deploymentBackupId}/actions/restore
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /20200407/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /20200407/deployments/{deploymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /20200407/deployments/{deploymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /20200407/deployments/{deploymentId}/actions/changeCompartment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /20200407/deployments/{deploymentId}/actions/collectDiagnostics
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /20200407/deployments/{deploymentId}/actions/start
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /20200407/deployments/{deploymentId}/actions/upgrade
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /20200407/deployments/{deploymentId}/certificates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /services/v2/deployments/{deployment}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /services/v2/deployments/{deployment}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /services/v2/deployments/{deployment}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /services/v2/deployments/{deployment}/services/{service}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /services/v2/deployments/{deployment}/services/{service}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /services/v2/deployments/{deployment}/services/{service}
operation_count: 281
overview: 'Oracle GoldenGate exposes 281 API operations that an AI agent could call, of which 137 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 144 read, 113 write, 17 physical, and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
slug: oracle-goldengate-agentic-access
source_filename: oracle-goldengate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/oracle-goldengate-big-data-rest-api-openapi.yml, openapi/oracle-goldengate-cloud-service-api-openapi.yml,\n  openapi/oracle-goldengate-data-streams-rest-api-openapi.yml, openapi/oracle-goldengate-rest-api-openapi.yml,\n  openapi/oracle-goldengate-stream-analytics-rest-api-openapi.yml, openapi/oracle-goldengate-veridata-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 281\n  by_action_class:\n    connected: 144\n    acting: 137\n  by_consequence:\n    read: 144\n    write: 113\n    physical: 17\n    safety-critical: 7\n  human_in_the_loop_required: 7\noperations:\n- path: /services/v2/config/health\n  method: get\n  operationId: getServiceHealth\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/extracts\n  method: get\n  operationId: listExtracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/extracts/{extract}\n  method: get\n  operationId: getExtract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/extracts/{extract}\n  method: post\n  operationId: createExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/extracts/{extract}\n  method: patch\n \
  \ operationId: updateExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/extracts/{extract}\n  method: delete\n  operationId: deleteExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/extracts/{extract}/command\n  method: post\n  operationId: issueExtractCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /services/v2/replicats\n  method: get\n  operationId: listReplicats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/replicats/{replicat}\n  method: get\n  operationId: getReplicat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/replicats/{replicat}\n  method: post\n  operationId: createReplicat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/replicats/{replicat}\n  method: patch\n  operationId: updateReplicat\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/replicats/{replicat}\n  method: delete\n  operationId: deleteReplicat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/replicats/{replicat}/command\n  method: post\n  operationId: issueReplicatCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/replicats/{replicat}/info/status\n\
  \  method: get\n  operationId: getReplicatStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/dataTargetTypes\n  method: get\n  operationId: listDataTargetTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/dataTargetTypes/{dataTargetType}\n  method: get\n  operationId: getDataTargetTypeSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/credentials\n  method: get\n  operationId: listCredentialDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/credentials/{domain}/{alias}\n  method: get\n  operationId:\
  \ getCredentialAlias\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/credentials/{domain}/{alias}\n  method: post\n  operationId: createCredentialAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/credentials/{domain}/{alias}\n  method: put\n  operationId: replaceCredentialAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/credentials/{domain}/{alias}\n  method: delete\n\
  \  operationId: deleteCredentialAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/config/files\n  method: get\n  operationId: listConfigFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/config/files/{file}\n  method: get\n  operationId: getConfigFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/config/files/{file}\n  method: post\n  operationId: createConfigFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/config/files/{file}\n  method: put\n  operationId: replaceConfigFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/config/files/{file}\n  method: delete\n  operationId: deleteConfigFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/trails\n  method: get\n  operationId: listTrails\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/sources\n  method: get\n  operationId: listDistributionPaths\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/sources/{distpath}\n  method: get\n  operationId: getDistributionPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/sources/{distpath}\n  method: post\n  operationId: createDistributionPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/sources/{distpath}\n  method: delete\n  operationId:\
  \ deleteDistributionPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/commands/execute\n  method: post\n  operationId: executeCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/mpoints/processes\n  method: get\n  operationId: listProcessMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/mpoints/{item}/statisticsReplicat\n  method: get\n  operationId: getReplicatStats\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/deployments\n  method: get\n  operationId: listDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/deployments\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/deployments/{deploymentId}\n  method: get\n  operationId: getDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /20200407/deployments/{deploymentId}\n  method: put\n  operationId: updateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/deployments/{deploymentId}\n  method: delete\n  operationId: deleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/deployments/{deploymentId}/actions/start\n  method: post\n  operationId: startDeployment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/deployments/{deploymentId}/actions/stop\n  method: post\n  operationId: stopDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /20200407/deployments/{deploymentId}/actions/upgrade\n  method: post\n  operationId: upgradeDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/deployments/{deploymentId}/actions/changeCompartment\n  method: post\n  operationId: changeDeploymentCompartment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/deployments/{deploymentId}/actions/collectDiagnostics\n  method: post\n  operationId: collectDeploymentDiagnostics\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/deploymentBackups\n  method: get\n  operationId: listDeploymentBackups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/deploymentBackups\n  method: post\n  operationId: createDeploymentBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/deploymentBackups/{deploymentBackupId}\n  method: get\n  operationId: getDeploymentBackup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /20200407/deploymentBackups/{deploymentBackupId}\n  method: delete\n  operationId: deleteDeploymentBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/deploymentBackups/{deploymentBackupId}/actions/restore\n  method: post\n  operationId: restoreDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/connections/{connectionId}\n  method: get\n  operationId: getConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/connections/{connectionId}\n  method: put\n  operationId: updateConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/connections/{connectionId}\n  method: delete\n  operationId: deleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/connectionAssignments\n  method: get\n  operationId: listConnectionAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/connectionAssignments\n  method: post\n  operationId: createConnectionAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/connectionAssignments/{connectionAssignmentId}\n  method: get\n  operationId: getConnectionAssignment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/connectionAssignments/{connectionAssignmentId}\n  method: delete\n  operationId: deleteConnectionAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/databaseRegistrations\n  method: get\n  operationId: listDatabaseRegistrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /20200407/databaseRegistrations\n  method: post\n  operationId: createDatabaseRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/databaseRegistrations/{databaseRegistrationId}\n  method: get\n  operationId: getDatabaseRegistration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/databaseRegistrations/{databaseRegistrationId}\n  method: put\n  operationId: updateDatabaseRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /20200407/databaseRegistrations/{databaseRegistrationId}\n  method: delete\n  operationId: deleteDatabaseRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/pipelines\n  method: get\n  operationId: listPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/pipelines\n  method: post\n  operationId: createPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /20200407/pipelines/{pipelineId}\n  method: get\n  operationId: getPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/pipelines/{pipelineId}\n  method: put\n  operationId: updatePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/pipelines/{pipelineId}\n  method: delete\n  operationId: deletePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/pipelines/{pipelineId}/actions/start\n\
  \  method: post\n  operationId: startPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/pipelines/{pipelineId}/actions/stop\n  method: post\n  operationId: stopPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /20200407/deployments/{deploymentId}/certificates\n  method: get\n  operationId: listCertificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/deployments/{deploymentId}/certificates\n\
  \  method: post\n  operationId: createCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /20200407/workRequests\n  method: get\n  operationId: listWorkRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/workRequests/{workRequestId}\n  method: get\n  operationId: getWorkRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/workRequests/{workRequestId}/logs\n  method: get\n  operationId: listWorkRequestLogs\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/workRequests/{workRequestId}/errors\n  method: get\n  operationId: listWorkRequestErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /20200407/deploymentVersions\n  method: get\n  operationId: listDeploymentVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/stream\n  method: get\n  operationId: listDataStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/stream/{streamname}\n  method: get\n  operationId: getDataStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /services/v2/stream/{streamname}\n  method: post\n  operationId: createDataStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/stream/{streamname}\n  method: patch\n  operationId: updateDataStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/stream/{streamname}\n  method: delete\n  operationId: deleteDataStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/stream/{streamname}/yaml\n  method: get\n  operationId: getAsyncApiSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/stream/{streamname}/yaml\n  method: patch\n  operationId: updateAsyncApiSpec\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services\n  method: get\n  operationId: getApiVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2\n  method:\
  \ get\n  operationId: describeApiVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/config/summary\n  method: get\n  operationId: getConfigSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/config/health\n  method: get\n  operationId: getServiceHealthDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/config/health/check\n  method: get\n  operationId: getServiceHealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/deployments\n  method: get\n  operationId: listDeployments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/deployments/{deployment}\n  method: get\n  operationId: getDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/deployments/{deployment}\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/deployments/{deployment}\n  method: patch\n  operationId: updateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/deployments/{deployment}\n  method: delete\n  operationId: deleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/deployments/{deployment}/services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/deployments/{deployment}/services/{service}\n  method: get\n  operationId: getService\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/deployments/{deployment}/services/{service}\n  method: post\n  operationId: createService\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/deployments/{deployment}/services/{service}\n  method: patch\n  operationId: updateService\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /services/v2/deployments/{deployment}/services/{service}\n  method: delete\n  operationId: deleteService\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/extracts\n  method: get\n  operationId: listExtracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/extracts/{extract}\n  method: get\n  operationId: getExtract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/v2/extracts/{extract}\n  method: post\n  operationId:\
  \ createExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/extracts/{extract}\n  method: patch\n  operationId: updateExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/v2/extracts/{extract}\n  method: delete\n  operationId: deleteExtract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    a\n\n# --- truncated at 32 KB (81 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/agentic-access/oracle-goldengate-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/agentic-access/oracle-goldengate-agentic-access.yml
summary_line: 281 operations · 137 acting · 7 human-in-the-loop
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
---
