---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 19
api_specs:
- filename: langgraph-openapi.json
  format: json
  label: LangSmith Deployment Control Plane API
  slug: control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/openapi/langgraph-openapi.json
consequence_counts:
  physical: 5
  read: 19
  safety-critical: 1
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Langgraph Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/auth/tokens/workspace/slack
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/deployments/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/deployments/{deployment_id}/revisions/{revision_id}/redeploy
operation_count: 39
overview: 'LangGraph exposes 39 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 14 write, 5 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LangGraph
provider_slug: langgraph
slug: langgraph-agentic-access
source_filename: langgraph-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/langgraph-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 19\n    acting: 20\n  by_consequence:\n    read: 19\n    physical: 5\n    write: 14\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/integrations/github/install\n  method: get\n  operationId: list_github_integrations_v1_integrations_github_install_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/github/{integration_id}/repos\n  method: get\n  operationId: list_github_repositories_v1_integrations_github__integration_id__repos_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/forge/github/install\n  method: get\n  operationId: list_forge_github_integrations_v1_integrations_forge_github_install_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/forge/github/{integration_id}/repos\n  method: get\n  operationId: list_forge_github_repositories_v1_integrations_forge_github__integration_id__repos_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments\n  method: get\n  operationId: list_deployments_v2_deployments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/deployments\n  method: post\n  operationId: create_deployment_v2_deployments_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/deployments\n  method: delete\n  operationId: delete_deployments_v2_deployments_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/deployments/{deployment_id}\n  method: get\n  operationId: get_deployment_v2_deployments__deployment_id__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{deployment_id}\n  method: patch\n  operationId: patch_deployment_v2_deployments__deployment_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/deployments/{deployment_id}\n  method: delete\n  operationId: delete_deployment_v2_deployments__deployment_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/deployments/{deployment_id}/revisions\n  method: get\n  operationId: list_revisions_v2_deployments__deployment_id__revisions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{deployment_id}/revisions/{revision_id}\n  method: get\n  operationId: get_revision_v2_deployments__deployment_id__revisions__revision_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deployments/{deployment_id}/revisions/{revision_id}/redeploy\n  method: post\n  operationId: redeploy_revision_v2_deployments__deployment_id__revisions__revision_id__redeploy_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/listeners\n  method: get\n  operationId: list_listeners_v2_listeners_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/listeners\n  method: post\n  operationId: create_listener_v2_listeners_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/listeners/{listener_id}\n  method: get\n  operationId: get_listener_v2_listeners__listener_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/listeners/{listener_id}\n  method: patch\n  operationId: patch_listener_v2_listeners__listener_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/listeners/{listener_id}\n  method: delete\n  operationId: delete_listener_v2_listeners__listener_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/providers\n  method: get\n  operationId: list_oauth_providers_v2_auth_providers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/providers\n  method: post\n  operationId: create_oauth_provider_v2_auth_providers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/setup/{provider_id}\n  method: get\n  operationId: oauth_setup_callback_v2_auth_setup__provider_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/callback/{provider_id}\n  method: get\n  operationId: oauth_callback_get_v2_auth_callback__provider_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/callback/{provider_id}\n\
  \  method: post\n  operationId: oauth_callback_v2_auth_callback__provider_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/authenticate\n  method: post\n  operationId: authenticate_v2_auth_authenticate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/wait/{auth_id}\n  method: get\n  operationId: wait_for_auth_completion_v2_auth_wait__auth_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/auth/providers/mcp-discover\n  method: post\n  operationId: create_mcp_oauth_provider_v2_auth_providers_mcp_discover_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/providers/{provider_id}\n  method: get\n  operationId: get_oauth_provider_v2_auth_providers__provider_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/providers/{provider_id}\n  method: patch\n  operationId: update_oauth_provider_v2_auth_providers__provider_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/providers/{provider_id}\n  method: delete\n  operationId: delete_oauth_provider_v2_auth_providers__provider_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/tokens\n  method: get\n  operationId: list_oauth_tokens_for_user_v2_auth_tokens_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/tokens\n  method: delete\n  operationId: delete_oauth_tokens_for_user_v2_auth_tokens_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/tokens/{token_id}/metadata\n  method: patch\n  operationId: update_token_label_v2_auth_tokens__token_id__metadata_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/tokens/{token_id}\n  method: delete\n  operationId: delete_single_oauth_token_v2_auth_tokens__token_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/tokens/exists\n  method:\
  \ get\n  operationId: check_oauth_token_exists_v2_auth_tokens_exists_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/tokens/workspace/slack/exists\n  method: get\n  operationId: check_workspace_slack_tokens_exist_v2_auth_tokens_workspace_slack_exists_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/tokens/workspace/slack\n  method: delete\n  operationId: revoke_all_slack_tokens_for_workspace_v2_auth_tokens_workspace_slack_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/auth/agents/{agent_id}/connections\n\
  \  method: get\n  operationId: list_connections_v2_auth_agents__agent_id__connections_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth/agents/{agent_id}/connections\n  method: post\n  operationId: create_connection_v2_auth_agents__agent_id__connections_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/auth/agents/{agent_id}/connections/{connection_id}\n  method: delete\n  operationId: remove_connection_v2_auth_agents__agent_id__connections__connection_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langgraph/refs/heads/main/agentic-access/langgraph-agentic-access.yml
summary_line: 39 operations · 20 acting · 1 human-in-the-loop
tags:
- Agents
- Artificial Intelligence
- Large Language Models
- Workflows
- Orchestration
---
