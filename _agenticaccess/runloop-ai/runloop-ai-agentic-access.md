---
acting_count: 154
action_class_counts:
  acting: 154
  connected: 148
api_specs:
- filename: runloop-devbox-api-openapi.yml
  format: yaml
  label: Runloop Devbox API
  slug: runloop-devbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-devbox-api-openapi.yml
- filename: runloop-blueprint-api-openapi.yml
  format: yaml
  label: Runloop Blueprint API
  slug: runloop-blueprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-blueprint-api-openapi.yml
- filename: runloop-benchmark-api-openapi.yml
  format: yaml
  label: Runloop Benchmark API
  slug: runloop-benchmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-benchmark-api-openapi.yml
- filename: runloop-scenario-api-openapi.yml
  format: yaml
  label: Runloop Scenario API
  slug: runloop-scenario-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-scenario-api-openapi.yml
- filename: runloop-agents-api-openapi.yml
  format: yaml
  label: Runloop Agents API
  slug: runloop-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-agents-api-openapi.yml
- filename: runloop-axons-api-openapi.yml
  format: yaml
  label: Runloop Axons API
  slug: runloop-axons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-axons-api-openapi.yml
- filename: runloop-objects-api-openapi.yml
  format: yaml
  label: Runloop Storage Objects API
  slug: runloop-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-objects-api-openapi.yml
- filename: runloop-secrets-api-openapi.yml
  format: yaml
  label: Runloop Secrets API
  slug: runloop-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-secrets-api-openapi.yml
- filename: runloop-network-policies-api-openapi.yml
  format: yaml
  label: Runloop Network Policies API
  slug: runloop-network-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-network-policies-api-openapi.yml
- filename: runloop-gateway-configs-api-openapi.yml
  format: yaml
  label: Runloop Gateway Configs API
  slug: runloop-gateway-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-gateway-configs-api-openapi.yml
- filename: runloop-mcp-configs-api-openapi.yml
  format: yaml
  label: Runloop MCP Configs API
  slug: runloop-mcp-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-mcp-configs-api-openapi.yml
- filename: runloop-apikeys-api-openapi.yml
  format: yaml
  label: Runloop API Keys API
  slug: runloop-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-apikeys-api-openapi.yml
- filename: runloop-executions-api-openapi.yml
  format: yaml
  label: Runloop Executions Streaming API
  slug: runloop-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/openapi/runloop-executions-api-openapi.yml
consequence_counts:
  physical: 2
  read: 148
  safety-critical: 8
  write: 144
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Runloop Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pty/{session_name}/control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pty/{session_name}/control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/devboxes/{devbox_id}/executions/{execution_id}/kill
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/devboxes/{devbox_id}/executions/{execution_id}/kill
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/devboxes/{id}/keep_alive
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/devboxes/{id}/keep_alive
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/devboxes/{id}/shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/devboxes/{id}/shutdown
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/devboxes/{devbox_id}/executions/{execution_id}/send_std_in
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/devboxes/{devbox_id}/executions/{execution_id}/send_std_in
operation_count: 302
overview: 'Runloop exposes 302 API operations that an AI agent could call, of which 154 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 148 read, 144 write, 2 physical, and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Runloop
provider_slug: runloop-ai
slug: runloop-ai-agentic-access
source_filename: runloop-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/runloop-agents-api-openapi.yml, openapi/runloop-api-openapi.yml, openapi/runloop-apikeys-api-openapi.yml,\n  openapi/runloop-axons-api-openapi.yml, openapi/runloop-benchmark-api-openapi.yml, openapi/runloop-blueprint-api-openapi.yml,\n  openapi/runloop-devbox-api-openapi.yml, openapi/runloop-executions-api-openapi.yml, openapi/runloop-gateway-configs-api-openapi.yml,\n  openapi/runloop-mcp-configs-api-openapi.yml, openapi/runloop-network-policies-api-openapi.yml,\n  openapi/runloop-objects-api-openapi.yml, openapi/runloop-scenario-api-openapi.yml, openapi/runloop-secrets-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 302\n  by_action_class:\n    acting: 154\n    connected:\
  \ 148\n  by_consequence:\n    write: 144\n    read: 148\n    safety-critical: 8\n    physical: 2\n  human_in_the_loop_required: 8\noperations:\n- path: /v1/agents\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/devbox_counts\n  method: get\n  operationId: getAgentDevboxCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/list_public\n  method: get\n  operationId: listPublicAgents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{id}/delete\n  method: post\n  operationId: deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pty/{session_name}\n  method: get\n  operationId: connectDevboxPtySession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pty/{session_name}/control\n  method: post\n  operationId:\
  \ controlDevboxPtySession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agents\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/devbox_counts\n  method: get\n  operationId: getAgentDevboxCounts\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/list_public\n  method: get\n  operationId: listPublicAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{id}/delete\n  method: post\n  operationId: deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apikeys\n  method: post\n  operationId: createAPIKey\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/axons\n  method: post\n  operationId: createAxon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/axons\n  method: get\n  operationId: listActiveAxons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/axons/{id}\n  method: get\n  operationId: getAxon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/axons/{id}/events\n  method: get\n  operationId: listAxonEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/axons/{id}/publish\n  method: post\n  operationId: publishToAxon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/axons/{id}/sql/batch\n  method: post\n  operationId: axonSqlBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/axons/{id}/sql/query\n  method: post\n\
  \  operationId: axonSqlQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/axons/{id}/subscribe/sse\n  method: get\n  operationId: subscribeToAxonSse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmark_jobs\n  method: post\n  operationId: createBenchmarkJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmark_jobs\n  method: get\n  operationId: listBenchmarkJobs\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmark_jobs/{id}\n  method: get\n  operationId: getBenchmarkJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmark_runs\n  method: get\n  operationId: listBenchmarkRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmark_runs/{id}\n  method: get\n  operationId: getBenchmarkRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmark_runs/{id}/cancel\n  method: post\n  operationId: cancelBenchmarkRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmark_runs/{id}/complete\n  method: post\n  operationId: completeBenchmarkRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmark_runs/{id}/download_logs\n  method: post\n  operationId: downloadBenchmarkRunLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmark_runs/{id}/scenario_runs\n  method: get\n  operationId: listBenchmarkRunScenarioRuns\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks\n  method: post\n  operationId: createBenchmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmarks\n  method: get\n  operationId: listBenchmarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/list_public\n  method: get\n  operationId: listPublicBenchmarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/metadata/keys\n  method: get\n\
  \  operationId: getBenchmarkMetadataKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/metadata/keys/{key}/values\n  method: get\n  operationId: getBenchmarkMetadataValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/runs\n  method: get\n  operationId: listBenchmarkRunsDeprecated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/runs/{id}\n  method: get\n  operationId: getBenchmarkRunDeprecated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/runs/{id}/cancel\n  method: post\n  operationId: cancelBenchmarkRunDeprecated\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmarks/runs/{id}/complete\n  method: post\n  operationId: completeBenchmarkRunDeprecated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmarks/runs/{id}/download_logs\n  method: post\n  operationId: downloadBenchmarkRunLogsDeprecated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmarks/runs/{id}/scenario_runs\n  method: get\n  operationId: listBenchmarkRunScenarioRunsDeprecated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/start_run\n  method: post\n  operationId: startBenchmarkRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmarks/{id}\n  method: post\n  operationId: updateBenchmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/benchmarks/{id}\n  method: get\n  operationId: getBenchmark\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/{id}/archive\n  method: post\n  operationId: archiveBenchmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmarks/{id}/definitions\n  method: get\n  operationId: getBenchmarkScenarioDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/{id}/runs\n  method: get\n  operationId: getBenchmarkRuns\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmarks/{id}/scenarios\n  method: post\n  operationId: updateBenchmarkScenarios\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benchmarks/{id}/unarchive\n  method: post\n  operationId: unarchiveBenchmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/blueprints\n  method: post\n  operationId: createBlueprint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/blueprints\n  method: get\n  operationId: listImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/create_from_inspection\n  method: post\n  operationId: createBlueprintFromInspection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/blueprints/list_public\n  method: get\n  operationId: listPublicBlueprints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/blueprints/metadata/keys\n  method: get\n  operationId: getBlueprintMetadataKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/metadata/keys/{key}/values\n  method: get\n  operationId: getBlueprintMetadataValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/preview\n  method: post\n  operationId: previewImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/blueprints/public/metadata/keys\n  method: get\n  operationId: getPublicBlueprintMetadataKeys\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/public/metadata/keys/{key}/values\n  method: get\n  operationId: getPublicBlueprintMetadataValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/{id}\n  method: get\n  operationId: getBlueprint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blueprints/{id}/delete\n  method: post\n  operationId: deleteBlueprint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/blueprints/{id}/logs\n  method:\
  \ get\n  operationId: blueprintLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes\n  method: post\n  operationId: createDevbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes\n  method: get\n  operationId: listDevboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/disk_snapshots\n  method: get\n  operationId: getDevboxDiskSnapshotList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/disk_snapshots/list_public\n\
  \  method: get\n  operationId: listPublicSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/disk_snapshots/metadata/keys\n  method: get\n  operationId: getSnapshotMetadataKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/disk_snapshots/metadata/keys/{key}/values\n  method: get\n  operationId: getSnapshotMetadataValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/disk_snapshots/public/metadata/keys\n  method: get\n  operationId: getPublicSnapshotMetadataKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/disk_snapshots/public/metadata/keys/{key}/values\n\
  \  method: get\n  operationId: getPublicSnapshotMetadataValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/disk_snapshots/{id}\n  method: post\n  operationId: updateDiskSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/disk_snapshots/{id}/delete\n  method: post\n  operationId: deleteSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/disk_snapshots/{id}/status\n\
  \  method: get\n  operationId: queryDiskSnapshotAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/metadata/keys\n  method: get\n  operationId: getDevboxMetadataKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/metadata/keys/{key}/values\n  method: get\n  operationId: getDevboxMetadataValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/{devbox_id}/executions/{execution_id}\n  method: get\n  operationId: queryAsyncCommand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/{devbox_id}/executions/{execution_id}/kill\n\
  \  method: post\n  operationId: killAsyncExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/devboxes/{devbox_id}/executions/{execution_id}/send_std_in\n  method: post\n  operationId: sendStdIn\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{devbox_id}/executions/{execution_id}/stream_stderr_updates\n  method: get\n  operationId: streamStdErrUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/{devbox_id}/executions/{execution_id}/stream_stdout_updates\n  method: get\n  operationId: streamStdOutUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/{devbox_id}/executions/{execution_id}/wait_for_status\n  method: post\n  operationId: waitForCommandCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}\n  method: post\n  operationId: updateDevbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}\n  method: get\n  operationId: getDevbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/{id}/create_pty_tunnel\n  method: post\n  operationId: createDevboxPtyTunnel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/create_ssh_key\n  method: post\n  operationId: createDevboxSshKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/download_file\n  method: post\n  operationId: devboxDownloadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/enable_tunnel\n  method: post\n  operationId: enableDevboxTunnel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/execute\n  method: post\n  operationId: executeCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/execute_async\n  method: post\n  operationId: execAsyncCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/execute_sync\n  method: post\n  operationId: execSyncCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/keep_alive\n  method: post\n  operationId: keepAliveDevbox\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/devboxes/{id}/logs\n  method: get\n  operationId: listDevboxLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/{id}/logs/tail\n  method: get\n  operationId: tailDevboxLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/{id}/read_file_contents\n  method: post\n  operationId: devboxReadFileContents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/remove_tunnel\n  method: post\n  operationId: removeDevboxTunnel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/resume\n  method: post\n  operationId: resumeDevbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/shutdown\n  method: post\n  operationId: shutdownDevbox\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/devboxes/{id}/snapshot_disk\n  method: post\n  operationId: createDiskSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/snapshot_disk_async\n  method: post\n  operationId: createDiskSnapshotAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/suspend\n\
  \  method: post\n  operationId: suspendDevbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/upload_file\n  method: post\n  operationId: devboxUploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/usage\n  method: get\n  operationId: getDevboxResourceUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/devboxes/{id}/wait_for_status\n  method: post\n  operationId: waitForDevboxStatus\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/devboxes/{id}/write_file_contents\n  method: post\n  operationId: devboxWriteFileContents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gateway-configs\n  method: post\n  operationId: createGatewayConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/gateway-configs\n  method: get\n  operationId: listGatewayConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gateway-configs/{id}\n  method: get\n  operationId: getGatewayConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gateway-configs/{id}\n  method: post\n  operationId: updateGatewayConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gateway-configs/{id}/delete\n  method: post\n  operationId: deleteGatewayConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ req\n\n# --- truncated at 32 KB (86 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/agentic-access/runloop-ai-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runloop-ai/refs/heads/main/agentic-access/runloop-ai-agentic-access.yml
summary_line: 302 operations · 154 acting · 8 human-in-the-loop
tags:
- AI
- AI Agents
- Coding Agents
- Sandboxes
- Devboxes
- Code Execution
- Evaluation
- Benchmarks
- SWE-Bench
- MCP
- Snapshots
- microVM
- Enterprise
- SOC 2
---
