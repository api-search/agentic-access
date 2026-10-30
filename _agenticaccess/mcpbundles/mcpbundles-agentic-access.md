---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: mcpbundles-local-runtime-api-openapi.yml
  format: yaml
  label: MCPBundles Local Runtime API
  slug: mcpbundles-local-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcpbundles/refs/heads/main/openapi/mcpbundles-local-runtime-api-openapi.yml
- filename: mcpbundles-tunnel-api-openapi.yml
  format: yaml
  label: MCPBundles Tunnel API
  slug: mcpbundles-tunnel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcpbundles/refs/heads/main/openapi/mcpbundles-tunnel-api-openapi.yml
- filename: mcpbundles-graph-ql-api-openapi.yml
  format: yaml
  label: MCPBundles Graph QL API
  slug: mcpbundles-graph-ql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcpbundles/refs/heads/main/openapi/mcpbundles-graph-ql-api-openapi.yml
consequence_counts:
  read: 4
  safety-critical: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Mcpbundles Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/tunnel/expose
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/tunnel/sessions/{connection_id}
operation_count: 10
overview: 'MCPBundles exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 4 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MCPBundles
provider_slug: mcpbundles
slug: mcpbundles-agentic-access
source_filename: mcpbundles-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/mcpbundles-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 4\n    acting: 6\n  by_consequence:\n    read: 4\n    write: 4\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /graphql\n  method: get\n  operationId: handle_http_get_graphql_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graphql\n  method: post\n  operationId: handle_http_post_graphql_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tunnel/expose\n  method: post\n  operationId: tunnel_expose_register_api_tunnel_expose_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tunnel/expose\n  method: delete\n  operationId: tunnel_expose_revoke_api_tunnel_expose_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tunnel/sessions\n  method: get\n  operationId: tunnel_sessions_list_api_tunnel_sessions_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tunnel/sessions/{connection_id}\n  method: delete\n  operationId: tunnel_sessions_revoke_api_tunnel_sessions__connection_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/local-runtime/heartbeat\n  method: post\n  operationId: local_runtime_heartbeat_api_local_runtime_heartbeat_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/local-runtime/install-options/{server_name}\n  method: get\n  operationId: local_runtime_install_options_api_local_runtime_install_options__server_name__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/local-runtime/install-recipes/{server_name}\n  method: get\n  operationId: local_runtime_install_recipes_api_local_runtime_install_recipes__server_name__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/local-runtime/connections/{connection_key}/tools/{tool_name}/execute\n  method: post\n  operationId: local_runtime_execute_api_local_runtime_connections__connection_key__tools__tool_name__execute_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcpbundles/refs/heads/main/agentic-access/mcpbundles-agentic-access.yml
summary_line: 10 operations · 6 acting · 2 human-in-the-loop
tags:
- Company
- Directory
- ManagedCloudPlatforms
- Tools
- Integration
---
