---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 22
api_specs:
- filename: beam-ai-agent-context-files-api-openapi.yml
  format: yaml
  label: Beam AI Agent Context Files API
  slug: beam-ai-agent-context-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-context-files-api-openapi.yml
- filename: beam-ai-agent-graph-api-openapi.yml
  format: yaml
  label: Beam AI Agent Graph API
  slug: beam-ai-agent-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-graph-api-openapi.yml
- filename: beam-ai-agent-setup-api-openapi.yml
  format: yaml
  label: Beam AI Agent Setup API
  slug: beam-ai-agent-setup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-setup-api-openapi.yml
- filename: beam-ai-agent-skills-api-openapi.yml
  format: yaml
  label: Beam AI Agent Skills API
  slug: beam-ai-agent-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-skills-api-openapi.yml
- filename: beam-ai-agent-task-api-openapi.yml
  format: yaml
  label: Beam AI Agent Task API
  slug: beam-ai-agent-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-task-api-openapi.yml
- filename: beam-ai-agent-views-api-openapi.yml
  format: yaml
  label: Beam AI Agent Views API
  slug: beam-ai-agent-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agent-views-api-openapi.yml
- filename: beam-ai-agents-api-openapi.yml
  format: yaml
  label: Beam AI Agents API
  slug: beam-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-agents-api-openapi.yml
- filename: beam-ai-complete-agent-graph-api-openapi.yml
  format: yaml
  label: Beam AI Complete Agent Graph API
  slug: beam-ai-complete-agent-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-complete-agent-graph-api-openapi.yml
- filename: beam-ai-custom-tool-api-openapi.yml
  format: yaml
  label: Beam AI Custom Tool API
  slug: beam-ai-custom-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-custom-tool-api-openapi.yml
- filename: beam-ai-tool-api-openapi.yml
  format: yaml
  label: Beam AI Tool API
  slug: beam-ai-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-tool-api-openapi.yml
- filename: beam-ai-user-api-openapi.yml
  format: yaml
  label: Beam AI User API
  slug: beam-ai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/openapi/beam-ai-user-api-openapi.yml
consequence_counts:
  read: 22
  safety-critical: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 26
kind: agentic-access
layout: agentic-access
method: generated
name: Beam Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-graphs/add-edge
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-graphs/add-node
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-graphs/complete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-graphs/test-node
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /agent-graphs/update-edge/{edgeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /agent-graphs/update-node
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /agent-graphs/{agentId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /agent-graphs/{agentId}/nodes/{nodeId}/input-output-params
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /agent-graphs/{agentId}/nodes/{nodeId}/prompt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /agent-graphs/{graphId}/publish
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-setup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-setup/agent-context/feedback
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-setup/upload
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-setup/{agentId}/context-file
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-setup/{agentId}/{setupStep}/feedback
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-tasks
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /agent-tasks/execution/{taskId}/output-rating
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-tasks/execution/{taskId}/rejection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-tasks/execution/{taskId}/user-consent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /agent-tasks/execution/{taskId}/user-input
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-tasks/retry
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /agent/{agentId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent/{agentId}/skills/import
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /context/agent/{agentId}/file
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /context/agent/{agentId}/file/{fileKey}
operation_count: 48
overview: 'Beam AI exposes 48 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 26 safety-critical.


  26 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Beam AI
provider_slug: beam-ai
slug: beam-ai-agentic-access
source_filename: beam-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/beam-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 22\n    acting: 26\n  by_consequence:\n    read: 22\n    safety-critical: 26\n  human_in_the_loop_required: 26\noperations:\n- path: /v2/user/me\n  method: get\n  operationId: UserController_findCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent\n  method: get\n  operationId: AgentController_findMany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /context/agent/{agentId}/file\n\
  \  method: post\n  operationId: AgentContextFilesController_uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /context/agent/{agentId}/file/{fileId}/download\n  method: get\n  operationId: AgentContextFilesController_getFileDownloadLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-setup/session/{agentId}\n  method: get\n  operationId: AgentSetupController_session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tool/active-tools\n  method: get\n  operationId: ToolController_getActiveTools\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tool/optimize/{toolFunctionName}\n  method: post\n  operationId: ToolController_optimizeTool\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tool/optimization-status/thread/{threadId}\n  method: post\n  operationId: ToolController_getToolOptimizationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-tool/preferred-models\n  method: get\n  operationId: CustomToolController_fetchPreferredModels\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-views\n  method: get\n  operationId: AgentViewController_listViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-views/{viewId}\n  method: get\n  operationId: AgentViewController_getView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-views/{viewId}/records\n  method: get\n  operationId: AgentViewController_listRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-views/{viewId}/columns/{columnId}/links/{recordId}\n  method: get\n  operationId: AgentViewController_listLinkedRecords\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-setup\n  method: post\n  operationId: BeamAgentController_processInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-setup/agent-context/feedback\n  method: post\n  operationId: BeamAgentController_addIntroductionFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-setup/{agentId}/{setupStep}/feedback\n  method: post\n  operationId:\
  \ BeamAgentController_addStepFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-setup/upload\n  method: post\n  operationId: BeamAgentController_uploadFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-setup/{agentId}/context-file\n  method: post\n  operationId: BeamAgentController_uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-tasks/{taskId}/updates\n  method: get\n  operationId: AgentTaskController_getSseUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-tasks\n  method: post\n  operationId: AgentTaskController_createTaskSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-tasks\n  method: get\n  operationId: AgentTaskController_allTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-tasks/analytics\n  method: get\n  operationId: AgentTaskController_agentAnalyticsDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-tasks/execution/{taskId}/user-input\n  method: patch\n  operationId: AgentTaskController_submitUserInput\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-tasks/execution/{taskId}/rejection\n  method: post\n  operationId: AgentTaskController_submitUserRejection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-tasks/execution/{taskId}/user-consent\n  method: post\n  operationId: AgentTaskController_submitUserConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-tasks/latest-executions\n  method: get\n  operationId: AgentTaskController_getLatestExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-tasks/iterate\n  method: get\n  operationId: AgentTaskController_getNextTask\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-tasks/execution/{taskId}/output-rating\n  method: patch\n  operationId: AgentTaskController_submitOutputRating\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-tasks/tool-output-schema/{graphNodeId}\n  method: get\n  operationId: AgentTaskController_getToolOutputParamsByGraphNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-tasks/retry\n  method: post\n  operationId: AgentTaskController_retryTaskExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-tasks/{taskId}\n  method: get\n  operationId: AgentTaskController_taskDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-graphs/add-node\n  method: post\n  operationId: AgentGraphController_addNode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-graphs/add-edge\n  method: post\n  operationId: AgentGraphController_addEdge\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-graphs/update-edge/{edgeId}\n  method: put\n  operationId: AgentGraphController_updateEdge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-graphs/test-node\n  method: post\n  operationId: AgentGraphController_testTool\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-graphs/update-node\n  method: patch\n  operationId: AgentGraphController_updateNode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-graphs/{agentId}/nodes/lite\n  method: get\n  operationId: AgentGraphController_getAgentGraphLite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-graphs/{agentId}/nodes/{nodeId}\n  method: get\n  operationId: AgentGraphController_getNodeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /agent-graphs/{agentId}/nodes/{nodeId}/input-output-params\n  method: patch\n  operationId: AgentGraphController_updateNodeParams\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-graphs/{agentId}/nodes/{nodeId}/prompt\n  method: patch\n  operationId: AgentGraphController_updateNodePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-graphs/{agentId}\n  method: get\n  operationId: AgentGraphController_getAgentGraph\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-graphs/{agentId}\n  method: put\n  operationId: CompleteAgentGraphController_updateAgentGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-graphs/agent-task-nodes/{toolFunctionName}\n  method: get\n  operationId: AgentGraphController_getTaskNodesByToolFunctionName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-graphs/{graphId}/publish\n  method: patch\n  operationId: AgentGraphController_publishGraph\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent-graphs/complete\n  method: post\n  operationId: CompleteAgentGraphController_createAgentGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent/{agentId}/skills/import\n  method: post\n  operationId: AgentSkillController_importSkill\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /context/agent/{agentId}/file/{fileKey}\n  method: delete\n  operationId: AgentContextFilesController_deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agent/{agentId}\n  method: put\n  operationId: AgentController_updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beam-ai/refs/heads/main/agentic-access/beam-ai-agentic-access.yml
summary_line: 48 operations · 26 acting · 26 human-in-the-loop
tags:
- Company
- AI
- Automation
- Enterprise
- Platform
---
