---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 21
api_specs:
- filename: amazon-codedeploy-applications-api-openapi.yml
  format: yaml
  label: Amazon CodeDeploy Applications API
  slug: amazon-codedeploy-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/openapi/amazon-codedeploy-applications-api-openapi.yml
- filename: amazon-codedeploy-deployments-api-openapi.yml
  format: yaml
  label: Amazon CodeDeploy Deployments API
  slug: amazon-codedeploy-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/openapi/amazon-codedeploy-deployments-api-openapi.yml
- filename: amazon-codedeploy-aws-codedeploy-api-openapi.yml
  format: yaml
  label: Amazon CodeDeploy AWS CodeDeploy API
  slug: amazon-codedeploy-aws-codedeploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/openapi/amazon-codedeploy-aws-codedeploy-api-openapi.yml
consequence_counts:
  physical: 32
  read: 21
  safety-critical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Codedeploy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.StopDeployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.AddTagsToOnPremisesInstances
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetApplicationRevisions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetApplications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetDeploymentGroups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetDeploymentInstances
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetDeploymentTargets
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetDeployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetOnPremisesInstances
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.ContinueDeployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.CreateApplication
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.CreateDeployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.CreateDeploymentConfig
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.CreateDeploymentGroup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.DeleteApplication
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.DeleteDeploymentConfig
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.DeleteDeploymentGroup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.DeleteGitHubAccountToken
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.DeleteResourcesByExternalId
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.DeregisterOnPremisesInstance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.ListGitHubAccountTokenNames
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.PutLifecycleEventHookExecutionStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.RegisterApplicationRevision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.RegisterOnPremisesInstance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=CodeDeploy_20141006.RemoveTagsFromOnPremisesInstances
operation_count: 54
overview: 'Amazon CodeDeploy exposes 54 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 32 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
slug: amazon-codedeploy-agentic-access
source_filename: amazon-codedeploy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-codedeploy-applications-api-openapi.yml, openapi/amazon-codedeploy-deployments-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-addtagstoonpremisesinstances-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-batchgetapplicationrevisions-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-batchgetapplications-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-batchgetdeploymentgroups-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-batchgetdeploymentinstances-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-batchgetdeployments-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-batchgetdeploymenttargets-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-batchgetonpremisesinstances-api-openapi.yml,\n\
  \  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-continuedeployment-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-createapplication-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-createdeployment-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-createdeploymentconfig-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-createdeploymentgroup-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-deleteapplication-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-deletedeploymentconfig-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-deletedeploymentgroup-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-deletegithubaccounttoken-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-deleteresourcesbyexternalid-api-openapi.yml,\n\
  \  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-deregisteronpremisesinstance-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-getapplication-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-getapplicationrevision-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-getdeployment-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-getdeploymentconfig-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-getdeploymentgroup-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-getdeploymentinstance-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-getdeploymenttarget-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-getonpremisesinstance-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listapplicationrevisions-api-openapi.yml,\n\
  \  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listapplications-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listdeploymentconfigs-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listdeploymentgroups-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listdeploymentinstances-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listdeployments-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listdeploymenttargets-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listgithubaccounttokennames-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listonpremisesinstances-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-listtagsforresource-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-putlifecycleeventhookexecutionstatus-api-openapi.yml,\n\
  \  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-registerapplicationrevision-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-registeronpremisesinstance-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-removetagsfromonpremisesinstances-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-skipwaittimeforinstancetermination-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-stopdeployment-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-tagresource-api-openapi.yml, openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-untagresource-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-updateapplication-api-openapi.yml,\n  openapi/amazon-codedeploy-x-amz-target-codedeploy-20141006-updatedeploymentgroup-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically\
  \ from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    acting: 33\n    connected: 21\n  by_consequence:\n    physical: 32\n    read: 21\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /applications\n  method: post\n  operationId: CreateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications\n  method: get\n  operationId: ListApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /applications/{applicationName}\n  method: get\n  operationId: GetApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationName}\n  method: delete\n  operationId: DeleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments\n  method: post\n  operationId: CreateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /deployments\n  method: get\n  operationId: ListDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/{deploymentId}\n  method: get\n  operationId: GetDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.AddTagsToOnPremisesInstances\n  method: post\n  operationId: AddTagsToOnPremisesInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetApplicationRevisions\n\
  \  method: post\n  operationId: BatchGetApplicationRevisions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetApplications\n  method: post\n  operationId: BatchGetApplications\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetDeploymentGroups\n  method: post\n  operationId: BatchGetDeploymentGroups\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetDeploymentInstances\n  method: post\n  operationId: BatchGetDeploymentInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetDeployments\n  method: post\n  operationId: BatchGetDeployments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetDeploymentTargets\n  method: post\n  operationId: BatchGetDeploymentTargets\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.BatchGetOnPremisesInstances\n  method: post\n  operationId: BatchGetOnPremisesInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.ContinueDeployment\n  method: post\n  operationId: ContinueDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.CreateApplication\n  method: post\n  operationId: CreateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.CreateDeployment\n  method: post\n  operationId: CreateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.CreateDeploymentConfig\n  method: post\n  operationId: CreateDeploymentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.CreateDeploymentGroup\n  method: post\n\
  \  operationId: CreateDeploymentGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.DeleteApplication\n  method: post\n  operationId: DeleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.DeleteDeploymentConfig\n  method: post\n  operationId: DeleteDeploymentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.DeleteDeploymentGroup\n  method: post\n  operationId: DeleteDeploymentGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.DeleteGitHubAccountToken\n  method: post\n  operationId: DeleteGitHubAccountToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n  \
  \    exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.DeleteResourcesByExternalId\n  method: post\n  operationId: DeleteResourcesByExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.DeregisterOnPremisesInstance\n  method: post\n  operationId: DeregisterOnPremisesInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.GetApplication\n  method: post\n  operationId: GetApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.GetApplicationRevision\n  method: post\n  operationId: GetApplicationRevision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.GetDeployment\n  method: post\n  operationId: GetDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.GetDeploymentConfig\n  method: post\n  operationId: GetDeploymentConfig\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.GetDeploymentGroup\n  method: post\n  operationId: GetDeploymentGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.GetDeploymentInstance\n  method: post\n  operationId: GetDeploymentInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.GetDeploymentTarget\n  method: post\n  operationId: GetDeploymentTarget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.GetOnPremisesInstance\n\
  \  method: post\n  operationId: GetOnPremisesInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.ListApplicationRevisions\n  method: post\n  operationId: ListApplicationRevisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.ListApplications\n  method: post\n  operationId: ListApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.ListDeploymentConfigs\n  method: post\n  operationId: ListDeploymentConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /#X-Amz-Target=CodeDeploy_20141006.ListDeploymentGroups\n  method: post\n  operationId: ListDeploymentGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.ListDeploymentInstances\n  method: post\n  operationId: ListDeploymentInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.ListDeployments\n  method: post\n  operationId: ListDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.ListDeploymentTargets\n  method: post\n  operationId: ListDeploymentTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.ListGitHubAccountTokenNames\n  method: post\n  operationId: ListGitHubAccountTokenNames\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.ListOnPremisesInstances\n  method: post\n  operationId: ListOnPremisesInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.ListTagsForResource\n  method: post\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=CodeDeploy_20141006.PutLifecycleEventHookExecutionStatus\n  method: post\n  operationId: PutLifecycleEventHookExecutionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.RegisterApplicationRevision\n  method: post\n  operationId: RegisterApplicationRevision\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /#X-Amz-Target=CodeDeploy_20141006.RegisterOnPremisesInstance\n  method: post\n  operationId: RegisterOnPremisesInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.RemoveTagsFromOnPremisesInstances\n  method: post\n  operationId: RemoveTagsFromOnPremisesInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.SkipWaitTimeForInstanceTermination\n\
  \  method: post\n  operationId: SkipWaitTimeForInstanceTermination\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.StopDeployment\n  method: post\n  operationId: StopDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.TagResource\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.UntagResource\n  method: post\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.UpdateApplication\n  method: post\n  operationId: UpdateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=CodeDeploy_20141006.UpdateDeploymentGroup\n  method: post\n  operationId: UpdateDeploymentGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/agentic-access/amazon-codedeploy-agentic-access.yml
summary_line: 54 operations · 33 acting · 1 human-in-the-loop
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
- Developer Tools
---
