---
acting_count: 0
action_class_counts:
  acting: 0
  connected: 11
api_specs:
- filename: optionsahoy-com-openapi.json
  format: json
  label: OptionsAhoy Calculator API
  slug: optionsahoy-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optionsahoy-com/refs/heads/main/openapi/optionsahoy-com-openapi.json
consequence_counts:
  physical: 0
  read: 11
  write: 0
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Optionsahoy Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'AlphaLatitude Inc. exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AlphaLatitude Inc.
provider_slug: optionsahoy-com
slug: optionsahoy-com-agentic-access
source_filename: optionsahoy-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/optionsahoy-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance\n  starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n    acting: 0\n  by_consequence:\n    read: 11\n    write: 0\n    physical: 0\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: discover\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/amt-iso\n  method: post\n  operationId: optimizeAmtIso\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    x-curated:\n\
  \      was:\n        action-class: acting\n        consequence: write\n      basis: POST is a stateless pure computation; the provider's live MCP tools/list annotates the identical operation\n        (amt_iso_optimize) readOnlyHint true, idempotentHint true, destructiveHint false, openWorldHint false, and\n        SECURITY.md states 'No accounts, no authentication, no stored user data ... Inputs are not retained.' Nothing\n        is created, sent, spent or deleted.\n- path: /api/v1/nso\n  method: post\n  operationId: calculateNso\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    x-curated:\n      was:\n        action-class: acting\n        consequence: write\n      basis: POST is a stateless pure computation; the provider's live MCP tools/list annotates the identical operation\n        (nso_calculate) readOnlyHint true, idempotentHint true, destructiveHint false, openWorldHint\
  \ false, and\n        SECURITY.md states 'No accounts, no authentication, no stored user data ... Inputs are not retained.' Nothing\n        is created, sent, spent or deleted.\n- path: /api/v1/rsu-sell-vs-hold\n  method: post\n  operationId: calculateRsu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    x-curated:\n      was:\n        action-class: acting\n        consequence: write\n      basis: POST is a stateless pure computation; the provider's live MCP tools/list annotates the identical operation\n        (rsu_sell_vs_hold) readOnlyHint true, idempotentHint true, destructiveHint false, openWorldHint false, and\n        SECURITY.md states 'No accounts, no authentication, no stored user data ... Inputs are not retained.' Nothing\n        is created, sent, spent or deleted.\n- path: /api/v1/concentration\n  method: post\n  operationId: calculateConcentration\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    x-curated:\n      was:\n        action-class: acting\n        consequence: write\n      basis: POST is a stateless pure computation; the provider's live MCP tools/list annotates the identical operation\n        (concentration_analyze) readOnlyHint true, idempotentHint true, destructiveHint false, openWorldHint false,\n        and SECURITY.md states 'No accounts, no authentication, no stored user data ... Inputs are not retained.'\n        Nothing is created, sent, spent or deleted.\n- path: /api/v1/protective-put\n  method: post\n  operationId: priceProtectivePut\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    x-curated:\n      was:\n        action-class: acting\n        consequence: write\n      basis: POST is a stateless\
  \ pure computation; the provider's live MCP tools/list annotates the identical operation\n        (protective_put_price) readOnlyHint true, idempotentHint true, destructiveHint false, openWorldHint false,\n        and SECURITY.md states 'No accounts, no authentication, no stored user data ... Inputs are not retained.'\n        Nothing is created, sent, spent or deleted.\n- path: /api/v1/qsbs\n  method: post\n  operationId: checkQsbs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    x-curated:\n      was:\n        action-class: acting\n        consequence: write\n      basis: POST is a stateless pure computation; the provider's live MCP tools/list annotates the identical operation\n        (qsbs_check) readOnlyHint true, idempotentHint true, destructiveHint false, openWorldHint false, and SECURITY.md\n        states 'No accounts, no authentication, no stored user data\
  \ ... Inputs are not retained.' Nothing is created,\n        sent, spent or deleted.\n- path: /api/v1/equity-funding\n  method: post\n  operationId: planEquityFunding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    x-curated:\n      was:\n        action-class: acting\n        consequence: write\n      basis: POST is a stateless pure computation; the provider's live MCP tools/list annotates the identical operation\n        (equity_funding_plan) readOnlyHint true, idempotentHint true, destructiveHint false, openWorldHint false,\n        and SECURITY.md states 'No accounts, no authentication, no stored user data ... Inputs are not retained.'\n        Nothing is created, sent, spent or deleted.\n- path: /api/v1/rsu-lot-order\n  method: post\n  operationId: optimizeRsuLotOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    x-curated:\n      was:\n        action-class: acting\n        consequence: physical\n      basis: POST is a stateless pure computation; the provider's live MCP tools/list annotates the identical operation\n        (rsu_lot_optimize) readOnlyHint true, idempotentHint true, destructiveHint false, openWorldHint false, and\n        SECURITY.md states 'No accounts, no authentication, no stored user data ... Inputs are not retained.' Nothing\n        is created, sent, spent or deleted.\n- path: /api/v1/stats\n  method: get\n  operationId: stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/badge\n  method: get\n  operationId: badge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\nx-curated:\n  date: '2026-09-19'\n\
  \  by: API Evangelist enrichment pass\n  note: 'The heuristic classifier read the eight POST calculators as acting/write (planEquityFunding as physical,\n    on the ''fund''/''sell'' vocabulary). That is the wrong contract for this API: every operation is read-only\n    by the provider''s own machine-readable declaration (mcp/optionsahoy-com-mcp-tools.json annotations) and by\n    its security policy. Reclassified to connected/read with the generated values preserved under x-curated.was\n    so the change is auditable. The three GET operations were already connected/read.'\n  evidence:\n  - mcp/optionsahoy-com-mcp-tools.json — annotations.readOnlyHint true on 8 of 8 tools\n  - https://github.com/AlvisoOculus/optionsahoy-mcp/blob/main/SECURITY.md\n  - conventions/optionsahoy-com-conventions.yml — reversibility grade na, no write surface\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optionsahoy-com/refs/heads/main/agentic-access/optionsahoy-com-agentic-access.yml
summary_line: 11 operations
tags:
- Equity Compensation
- Tax
- Stock Options
- Financial Planning
- Personal Finance
- Fintech
- Calculators
- MCP
- A2A
- agent-native
- Deterministic
- United States
---
