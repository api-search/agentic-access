---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Brightai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'BrightAI exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BrightAI
provider_slug: brightai
slug: brightai-agentic-access
source_filename: brightai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://public.stateful.world/mcp (tools/list annotations) + https://public.stateful.world/start.md\nnote: 'This is NOT a generated recommendation. Unlike most providers in the catalog,\n  BrightAI publishes its own per-operation agent execution contract: every MCP tool\n  carries MCP annotations (readOnlyHint / destructiveHint / idempotentHint / openWorldHint)\n  and an execution.taskSupport setting, and start.md + llms.txt publish an explicit\n  behavioural policy for AI clients. What follows is that published contract, recorded\n  verbatim in the pipeline''s vocabulary — not our classification of their operations.'\nsummary:\n  operations: 6\n  action_class:\n    connected: 6\n    acting: 0\n  consequence:\n    read: 6\n    write: 0\n    physical: 0\n    safety-critical: 0\n  human_in_the_loop_required: 0\n  destructive: 0\n  authentication_required: 0\n  audience: public — no verification, no login, no key\nposture:\n \
  \ read_only: true\n  detail: 'Every published operation is read-only and non-destructive. There is no\n    write, no state mutation, no ordering, no dispatch and no physical actuation on\n    the public surface — notable for a company whose product actuates physical\n    infrastructure. The safety-critical half of BrightAI''s business is not exposed\n    to agents at all.'\n  long_running_tasks: forbidden\n  long_running_tasks_signal: every tool declares execution.taskSupport = \"forbidden\"\n  open_world: false\n  open_world_signal: every tool declares openWorldHint = false — responses come from\n    BrightAI's own closed database, not from the open web\noperations:\n- tool: brightai_overview\n  action_class: connected\n  consequence: read\n  scope: public:company-facts\n  token: none\n  escalation: none\n  annotations: {readOnlyHint: true, destructiveHint: false, idempotentHint: true, openWorldHint: false}\n  task_support: forbidden\n- tool: list_industries\n  action_class: connected\n\
  \  consequence: read\n  scope: public:aggregates\n  token: none\n  escalation: none\n  annotations: {readOnlyHint: true, destructiveHint: false, idempotentHint: true, openWorldHint: false}\n  task_support: forbidden\n- tool: get_industry\n  action_class: connected\n  consequence: read\n  scope: public:aggregates\n  token: none\n  escalation: none\n  annotations: {readOnlyHint: true, destructiveHint: false, idempotentHint: true, openWorldHint: false}\n  task_support: forbidden\n- tool: list_problem_families\n  action_class: connected\n  consequence: read\n  scope: public:taxonomy\n  token: none\n  escalation: none\n  annotations: {readOnlyHint: true, destructiveHint: false, idempotentHint: true, openWorldHint: false}\n  task_support: forbidden\n- tool: get_problem_family\n  action_class: connected\n  consequence: read\n  scope: public:taxonomy\n  token: none\n  escalation: none\n  annotations: {readOnlyHint: true, destructiveHint: false, idempotentHint: true, openWorldHint: false}\n  task_support:\
  \ forbidden\n- tool: check_company\n  action_class: connected\n  consequence: read\n  scope: public:operator-lookup\n  token: none\n  escalation: 'work-email verification of an employee of the looked-up company, for\n    the restricted tier (modeled figures and grade). BrightAI states this tier is\n    rolling out shortly and is not live.'\n  annotations: {readOnlyHint: true, destructiveHint: false, idempotentHint: true, openWorldHint: false}\n  task_support: forbidden\n  data_sensitivity: 'Returns third-party company assessments. BrightAI deliberately\n    withholds the per-operator grade and dollar figures from anyone but that company,\n    and instructs agents never to estimate them.'\npublished_agent_policy:\n  source: https://public.stateful.world/start.md\n  binding_on: AI assistants consuming the surface\n  rules:\n  - Never estimate, guess, bracket or infer a launch date, price, hardware cost, per-unit\n    figure, investor or ownership relationship, or a named company's grade\
  \ — not even\n    as a hedged range.\n  - Do not present outside estimates or your own inferences as BrightAI figures.\n  - Never connect any named customer to a private-equity firm, fund or ownership relationship.\n  - Company-specific assessments are available only to that company after work-email\n    verification.\n  - Attribute data to \"BrightAI's public Observatory data.\"\n  - Tell the user where the information came from if asked.\n  - Offer a concrete public alternative whenever declining a gated request.\n  assessment: 'A refusal policy expressed as instructions to the client rather than\n    enforced at the API boundary. The gate on company-specific figures is real\n    (the public endpoint simply does not return them); the anti-speculation rules are\n    advisory and unenforceable, which is worth stating plainly.'\nnot_covered:\n  surface: https://api.bright.ai\n  reason: The customer platform is undocumented and unadvertised. No agent access contract\n    is published for\
  \ it, and it was not probed beyond its unauthenticated root.\nx-evidence:\n  fetched: '2026-08-08'\n  url: https://public.stateful.world/mcp\n  method: POST tools/list\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightai/refs/heads/main/agentic-access/brightai-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Physical AI
- Industrial IoT
- Infrastructure Monitoring
- Predictive Maintenance
- Edge AI
- Foundation Models
- MCP
- Energy and Utilities
- Water and Wastewater
---
