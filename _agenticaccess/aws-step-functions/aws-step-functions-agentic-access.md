---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 7
api_specs:
- filename: aws-step-functions-state-machines-api-openapi.yml
  format: yaml
  label: AWS Step Functions State Machines API
  slug: aws-step-functions-state-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/openapi/aws-step-functions-state-machines-api-openapi.yml
- filename: aws-step-functions-aws-step-functions-api-openapi.yml
  format: yaml
  label: AWS Step Functions AWS Step Functions API
  slug: aws-step-functions-aws-step-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/openapi/aws-step-functions-aws-step-functions-api-openapi.yml
- filename: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-createstat-api-openapi.yml
  format: yaml
  label: 'AWS Step Functions AWS Step Functions #X Amz Target=AWSStepFunctions.CreateStat… API'
  slug: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-createstat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/openapi/aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-createstat-api-openapi.yml
- filename: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-deletestat-api-openapi.yml
  format: yaml
  label: 'AWS Step Functions AWS Step Functions #X Amz Target=AWSStepFunctions.DeleteStat… API'
  slug: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-deletestat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/openapi/aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-deletestat-api-openapi.yml
- filename: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-describest-api-openapi.yml
  format: yaml
  label: 'AWS Step Functions AWS Step Functions #X Amz Target=AWSStepFunctions.DescribeSt… API'
  slug: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-describest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/openapi/aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-describest-api-openapi.yml
- filename: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-liststatem-api-openapi.yml
  format: yaml
  label: 'AWS Step Functions AWS Step Functions #X Amz Target=AWSStepFunctions.ListStateM… API'
  slug: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-liststatem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/openapi/aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-liststatem-api-openapi.yml
- filename: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-publishsta-api-openapi.yml
  format: yaml
  label: 'AWS Step Functions AWS Step Functions #X Amz Target=AWSStepFunctions.PublishSta… API'
  slug: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-publishsta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/openapi/aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-publishsta-api-openapi.yml
- filename: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-updatestat-api-openapi.yml
  format: yaml
  label: 'AWS Step Functions AWS Step Functions #X Amz Target=AWSStepFunctions.UpdateStat… API'
  slug: aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-updatestat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/openapi/aws-step-functions-aws-step-functions-x-amz-target-awsstepfunctions-updatestat-api-openapi.yml
consequence_counts:
  physical: 3
  read: 7
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Aws Step Functions Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=AWSStepFunctions.StopExecution
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSStepFunctions.SendTaskFailure
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSStepFunctions.SendTaskHeartbeat
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSStepFunctions.SendTaskSuccess
operation_count: 27
overview: 'AWS Step Functions exposes 27 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 16 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AWS Step Functions
provider_slug: aws-step-functions
slug: aws-step-functions-agentic-access
source_filename: aws-step-functions-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/aws-step-functions-state-machines-api-openapi.yml, openapi/aws-step-functions-x-amz-target-awsstepfunctions-createactivity-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-createstatemachine-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-deleteactivity-api-openapi.yml, openapi/aws-step-functions-x-amz-target-awsstepfunctions-deletestatemachine-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-describeactivity-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-describeexecution-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-describemaprun-api-openapi.yml, openapi/aws-step-functions-x-amz-target-awsstepfunctions-describestatemachine-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-describestatemachineforexecution-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-getactivitytask-api-openapi.yml,\n\
  \  openapi/aws-step-functions-x-amz-target-awsstepfunctions-getexecutionhistory-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-listactivities-api-openapi.yml, openapi/aws-step-functions-x-amz-target-awsstepfunctions-listexecutions-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-listmapruns-api-openapi.yml, openapi/aws-step-functions-x-amz-target-awsstepfunctions-liststatemachines-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-listtagsforresource-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-sendtaskfailure-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-sendtaskheartbeat-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-sendtasksuccess-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-startexecution-api-openapi.yml, openapi/aws-step-functions-x-amz-target-awsstepfunctions-startsyncexecution-api-openapi.yml,\n\
  \  openapi/aws-step-functions-x-amz-target-awsstepfunctions-stopexecution-api-openapi.yml, openapi/aws-step-functions-x-amz-target-awsstepfunctions-tagresource-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-untagresource-api-openapi.yml, openapi/aws-step-functions-x-amz-target-awsstepfunctions-updatemaprun-api-openapi.yml,\n  openapi/aws-step-functions-x-amz-target-awsstepfunctions-updatestatemachine-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 20\n    connected: 7\n  by_consequence:\n    write: 16\n    read: 7\n    physical: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /\n  method: post\n  operationId: createStateMachine\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.CreateActivity\n  method: post\n  operationId: CreateActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.CreateStateMachine\n  method: post\n  operationId: CreateStateMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.DeleteActivity\n  method: post\n  operationId: DeleteActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.DeleteStateMachine\n  method: post\n  operationId: DeleteStateMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.DescribeActivity\n  method: post\n  operationId: DescribeActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.DescribeExecution\n  method: post\n  operationId: DescribeExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.DescribeMapRun\n  method: post\n  operationId: DescribeMapRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.DescribeStateMachine\n\
  \  method: post\n  operationId: DescribeStateMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.DescribeStateMachineForExecution\n  method: post\n  operationId: DescribeStateMachineForExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.GetActivityTask\n  method: post\n  operationId: GetActivityTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /#X-Amz-Target=AWSStepFunctions.GetExecutionHistory\n  method: post\n  operationId: GetExecutionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=AWSStepFunctions.ListActivities\n  method: post\n  operationId: ListActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=AWSStepFunctions.ListExecutions\n  method: post\n  operationId: ListExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=AWSStepFunctions.ListMapRuns\n  method: post\n  operationId: ListMapRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /#X-Amz-Target=AWSStepFunctions.ListStateMachines\n  method: post\n  operationId: ListStateMachines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=AWSStepFunctions.ListTagsForResource\n  method: post\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=AWSStepFunctions.SendTaskFailure\n  method: post\n  operationId: SendTaskFailure\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.SendTaskHeartbeat\n\
  \  method: post\n  operationId: SendTaskHeartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.SendTaskSuccess\n  method: post\n  operationId: SendTaskSuccess\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.StartExecution\n  method: post\n  operationId: StartExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.StartSyncExecution\n  method: post\n  operationId: StartSyncExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.StopExecution\n  method: post\n  operationId: StopExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n-\
  \ path: /#X-Amz-Target=AWSStepFunctions.TagResource\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.UntagResource\n  method: post\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.UpdateMapRun\n  method: post\n  operationId: UpdateMapRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSStepFunctions.UpdateStateMachine\n  method: post\n  operationId: UpdateStateMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/agentic-access/aws-step-functions-agentic-access.yml
summary_line: 27 operations · 20 acting · 1 human-in-the-loop
tags:
- iPaaS
- Orchestration
- Serverless
---
