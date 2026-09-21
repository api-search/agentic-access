---
acting_count: 0
action_class_counts:
  connected: 16
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts for the b612 agent surfaces. Every MCP tool declares execution.taskSupport "forbidden" and returns reference text; the server states it has no input for source code. Every operation is therefore classified connected/read. The single elevation is b612_notes, which reads a per-licence store of personal memos and so needs a bound subject and an audit trail. A governance starting point, not a provider claim — review and bind audience per deployment.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: derived
name: Hakuto 0209 Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'HaneruTo exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HaneruTo
provider_slug: hakuto-0209-com
slug: hakuto-0209-com-agentic-access
source_filename: hakuto-0209-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: >-\n  mcp/hakuto-0209-com-mcp-tools.json (the live tools/list, 10 tools with inputSchema and\n  execution.taskSupport), the MCP initialize instructions, the A2A agent card (6 skills) and the data policy\n  at https://mcp.hakuto-0209.com/terms. There is no OpenAPI, so 0-working/derive-agentic-access.py could not\n  be run; the classification below applies the same heuristics (Curity Access Intelligence vocabulary,\n  research/curity/agentic-governance/) to the MCP tools and A2A skills by hand from what each declares and\n  what the provider states about side effects.\ndescription: >-\n  Recommended x-agentic-access execution contracts for the b612 agent surfaces. Every MCP tool declares\n  execution.taskSupport \"forbidden\" and returns reference text; the server states it has no input for\n  source code. Every operation is therefore classified connected/read. The single elevation is b612_notes,\n  which reads a per-licence store\
  \ of personal memos and so needs a bound subject and an audit trail. A\n  governance starting point, not a provider claim — review and bind audience per deployment.\nprovider_guidance:\n  source: MCP initialize instructions (https://mcp.hakuto-0209.com/mcp)\n  summary: >-\n    The provider's own instructions to a connecting agent: consult b612_patterns with the project's keywords\n    before starting; pull b612_domain_preset and b612_review_checklist (sending only short strings such as\n    an industry name); apply the returned checkpoints to the local code yourself; re-check with the\n    checklist and the three self-questions before declaring done; apply b612_rules locally for mechanical\n    checks. \"There is no input on this server for code bodies — customer code never reaches the provider.\"\nsummary:\n  operations: 16\n  mcp_tools: 10\n  a2a_skills: 6\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\n  subject_required: 1\n\
  operations:\n- surface: mcp\n  tool: b612_principles\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n  note: Keyless tier (20 req/min per IP).\n- surface: mcp\n  tool: b612_review_checklist\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: mcp\n  tool: b612_patterns\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: mcp\n  tool: b612_domain_preset\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: mcp\n  tool: b612_rules\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n  note: Keyless tier (20 req/min per IP).\n- surface:\
  \ mcp\n  tool: b612_design\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: mcp\n  tool: b612_reference\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: mcp\n  tool: b612_grow\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: mcp\n  tool: b612_notes\n  x-agentic-access: {action-class: connected, consequence: read, subject: required, audience: null, token: {max-ttl: 3600}, audit: required}\n  note: Reads the licence holder's own LINE memos (personal data, 90-day retention per the data policy). Bind the licence to a subject and audit reads.\n- surface: mcp\n  tool: b612_update\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl:\
  \ 3600}, audit: none}\n  note: Returns an update PROCEDURE the client executes locally; the local execution (file writes under .claude/) is the agent's own act, outside this server's surface, and the provider's uninstall page documents exactly which files it touches.\n- surface: a2a\n  skill: principles\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: a2a\n  skill: review-checklist\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: a2a\n  skill: patterns\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: a2a\n  skill: domain-preset\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n- surface: a2a\n  skill:\
  \ scan-code\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n  note: The only operation that transmits source text to the provider. Read-class because the provider states it is analysed in memory and discarded (no persistence, no LLM); a deployment that treats source as confidential should still gate WHICH files an agent may send.\n- surface: a2a\n  skill: rules\n  x-agentic-access: {action-class: connected, consequence: read, subject: optional, audience: null, token: {max-ttl: 3600}, audit: none}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hakuto-0209-com/refs/heads/main/agentic-access/hakuto-0209-com-agentic-access.yml
summary_line: 16 operations
tags:
- Agents
- MCP
- A2A
- Code Review
- Static Analysis
- Developer Tools
- Compliance
- Web Development
- Japan
- agent-native
---
