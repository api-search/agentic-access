---
acting_count: 54
action_class_counts:
  acting: 54
  connected: 2
api_specs:
- filename: ainote-dev-dev-docs-api-openapi.yml
  format: yaml
  label: ainote Dev Docs API
  slug: ainote-dev-dev-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-dev-docs-api-openapi.yml
- filename: ainote-dev-handoffs-api-openapi.yml
  format: yaml
  label: ainote Handoffs API
  slug: ainote-dev-handoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-handoffs-api-openapi.yml
- filename: ainote-dev-misc-api-openapi.yml
  format: yaml
  label: ainote Misc API
  slug: ainote-dev-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-misc-api-openapi.yml
- filename: ainote-dev-onboarding-api-openapi.yml
  format: yaml
  label: ainote Onboarding API
  slug: ainote-dev-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-onboarding-api-openapi.yml
- filename: ainote-dev-sync-api-openapi.yml
  format: yaml
  label: ainote Sync API
  slug: ainote-dev-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-sync-api-openapi.yml
- filename: ainote-dev-tasks-api-openapi.yml
  format: yaml
  label: ainote Tasks API
  slug: ainote-dev-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-tasks-api-openapi.yml
- filename: ainote-dev-vaults-api-openapi.yml
  format: yaml
  label: ainote Vaults API
  slug: ainote-dev-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ainote-dev/openapi/ainote-dev-vaults-api-openapi.yml
consequence_counts:
  physical: 3
  read: 2
  safety-critical: 5
  write: 46
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Ainote Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/env_sync.drift_status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/env_sync_txn_rollback
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/graph_add_entity
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/sync_changes
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/mcp/tools/sync_delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/env_sync_txn_pull
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/judgment_list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp/tools/sync_pending_conflicts
operation_count: 56
overview: 'ainote exposes 56 API operations that an AI agent could call, of which 54 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 46 write, 3 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ainote
provider_slug: ainote-dev
slug: ainote-dev-agentic-access
source_filename: ainote-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/ainote-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    acting: 54\n    connected: 2\n  by_consequence:\n    write: 46\n    physical: 3\n    read: 2\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /api/mcp/tools/list_tasks\n  method: post\n  operationId: tool_list_tasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/create_task\n  method: post\n  operationId:\
  \ tool_create_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_task\n  method: post\n  operationId: tool_update_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/delete_task\n  method: post\n  operationId: tool_delete_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/mcp/tools/list_categories\n  method: post\n  operationId: tool_list_categories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/list_papers\n  method: post\n  operationId: tool_list_papers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/project_read\n  method: post\n  operationId: tool_project_read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/project_write\n  method: post\n  operationId: tool_project_write\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/assumption_write\n  method: post\n  operationId: tool_assumption_write\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/judgment_submit\n  method: post\n  operationId: tool_judgment_submit\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/judgment_list\n  method: post\n  operationId: tool_judgment_list\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/list_dev_docs\n  method: post\n  operationId: tool_list_dev_docs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/mcp/tools/get_dev_doc\n  method: post\n  operationId: tool_get_dev_doc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/create_dev_doc\n  method: post\n  operationId: tool_create_dev_doc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/update_dev_doc\n  method: post\n  operationId: tool_update_dev_doc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/pull_dev_docs\n  method: post\n  operationId: tool_pull_dev_docs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/delete_dev_doc\n  method: post\n  operationId: tool_delete_dev_doc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/list_dev_categories\n  method: post\n  operationId: tool_list_dev_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/get_setup_guide\n  method: post\n  operationId: tool_get_setup_guide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/vault_list\n  method: post\n  operationId: tool_vault_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/vault_create\n  method: post\n  operationId: tool_vault_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/vault_clone\n  method: post\n  operationId: tool_vault_clone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/vault_connect_status\n  method: post\n  operationId: tool_vault_connect_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/vault_sync\n  method: post\n  operationId: tool_vault_sync\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/sync_push\n  method: post\n  operationId: tool_sync_push\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/sync_push_batch\n  method: post\n  operationId: tool_sync_push_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/sync_pull\n\
  \  method: post\n  operationId: tool_sync_pull\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/sync_list\n  method: post\n  operationId: tool_sync_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/sync_changes\n  method: post\n  operationId: tool_sync_changes\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/mcp/tools/sync_delete\n  method: post\n  operationId: tool_sync_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/mcp/tools/sync_merge\n  method: post\n  operationId: tool_sync_merge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/sync_diff\n  method: post\n  operationId: tool_sync_diff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/sync_pending_conflicts\n  method: post\n  operationId: tool_sync_pending_conflicts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/sync_audit_layer5\n  method: post\n  operationId: tool_sync_audit_layer5\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/mcp/tools/handoff_save\n  method: post\n  operationId: tool_handoff_save\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/handoff_list\n  method: post\n  operationId: tool_handoff_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/handoff_get\n  method: post\n  operationId: tool_handoff_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/memory_search\n  method: post\n  operationId: tool_memory_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/memory_get\n  method: post\n  operationId: tool_memory_get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/graph_get_node\n  method: post\n  operationId: tool_graph_get_node\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/graph_list_nodes\n  method: post\n  operationId: tool_graph_list_nodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/graph_add_entity\n  method: post\n  operationId: tool_graph_add_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/mcp/tools/graph_update_entity\n\
  \  method: post\n  operationId: tool_graph_update_entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/graph_soft_delete\n  method: post\n  operationId: tool_graph_soft_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/env_sync.device_enroll\n  method: post\n  operationId: tool_env_sync.device_enroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/env_sync.device_list\n  method: post\n  operationId: tool_env_sync.device_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp/tools/env_sync.device_request_secret_share\n  method: post\n  operationId: tool_env_sync.device_request_secret_share\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/env_sync.secret_push\n  method: post\n  operationId: tool_env_sync.secret_push\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/env_sync.secret_pull\n  method: post\n  operationId: tool_env_sync.secret_pull\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/env_sync.secret_rotate\n  method: post\n  operationId: tool_env_sync.secret_rotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/env_sync_txn_push\n  method: post\n  operationId: tool_env_sync_txn_push\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/env_sync_txn_pull\n  method: post\n  operationId: tool_env_sync_txn_pull\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/env_sync_txn_rollback\n  method: post\n  operationId: tool_env_sync_txn_rollback\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/mcp/tools/env_sync.heartbeat_ping\n  method: post\n  operationId: tool_env_sync.heartbeat_ping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/tools/env_sync.drift_status\n  method: post\n  operationId: tool_env_sync.drift_status\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/mcp/tools/env_sync.sync_status\n  method: post\n  operationId: tool_env_sync.sync_status\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ainote-dev/agentic-access/ainote-dev-agentic-access.yml
summary_line: 56 operations · 54 acting · 5 human-in-the-loop
tags:
- Artificial Intelligence
- Productivity
- Note Taking
- Task Management
- Mobile
---
