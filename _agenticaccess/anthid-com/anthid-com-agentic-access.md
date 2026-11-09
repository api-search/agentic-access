---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 10
api_specs:
- filename: anthid-com-account-manual-controls-api-openapi.yml
  format: yaml
  label: anthid-com Account Manual Controls API
  slug: anthid-com-account-manual-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-account-manual-controls-api-openapi.yml
- filename: anthid-com-account-risk-controls-api-openapi.yml
  format: yaml
  label: anthid-com Account Risk Controls API
  slug: anthid-com-account-risk-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-account-risk-controls-api-openapi.yml
- filename: anthid-com-account-time-controls-api-openapi.yml
  format: yaml
  label: anthid-com Account Time Controls API
  slug: anthid-com-account-time-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-account-time-controls-api-openapi.yml
- filename: anthid-com-control-evaluation-api-openapi.yml
  format: yaml
  label: anthid-com Control Evaluation API
  slug: anthid-com-control-evaluation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-control-evaluation-api-openapi.yml
- filename: anthid-com-effective-controls-api-openapi.yml
  format: yaml
  label: anthid-com Effective Controls API
  slug: anthid-com-effective-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-effective-controls-api-openapi.yml
- filename: anthid-com-organization-controls-api-openapi.yml
  format: yaml
  label: anthid-com Organization Controls API
  slug: anthid-com-organization-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-organization-controls-api-openapi.yml
- filename: anthid-com-symbol-manual-controls-api-openapi.yml
  format: yaml
  label: anthid-com Symbol Manual Controls API
  slug: anthid-com-symbol-manual-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-symbol-manual-controls-api-openapi.yml
- filename: anthid-com-symbol-risk-controls-api-openapi.yml
  format: yaml
  label: anthid-com Symbol Risk Controls API
  slug: anthid-com-symbol-risk-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-symbol-risk-controls-api-openapi.yml
- filename: anthid-com-symbol-time-controls-api-openapi.yml
  format: yaml
  label: anthid-com Symbol Time Controls API
  slug: anthid-com-symbol-time-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-symbol-time-controls-api-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 22
kind: agentic-access
layout: agentic-access
method: generated
name: Anthid Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/controls/accounts/{account_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/controls/accounts/{account_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/controls/accounts/{account_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/controls/accounts/{account_id}/risk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/controls/accounts/{account_id}/risk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/controls/accounts/{account_id}/risk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/controls/accounts/{account_id}/symbols/{symbol}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/controls/accounts/{account_id}/symbols/{symbol}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/controls/accounts/{account_id}/symbols/{symbol}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/controls/accounts/{account_id}/symbols/{symbol}/risk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/controls/accounts/{account_id}/symbols/{symbol}/risk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/controls/accounts/{account_id}/symbols/{symbol}/risk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/controls/accounts/{account_id}/symbols/{symbol}/time
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/controls/accounts/{account_id}/symbols/{symbol}/time
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/controls/accounts/{account_id}/symbols/{symbol}/time
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/controls/accounts/{account_id}/time
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/controls/accounts/{account_id}/time
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/controls/accounts/{account_id}/time
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/controls/evaluate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/controls/organizations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/controls/organizations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/controls/organizations
operation_count: 32
overview: 'anthid-com exposes 32 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 22 safety-critical.


  22 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: anthid-com
provider_slug: anthid-com
slug: anthid-com-agentic-access
source_filename: anthid-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/controls.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 10\n    acting: 22\n  by_consequence:\n    read: 10\n    safety-critical: 22\n  human_in_the_loop_required: 22\noperations:\n- path: /v1/controls/accounts/{account_id}\n  method: get\n  operationId: getAccountControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/accounts/{account_id}\n  method: put\n  operationId: upsertAccountControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}\n  method: delete\n  operationId: deleteAccountControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}\n  method: patch\n  operationId: patchAccountControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /v1/controls/accounts/{account_id}/history\n  method: get\n  operationId: listAccountControlChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/accounts/{account_id}/risk\n  method: get\n  operationId: getAccountRiskControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/accounts/{account_id}/risk\n  method: put\n  operationId: upsertAccountRiskControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/risk\n  method: delete\n  operationId:\
  \ deleteAccountRiskControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/risk\n  method: patch\n  operationId: patchAccountRiskControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/symbols\n  method: get\n  operationId: listEffectiveSymbolControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}\n  method: get\n  operationId: getSymbolControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}\n  method: put\n  operationId: upsertSymbolControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}\n  method: delete\n  operationId: deleteSymbolControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}\n  method: patch\n  operationId: patchSymbolControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}/risk\n  method: get\n  operationId: getSymbolRiskControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}/risk\n  method: put\n  operationId: upsertSymbolRiskControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}/risk\n  method: delete\n  operationId: deleteSymbolRiskControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}/risk\n  method: patch\n  operationId: patchSymbolRiskControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}/time\n  method: get\n  operationId: getSymbolTimeControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}/time\n  method: put\n  operationId: upsertSymbolTimeControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}/time\n  method: delete\n  operationId: deleteSymbolTimeControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/symbols/{symbol}/time\n  method: patch\n  operationId: patchSymbolTimeControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/time\n  method: get\n  operationId: getAccountTimeControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/accounts/{account_id}/time\n  method: put\n  operationId: upsertAccountTimeControl\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/time\n  method: delete\n  operationId: deleteAccountTimeControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/accounts/{account_id}/time\n  method: patch\n  operationId: patchAccountTimeControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/evaluate\n  method: post\n  operationId: evaluateControls\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/organizations\n  method: get\n  operationId: getPrincipalOrganizationControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/organizations\n  method: put\n  operationId: upsertOrganizationControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/organizations\n  method: delete\n  operationId: deleteOrganizationControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/organizations\n  method: patch\n  operationId: patchOrganizationControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /v1/controls/organizations/{org_id}\n  method: get\n  operationId: getOrganizationControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/anthid-com/agentic-access/anthid-com-agentic-access.yml
summary_line: 32 operations · 22 acting · 22 human-in-the-loop
tags:
- Company
---
