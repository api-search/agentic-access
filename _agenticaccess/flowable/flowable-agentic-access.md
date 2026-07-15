---
acting_count: 234
action_class_counts:
  acting: 234
  connected: 264
api_specs:
- filename: flowable-bpmn-openapi.yml
  format: yaml
  label: Flowable BPMN API
  slug: flowable-bpmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-bpmn-openapi.yml
- filename: flowable-cmmn-openapi.yml
  format: yaml
  label: Flowable CMMN API
  slug: flowable-cmmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-cmmn-openapi.yml
- filename: flowable-dmn-openapi.yml
  format: yaml
  label: Flowable DMN API
  slug: flowable-dmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-dmn-openapi.yml
- filename: flowable-form-openapi.yml
  format: yaml
  label: Flowable Form API
  slug: flowable-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-form-openapi.yml
- filename: flowable-content-openapi.yml
  format: yaml
  label: Flowable Content API
  slug: flowable-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-content-openapi.yml
- filename: flowable-idm-openapi.yml
  format: yaml
  label: Flowable IDM API
  slug: flowable-idm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-idm-openapi.yml
- filename: flowable-external-worker-openapi.yml
  format: yaml
  label: Flowable External Worker API
  slug: flowable-external-worker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-external-worker-openapi.yml
consequence_counts:
  physical: 14
  read: 264
  safety-critical: 4
  write: 216
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Flowable Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /access-tokens/{tokenId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /acquire/jobs/{jobId}/cmmnTerminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cmmn-runtime/case-instances/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /cmmn-runtime/case-instances/{caseInstanceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cmmn-repository/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /cmmn-repository/deployments/{deploymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /dmn-repository/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /dmn-repository/deployments/{deploymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document-repository/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /document-repository/deployments/{deploymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /form-repository/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /form-repository/deployments/{deploymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /groups/{groupId}/members
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /groups/{groupId}/members/{userId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /identity/groups/{groupId}/members
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /identity/groups/{groupId}/members/{userId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /repository/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /repository/deployments/{deploymentId}
operation_count: 498
overview: 'Flowable exposes 498 API operations that an AI agent could call, of which 234 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 264 read, 216 write, 14 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flowable
provider_slug: flowable
slug: flowable-agentic-access
source_filename: flowable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/flowable-bpmn-openapi.yml, openapi/flowable-cmmn-openapi.yml, openapi/flowable-content-openapi.yml,\n  openapi/flowable-dmn-openapi.yml, openapi/flowable-external-worker-openapi.yml, openapi/flowable-form-openapi.yml,\n  openapi/flowable-idm-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 498\n  by_action_class:\n    connected: 264\n    acting: 234\n  by_consequence:\n    read: 264\n    write: 216\n    physical: 14\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /form/form-data\n  method: get\n  operationId: getFormData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /form/form-data\n  method: post\n  operationId: submitForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history/historic-activity-instances\n  method: get\n  operationId: listHistoricActivityInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-detail\n  method: get\n  operationId: listHistoricDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-detail/{detailId}/data\n  method: get\n  operationId: getHistoricDetailVariableData\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-process-instances\n  method: get\n  operationId: listHistoricProcessInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-process-instances/delete\n  method: post\n  operationId: bulkDeleteHistoricProcessInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history/historic-process-instances/{processInstanceId}\n  method: get\n  operationId: getHistoricProcessInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /history/historic-process-instances/{processInstanceId}\n  method: delete\n  operationId: deleteHistoricProcessInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history/historic-process-instances/{processInstanceId}/comments\n  method: get\n  operationId: listHistoricProcessInstanceComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-process-instances/{processInstanceId}/comments\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history/historic-process-instances/{processInstanceId}/comments/{commentId}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-process-instances/{processInstanceId}/comments/{commentId}\n  method: delete\n  operationId: deleteComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history/historic-process-instances/{processInstanceId}/identitylinks\n  method: get\n  operationId: listHistoricProcessInstanceIdentityLinks\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-process-instances/{processInstanceId}/variables/{variableName}/data\n  method: get\n  operationId: getHistoricProcessInstanceVariableData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-task-instances\n  method: get\n  operationId: listHistoricTaskInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-task-instances/{taskId}\n  method: get\n  operationId: getTaskInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-task-instances/{taskId}\n  method: delete\n  operationId: deleteTaskInstance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history/historic-task-instances/{taskId}/form\n  method: get\n  operationId: getHistoricTaskForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-task-instances/{taskId}/identitylinks\n  method: get\n  operationId: listHistoricTaskInstanceIdentityLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-task-instances/{taskId}/variables/{variableName}/data\n  method: get\n  operationId: getHistoricTaskInstanceVariableData\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-task-log-entries\n  method: get\n  operationId: getHistoricTaskLogEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-variable-instances\n  method: get\n  operationId: listHistoricVariableInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/historic-variable-instances/{varInstanceId}/data\n  method: get\n  operationId: getHistoricInstanceVariableData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/groups/{groupId}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/groups/{groupId}\n  method: put\n  operationId: updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /identity/groups/{groupId}\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/groups/{groupId}/members\n  method: post\n  operationId: createMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/groups/{groupId}/members/{userId}\n  method: delete\n  operationId: deleteMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /identity/users/{userId}\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/users/{userId}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/users/{userId}/info\n  method: get\n  operationId: listUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/users/{userId}/info\n  method: post\n  operationId:\
  \ createUserInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/users/{userId}/info/{key}\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/users/{userId}/info/{key}\n  method: put\n  operationId: updateUserInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/users/{userId}/info/{key}\n  method: delete\n  operationId: deleteUserInfo\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity/users/{userId}/picture\n  method: get\n  operationId: getUserPicture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/users/{userId}/picture\n  method: put\n  operationId: updateUserPicture\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/batch-parts/{batchPartId}\n  method: get\n  operationId: getBatchPart\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/batch-parts/{batchPartId}/batch-part-document\n  method: get\n  operationId: getBatchPartDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/batches\n  method: get\n  operationId: listBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/batches/{batchId}\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/batches/{batchId}\n  method: delete\n  operationId: deleteBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/batches/{batchId}/batch-document\n  method: get\n  operationId: getBatchDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/batches/{batchId}/batch-parts\n  method: get\n  operationId: listBatchesPart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/deadletter-jobs\n  method: get\n  operationId: listDeadLetterJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/deadletter-jobs\n  method: post\n  operationId: executeDeadLetterJobAction\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/deadletter-jobs/{jobId}\n  method: get\n  operationId: getDeadletterJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/deadletter-jobs/{jobId}\n  method: post\n  operationId: executeDeadLetterJobAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/deadletter-jobs/{jobId}\n  method: delete\n  operationId: deleteDeadLetterJob\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/deadletter-jobs/{jobId}/exception-stacktrace\n  method: get\n  operationId: getDeadLetterJobStacktrace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/engine\n  method: get\n  operationId: getEngineInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/engine-properties\n  method: get\n  operationId: getEngineProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/engine-properties\n\
  \  method: post\n  operationId: createEngineProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/engine-properties/{engineProperty}\n  method: put\n  operationId: updateEngineProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/engine-properties/{engineProperty}\n  method: delete\n  operationId: deleteEngineProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/history-jobs\n  method: get\n  operationId: listDeadLetterJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/history-jobs/{jobId}\n  method: get\n  operationId: getHistoryJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/history-jobs/{jobId}\n  method: post\n  operationId: executeHistoryJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/history-jobs/{jobId}\n  method: delete\n  operationId: deleteHistoryJob\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/jobs/{jobId}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/jobs/{jobId}\n  method: post\n  operationId: executeJobAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /management/jobs/{jobId}\n  method: delete\n  operationId: deleteJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/jobs/{jobId}/exception-stacktrace\n  method: get\n  operationId: getJobStacktrace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/properties\n  method: get\n  operationId: getProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/suspended-jobs\n  method: get\n  operationId: listSuspendedJobs\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/suspended-jobs/{jobId}\n  method: get\n  operationId: getSuspendedJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/suspended-jobs/{jobId}\n  method: delete\n  operationId: deleteSuspendedJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/suspended-jobs/{jobId}/exception-stacktrace\n  method: get\n  operationId: getSuspendedJobStacktrace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/tables\n\
  \  method: get\n  operationId: listTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/tables/{tableName}\n  method: get\n  operationId: getTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/tables/{tableName}/columns\n  method: get\n  operationId: getTableMetaData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/tables/{tableName}/data\n  method: get\n  operationId: getTableData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/timer-jobs\n  method: get\n  operationId: listTimerJobs\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/timer-jobs/{jobId}\n  method: get\n  operationId: getTimerJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/timer-jobs/{jobId}\n  method: post\n  operationId: executeTimerJobAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/timer-jobs/{jobId}\n  method: delete\n  operationId: deleteTimerJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/timer-jobs/{jobId}/exception-stacktrace\n  method: get\n  operationId: getTimerJobStacktrace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query/activity-instances\n  method: post\n  operationId: queryActivityInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/executions\n  method: post\n  operationId: queryExecutions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /query/historic-activity-instances\n  method: post\n  operationId: queryActivityInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/historic-detail\n  method: post\n  operationId: queryHistoricDetail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/historic-process-instances\n  method: post\n  operationId: queryHistoricProcessInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/historic-task-instances\n  method: post\n  operationId: queryHistoricTaskInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/historic-variable-instances\n  method: post\n  operationId: queryVariableInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/process-instances\n  method: post\n  operationId: queryProcessInstances\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/tasks\n  method: post\n  operationId: queryTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query/variable-instances\n  method: post\n  operationId: queryVariableInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repository/deployments\n\
  \  method: get\n  operationId: listDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repository/deployments\n  method: post\n  operationId: uploadDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repository/deployments/{deploymentId}\n  method: get\n  operationId: getDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repository/deployments/{deploymentId}\n  method: delete\n  operationId: deleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repository/deployments/{deploymentId}/resourcedata/{resourceName}\n  method: get\n  operationId: getDeploymentResourceData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repository/deployments/{deploymentId}/resources\n  method: get\n  operationId: listDeploymentResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repository/deployments/{deploymentId}/resources/**\n  method: get\n  operationId: getDeploymentResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repository/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repository/models\n  method: post\n  operationId: createModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repository/models/{modelId}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repository/models/{modelId}\n  method: put\n  operationId: updateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repository/models/{modelId}\n  method: delete\n  operationId: deleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repository/models/{modelId}/source\n  method: get\n  operationId: getModelBytes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repository/models/{modelId}/source\n  method: put\n  operationId: setModelSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repository/models/{modelId}/source-extra\n  method: get\n  operationId: getExtraEditorSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repository/models/{modelId}/source-extra\n  method: put\n  operationId: setExtraEditorSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repository/process-definitions\n  method: get\n  operationId: listProcessDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n\n# --- truncated at 32 KB (147 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/agentic-access/flowable-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/agentic-access/flowable-agentic-access.yml
summary_line: 498 operations · 234 acting · 4 human-in-the-loop
tags:
- BPM
- Business Process Management
- Workflow
- BPMN
- CMMN
- DMN
- Process Automation
- Case Management
- Open Source
- REST API
---
