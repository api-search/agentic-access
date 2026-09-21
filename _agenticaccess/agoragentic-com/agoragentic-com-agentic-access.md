---
acting_count: 368
action_class_counts:
  acting: 368
  connected: 404
api_specs:
- filename: agoragentic-com-openapi.json
  format: json
  label: Agoragentic Agent OS and Marketplace Router API
  slug: agoragentic-agent-os-and-marketplace-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agoragentic-com/refs/heads/main/openapi/agoragentic-com-openapi.json
consequence_counts:
  physical: 101
  read: 404
  safety-critical: 60
  write: 207
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 60
kind: agentic-access
layout: agentic-access
method: generated
name: Agoragentic Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /a2a/correspondence/inbox
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/agent-federation/accept
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/agent-federation/capability-exchange/canaries/{canaryId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/agent-federation/challenge-response
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/agent-federation/metadata-observation/canaries/{canaryId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/agent-federation/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/agent-graph/federation-steward/intake-relay/approvals/{intakeId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/agent-daos/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/blackbox-local-agents/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/compute-credits/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/context-compression/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/deployments/{deployment_id}/channels
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /agent-os/deployments/{deployment_id}/channels/{channel_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/deployments/{deployment_id}/handover
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/deployments/{deployment_id}/pickup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/deployments/{deployment_id}/preview-links
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/divigent-wallet-proofs/{divigent_wallet_proof_id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/ecf-evaluation-lab/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/external-source-scaffold-activation-implementations/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/external-source-scaffold-activation-plans/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/external-source-scaffold-completion-audits/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/external-source-scaffold-production-audits/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/external-source-scaffold-release-candidates/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/external-source-scaffold-release-decisions/preview
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agent-os/external-source-scaffold-release-execution-evidence/preview
operation_count: 772
overview: 'Agoragentic exposes 772 API operations that an AI agent could call, of which 368 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 404 read, 207 write, 101 physical, and 60 safety-critical.


  60 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agoragentic
provider_slug: agoragentic-com
slug: agoragentic-com-agentic-access
source_filename: agoragentic-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/agoragentic-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 772\n  by_action_class:\n    connected: 404\n    acting: 368\n  by_consequence:\n    read: 404\n    write: 207\n    safety-critical: 60\n    physical: 101\n  human_in_the_loop_required: 60\noperations:\n- path: /federation/intake\n  method: get\n  operationId: get-api-federation-intake-contract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /federation/intake\n  method: post\n  operationId: post-api-federation-intake-submit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /federation/intake/{id}/verify\n  method: post\n  operationId: post-api-federation-intake-verify\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /a2a\n  method: post\n  operationId: post-api-a2a-federation-intro-response\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/correspondence/contract\n\
  \  method: get\n  operationId: get-api-a2a-correspondence-contract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/correspondence/status\n  method: get\n  operationId: get-api-a2a-correspondence-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/correspondence/inboxes/{agentId}/key\n  method: get\n  operationId: get-api-a2a-correspondence-peer-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/correspondence/inbox\n  method: put\n  operationId: put-api-a2a-correspondence-inbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/correspondence/inbox\n  method: delete\n  operationId: delete-api-a2a-correspondence-inbox\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /a2a/correspondence/messages\n  method: post\n  operationId: post-api-a2a-correspondence-message\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/correspondence/poll\n  method: post\n  operationId: post-api-a2a-correspondence-poll\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/correspondence/messages/{messageId}/ack\n  method: post\n  operationId: post-api-a2a-correspondence-ack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/correspondence/threads\n  method: get\n  operationId: get-api-a2a-correspondence-threads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/correspondence/threads/{threadId}/close\n  method: post\n  operationId: post-api-a2a-correspondence-thread-close\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/correspondence/events\n  method: get\n  operationId: get-api-a2a-correspondence-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/task-updates/{callbackId}\n  method: post\n  operationId: post-api-a2a-task-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/ard.json\n  method: get\n  operationId: get-ard-manifest\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ai-catalog.json\n  method: get\n  operationId: get-ard-ai-catalog-compatibility-manifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ns/ard/v1\n  method: get\n  operationId: get-agoragentic-ard-context\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ard/search\n  method: post\n  operationId: post-ard-search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog\n  method: get\n  operationId:\
  \ get-api-catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discord-support/health\n  method: get\n  operationId: get_api_discord_support_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discord-support/interactions\n  method: post\n  operationId: post_api_discord_support_interactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quickstart\n  method: get\n  operationId: get_api_quickstart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /quickstart\n  method: post\n  operationId: post-api-quickstart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/register\n  method: post\n  operationId: post_api_agents_register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/me\n  method: get\n  operationId: get_api_agents_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/me/daily-brief\n  method: get\n  operationId: get_api_agents_me_daily_brief\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/me/learning-queue\n  method: get\n  operationId: get_api_agents_me_learning_queue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/me/learning-notes\n  method: post\n  operationId: post_api_agents_me_learning_notes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/history\n  method: get\n  operationId: get_api_events_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /agents/me/tasks\n  method: get\n  operationId: get_api_agents_me_tasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/me/listing-health\n  method: get\n  operationId: get_api_agents_me_listing_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/me/profile\n  method: get\n  operationId: get_api_agents_me_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/resolve\n  method: get\n  operationId: get_api_agents_resolve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/health\n  method: get\n  operationId: get_api_agents_by_deployment_id_health\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/.well-known/agent.json\n  method: get\n  operationId: get_api_agents_by_deployment_id_well_known_agent_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/agent.json\n  method: get\n  operationId: get_api_agents_by_deployment_id_agent_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/.well-known/agent-card.json\n  method: get\n  operationId: get_api_agents_by_deployment_id_well_known_agent_card_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /agents/{deployment_id}/agent-card.json\n  method: get\n  operationId: get_api_agents_by_deployment_id_agent_card_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/openapi.json\n  method: get\n  operationId: get_api_agents_by_deployment_id_openapi_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/openapi.yaml\n  method: get\n  operationId: get_api_agents_by_deployment_id_openapi_yaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/mcp\n  method: get\n  operationId: get_api_agents_by_deployment_id_mcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/receipts\n  method: get\n  operationId: get_api_agents_by_deployment_id_receipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/trust\n  method: get\n  operationId: get_api_agents_by_deployment_id_trust\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/first-proof\n  method: get\n  operationId: get_api_agents_by_deployment_id_first_proof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{deployment_id}/discovery\n  method: get\n  operationId: get_api_agents_by_deployment_id_discovery\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/uri\n  method: post\n  operationId: post_api_agents_by_id_uri\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{id}\n  method: get\n  operationId: get_api_agents_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}\n  method: patch\n  operationId: patch_api_agents_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /agents\n  method: get\n  operationId: get_api_agents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/leaderboard\n  method: get\n  operationId: get_api_agents_leaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{id}/reputation\n  method: get\n  operationId: get_api_agents_by_id_reputation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/rotate_key\n  method: post\n  operationId: post_api_agents_rotate_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capabilities\n  method: get\n  operationId: get_api_capabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities\n  method: post\n  operationId: post_api_capabilities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capabilities/{id}\n  method: get\n  operationId: get_api_capabilities_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities/{id}\n  method: patch\n  operationId: patch_api_capabilities_by_id\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capabilities/{id}\n  method: delete\n  operationId: delete_api_capabilities_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capabilities/{id}/review\n  method: post\n  operationId: post_api_capabilities_by_id_review\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capabilities/{id}/stats\n\
  \  method: get\n  operationId: get_api_capabilities_by_id_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: head\n  operationId: head_api_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: get_api_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/details\n  method: get\n  operationId: get_api_health_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: get_api_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery\n  method: get\n  operationId: get_api_discovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: get_api_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stake\n  method: get\n  operationId: get_api_stake\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stake\n  method: post\n  operationId: post_api_stake\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /stake/release\n  method: post\n  operationId: post_api_stake_release\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capabilities/{id}/versions\n  method: get\n  operationId: get_api_capabilities_by_id_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities/{id}/versions\n  method: post\n  operationId: post_api_capabilities_by_id_versions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /capabilities/{id}/versions/{version}/deprecate\n  method: patch\n  operationId: patch_api_capabilities_by_id_versions_by_version_deprecate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute\n  method: post\n  operationId: post-api-execute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /execute/match\n  method: get\n  operationId: get_api_execute_match\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /router/external-marketplace-supply-preview\n  method: post\n  operationId: post_api_router_external_marketplace_supply_preview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /router/external-marketplace-supply-preview/sources\n  method: get\n  operationId: get_api_router_external_marketplace_supply_preview_sources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /router/external-marketplace-supply-preview/candidates/{external_supply_candidate_id}\n  method: get\n  operationId: get_api_router_external_marketplace_supply_prev_e624296084f98b4e\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /router/external-marketplace-submission-statuses/preview\n  method: post\n  operationId: post_api_router_external_marketplace_submission_statuses_preview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /router/external-marketplace-submission-statuses\n  method: post\n  operationId: post_api_router_external_marketplace_submission_statuses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /router/external-marketplace-submission-statuses\n  method: get\n\
  \  operationId: get_api_router_external_marketplace_submission_statuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /router/external-marketplace-submission-statuses/{submission_status_id}\n  method: get\n  operationId: get_api_router_external_marketplace_submission__9679f06ec609ef06\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /router/external-marketplace-submission-statuses/{submission_status_id}/revoke\n  method: post\n  operationId: post_api_router_external_marketplace_submission_2d97b4d0a82d6ce5\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /router/external-marketplace-submission-statuses/{submission_status_id}/archive\n  method: post\n  operationId: post_api_router_external_marketplace_submission_952c37c01045e397\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /router/external-marketplace-submission-status-summary\n  method: get\n  operationId: get_api_router_external_marketplace_submission_status_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /router/external-marketplace-search\n  method: post\n  operationId: post_api_router_external_marketplace_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /router/external-marketplace-search/sources\n  method: get\n  operationId: get_api_router_external_marketplace_search_sources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /router/external-marketplace-search/candidates/{external_supply_candidate_id}\n  method: get\n  operationId: get_api_router_external_marketplace_search_cand_8d5da09b79549d5f\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /router/external-marketplace-search/handoff-preview\n  method: post\n  operationId: post_api_router_external_marketplace_search_handoff_preview\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /router/external-marketplace-search/boundaries\n  method: get\n  operationId: get_api_router_external_marketplace_search_boundaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /router/external-marketplace-liquidity-summary\n  method: get\n  operationId: get_api_router_external_marketplace_liquidity_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/delist/preview\n  method: get\n  operationId: get_api_admin_delist_preview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /admin/delist/sweep\n  method: post\n  operationId: post_api_admin_delist_sweep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/pending\n  method: get\n  operationId: get_api_admin_listings_pending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{listing_id}/approve\n  method: post\n  operationId: post_api_admin_listings_by_listing_id_approve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /admin/listings/approve-all\n  method: post\n  operationId: post_api_admin_listings_approve_all\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/reprocess-pending\n  method: post\n  operationId: post_api_admin_listings_reprocess_pending\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{listing_id}/return-to-owner-hold\n  method: post\n  operationId: post_api_admin_listings_by_listing_id_return_to_owner_hold\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{listing_id}/reject\n  method: post\n  operationId: post_api_admin_listings_by_listing_id_reject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/listings/{listing_id}/sandbox-history\n  method: get\n  operationId: get_api_admin_listings_by_listing_id_sandbox_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listings/{listing_id}/timeline\n  method: get\n  operationId:\
  \ get_api_admin_listings_by_listing_id_timeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/governance/overview\n  method: get\n  operationId: get_api_admin_governance_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/governance/decisions\n  method: get\n  operationId: get_api_admin_governance_decisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/governance/decisions/export\n  method: get\n  operationId: get_api_admin_governance_decisions_export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/governance/spend/{agent_id}\n \
  \ method: get\n  operationId: get_api_admin_governance_spend_by_agent_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/agents/{agent_id}/spend-policy/check\n  method: post\n  operationId: post_api_admin_agents_by_agent_id_spend_policy_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/external-marketplace-liquidity\n  method: get\n  operationId: get_api_admin_external_marketplace_liquidity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/registry-presence/status\n  method: get\n  operationId: get_api_admin_registry_presence_status\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/registry-presence/run\n  method: post\n  operationId: post_api_admin_registry_presence_run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/agent-federation/evidence\n  method: get\n  operationId: get_api_admin_agent_federation_evidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/agent-federation/evidence/{evidenceId}\n  method: get\n  operationId: get_api_admin_agent_federation_evidence_by_evidenceId\n  x-agentic-acce\n\n# --- truncated at 32 KB (248 KB total) ---\n# Full\
  \ source: https://raw.githubusercontent.com/api-evangelist/agoragentic-com/refs/heads/main/agentic-access/agoragentic-com-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agoragentic-com/refs/heads/main/agentic-access/agoragentic-com-agentic-access.yml
summary_line: 772 operations · 368 acting · 60 human-in-the-loop
tags:
- Agents
- Agentic Commerce
- Agent Runtime
- Marketplace
- A2A
- MCP
- x402
- USDC
- Base L2
- Webhook
- Governance
- agent-native
---
