---
acting_count: 81
action_class_counts:
  acting: 81
  connected: 66
api_specs:
- filename: engine.oas3.json
  format: json
  label: Seldon Inference API
  slug: seldon-inference-api
  spec_type: OpenAPI
  url: https://github.com/SeldonIO/seldon-core/blob/master/openapi/engine.oas3.json
- filename: seldon-enterprise-platform-api-openapi.yml
  format: yaml
  label: Seldon Enterprise Platform REST API
  slug: seldon-enterprise-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seldon/refs/heads/main/openapi/seldon-enterprise-platform-api-openapi.yml
consequence_counts:
  physical: 24
  read: 66
  safety-critical: 1
  write: 56
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Seldon Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /iam/users/{username}/resetPassword
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /inference-logs/namespace/{namespace}/seldondeployments/{deploymentName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /namespaces/{namespace}/seldondeployments/{name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /namespaces/{namespace}/seldondeployments/{name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/batchjobs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/explain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/gitrestore
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/gitrevert
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/loadtestjobs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /namespaces/{namespace}/seldondeployments/{name}/loadtestjobs/{jobName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/monitor/drift-detector
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /namespaces/{namespace}/seldondeployments/{name}/monitor/drift-detector/{detectorName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/monitor/featuredistributions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/monitor/featurestatistics
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/monitor/metrics-server
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /namespaces/{namespace}/seldondeployments/{name}/monitor/metrics-server/{detectorName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/monitor/outlier-detector
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /namespaces/{namespace}/seldondeployments/{name}/monitor/outlier-detector/{detectorName}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/predict
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /namespaces/{namespace}/seldondeployments/{name}/predictcurl
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /namespaces/{namespace}/seldondeployments/{name}/predictfile
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /seldon/{namespace}/{deployment}/api/v1.0/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /seldon/{namespace}/{deployment}/api/v1.0/predictions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send-feedback
operation_count: 147
overview: 'Seldon exposes 147 API operations that an AI agent could call, of which 81 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 66 read, 56 write, 24 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Seldon
provider_slug: seldon
slug: seldon-agentic-access
source_filename: seldon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/seldon-enterprise-platform-api-openapi.yml, openapi/seldon-inference-api-openapi.yml,\n  openapi/seldon-inference-api-v2-openapi.yml, openapi/seldon-wrapper-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 147\n  by_action_class:\n    acting: 81\n    connected: 66\n  by_consequence:\n    write: 56\n    read: 66\n    physical: 24\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /applicationlogs\n  method: post\n  operationId: ReadApplicationLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /cluster\n  method: get\n  operationId: ReadCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /healthcheck\n  method: get\n  operationId: ReadHealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/experiments/{name}/gitdiff\n  method: get\n  operationId: ReadExperimentGitDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/experiments/{name}/gitlogs\n  method: get\n  operationId: ReadExperimentGitLogs\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/gitdiffs\n  method: get\n  operationId: ReadGitDiffs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/gitops-status\n  method: get\n  operationId: ReadGitOpsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/models\n  method: post\n  operationId: CreateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/models/{name}\n  method: delete\n  operationId: DeleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/models/{name}\n  method: get\n  operationId: ReadModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/models/{name}\n  method: put\n  operationId: UpdateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/models/{name}/gitdiff\n  method: get\n  operationId: ReadModelGitDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/models/{name}/gitlogs\n  method: get\n  operationId: ReadModelGitLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines\n  method: get\n  operationId: ListPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines\n  method: post\n  operationId: CreatePipeline\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}\n  method: delete\n  operationId: DeletePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}\n  method: get\n  operationId: ReadPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}\n  method:\
  \ put\n  operationId: UpdatePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/batchjobs\n  method: get\n  operationId: ListPipelineBatchJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/batchjobs\n  method: post\n  operationId: CreatePipelineBatchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/batchjobs/{jobName}\n  method: get\n  operationId: GetPipelineBatchJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment\n  method: delete\n  operationId: DeletePipelineExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment\n  method: get\n  operationId: GetPipelineExperiment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment\n  method: post\n  operationId: CreatePipelineExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment\n  method: put\n  operationId: UpdatePipelineExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment/canary\n  method: delete\n  operationId: RemoveCanary\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment/canary\n  method: post\n  operationId: CreateCanaryExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment/canary\n  method: put\n  operationId: PromoteCanary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment/shadow\n  method: delete\n  operationId: RemoveShadow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment/shadow\n  method: post\n  operationId: CreateShadowExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/experiment/shadow\n\
  \  method: put\n  operationId: PromoteShadow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/explain\n  method: post\n  operationId: ExplainSeldonPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/explainer\n  method: delete\n  operationId: DeletePipelineExplainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/explainer\n  method: get\n  operationId: ReadPipelineExplainer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/explainer\n  method: post\n  operationId: CreatePipelineExplainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/explainer\n  method: put\n  operationId: UpdatePipelineExplainer\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/gitdiff\n  method: get\n  operationId: ReadPipelineGitDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/gitlogs\n  method: get\n  operationId: ReadPipelineGitLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/loadtestjobs\n  method: get\n  operationId: ListLoadtestPipeline\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/loadtestjobs\n  method: post\n  operationId: CreateLoadtestPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/loadtestjobs/{jobName}\n  method: delete\n  operationId: DeleteLoadtestPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/models\n\
  \  method: get\n  operationId: ListPipelineModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/drift-detector\n  method: get\n  operationId: ListDriftDetectorSeldonPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/drift-detector\n  method: post\n  operationId: CreateDriftDetectorSeldonPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/drift-detector/{detectorName}\n\
  \  method: delete\n  operationId: DeleteDriftDetectorSeldonPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/drift-detector/{detectorName}\n  method: get\n  operationId: ReadDriftDetectorSeldonPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/featuredistributions\n  method: post\n  operationId: SeldonPipelineFeatureDistributions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/featurestatistics\n  method: post\n  operationId: SeldonPipelineFeatureStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/outlier-detector\n  method: get\n  operationId: ListOutlierDetectorSeldonPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/outlier-detector\n  method: post\n  operationId: CreateOutlierDetectorSeldonPipeline\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/outlier-detector/{detectorName}\n  method: delete\n  operationId: DeleteOutlierDetectorSeldonPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/monitor/outlier-detector/{detectorName}\n  method: get\n  operationId: ReadOutlierDetectorSeldonPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/predictcurl\n  method: put\n  operationId: ReadPredictCurlSeldonPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/pipelines/{name}/predictfile\n  method: post\n  operationId: PredictFileSeldonPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments\n  method: get\n  operationId:\
  \ ListSeldonDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments\n  method: post\n  operationId: CreateSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}\n  method: delete\n  operationId: DeleteSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}\n  method: get\n  operationId: ReadSeldonDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}\n  method: put\n  operationId: UpdateSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/batchjobs\n  method: get\n  operationId: ListSeldonDeploymentBatchJobs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/batchjobs\n  method: post\n  operationId: CreateSeldonDeploymentBatchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/batchjobs/{jobName}\n  method: get\n  operationId: GetDeploymentBatchJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/explain\n\
  \  method: post\n  operationId: ExplainSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/gitdiff\n  method: get\n  operationId: ReadSeldonDeploymentGitDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/gitlogs\n  method: get\n  operationId: ReadSeldonDeploymentGitLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n\
  - path: /namespaces/{namespace}/seldondeployments/{name}/gitrestore\n  method: post\n  operationId: SeldonDeploymentGitRestore\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/gitrevert\n  method: post\n  operationId: SeldonDeploymentGitRevert\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/loadtestjobs\n\
  \  method: get\n  operationId: ListLoadtestSeldonDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/loadtestjobs\n  method: post\n  operationId: CreateLoadtestSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/loadtestjobs/{jobName}\n  method: delete\n  operationId: DeleteLoadtestSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/drift-detector\n  method: get\n  operationId: ListDriftDetectorSeldonDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/drift-detector\n  method: post\n  operationId: CreateDriftDetectorSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/drift-detector/{detectorName}\n  method: delete\n  operationId: DeleteDriftDetectorSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/drift-detector/{detectorName}\n  method: get\n  operationId: ReadDriftDetectorSeldonDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/featuredistributions\n  method: post\n\
  \  operationId: SeldonDeploymentFeatureDistributions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/featurestatistics\n  method: post\n  operationId: SeldonDeploymentFeatureStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/metrics-server\n  method:\
  \ get\n  operationId: ListMetricsServerSeldonDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/metrics-server\n  method: post\n  operationId: CreateMetricsServerSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/metrics-server/{detectorName}\n  method: delete\n  operationId: DeleteMetricsServerSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/metrics-server/{detectorName}\n  method: get\n  operationId: ReadMetricsServerSeldonDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/outlier-detector\n  method: get\n  operationId: ListOutlierDetectorSeldonDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/outlier-detector\n  method: post\n  operationId:\
  \ CreateOutlierDetectorSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/outlier-detector/{detectorName}\n  method: delete\n  operationId: DeleteOutlierDetectorSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/monitor/outlier-detector/{detectorName}\n\
  \  method: get\n  operationId: ReadOutlierDetectorSeldonDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/predict\n  method: post\n  operationId: PredictSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/predictcurl\n  method: put\n  operationId: ReadPredictCurlSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n \
  \     exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/predictfile\n  method: post\n  operationId: PredictFileSeldonDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - '[]'\n- path: /namespaces/{namespace}/seldondeployments/{name}/resources\n  method: get\n  operationId: ListSeldonDeploymentResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\n\n# --- truncated at 32 KB (50 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/seldon/refs/heads/main/agentic-access/seldon-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seldon/refs/heads/main/agentic-access/seldon-agentic-access.yml
summary_line: 147 operations · 81 acting · 1 human-in-the-loop
tags:
- MLOps
- Machine Learning
- Model Serving
- Inference
- Kubernetes
- AI Operations
- Drift Detection
- Explainability
- Canary Deployment
- A/B Testing
- LLMOps
---
