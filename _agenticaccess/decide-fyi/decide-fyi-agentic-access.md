---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 18
api_specs:
- filename: decide-fyi-action-execution-api-openapi.yml
  format: yaml
  label: decide-fyi Action Execution API
  slug: decide-fyi-action-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-action-execution-api-openapi.yml
- filename: decide-fyi-anomalies-api-openapi.yml
  format: yaml
  label: decide-fyi Anomalies API
  slug: decide-fyi-anomalies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-anomalies-api-openapi.yml
- filename: decide-fyi-audit-chain-api-openapi.yml
  format: yaml
  label: decide-fyi Audit Chain API
  slug: decide-fyi-audit-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-audit-chain-api-openapi.yml
- filename: decide-fyi-benchmarks-api-openapi.yml
  format: yaml
  label: decide-fyi Benchmarks API
  slug: decide-fyi-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-benchmarks-api-openapi.yml
- filename: decide-fyi-confidence-api-openapi.yml
  format: yaml
  label: decide-fyi Confidence API
  slug: decide-fyi-confidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-confidence-api-openapi.yml
- filename: decide-fyi-counterfactuals-api-openapi.yml
  format: yaml
  label: decide-fyi Counterfactuals API
  slug: decide-fyi-counterfactuals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-counterfactuals-api-openapi.yml
- filename: decide-fyi-crm-sync-api-openapi.yml
  format: yaml
  label: decide-fyi CRM Sync API
  slug: decide-fyi-crm-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-crm-sync-api-openapi.yml
- filename: decide-fyi-decision-packets-api-openapi.yml
  format: yaml
  label: decide-fyi Decision Packets API
  slug: decide-fyi-decision-packets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-decision-packets-api-openapi.yml
- filename: decide-fyi-decision-protocol-api-openapi.yml
  format: yaml
  label: decide-fyi Decision Protocol API
  slug: decide-fyi-decision-protocol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-decision-protocol-api-openapi.yml
- filename: decide-fyi-effectiveness-api-openapi.yml
  format: yaml
  label: decide-fyi Effectiveness API
  slug: decide-fyi-effectiveness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-effectiveness-api-openapi.yml
- filename: decide-fyi-outcome-tracking-api-openapi.yml
  format: yaml
  label: decide-fyi Outcome Tracking API
  slug: decide-fyi-outcome-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-outcome-tracking-api-openapi.yml
- filename: decide-fyi-policy-patterns-api-openapi.yml
  format: yaml
  label: decide-fyi Policy Patterns API
  slug: decide-fyi-policy-patterns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-policy-patterns-api-openapi.yml
- filename: decide-fyi-registries-api-openapi.yml
  format: yaml
  label: decide-fyi Registries API
  slug: decide-fyi-registries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-registries-api-openapi.yml
- filename: decide-fyi-verification-api-openapi.yml
  format: yaml
  label: decide-fyi Verification API
  slug: decide-fyi-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/decide-fyi/openapi/decide-fyi-verification-api-openapi.yml
consequence_counts:
  read: 18
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Decide Fyi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'decide-fyi exposes 28 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: decide-fyi
provider_slug: decide-fyi
slug: decide-fyi-agentic-access
source_filename: decide-fyi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/decide-fyi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 10\n    connected: 18\n  by_consequence:\n    write: 10\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /api/decide\n  method: post\n  operationId: createDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/status\n  method: get\n  operationId: getDecisionStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/policy-bundles\n  method: get\n  operationId: listPolicyBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/rulebooks\n  method: get\n  operationId: getRulebookMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/policy-patterns\n  method: get\n  operationId: listPolicyPatterns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/receipt-keys\n  method: get\n  operationId: listReceiptKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/decision/verify\n  method: get\n  operationId: describeRecordVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/verify\n  method: post\n  operationId: verifyExportedDecisionRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/packet/verify\n  method: get\n  operationId: describeDecisionPacketVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/packet/verify\n  method: post\n  operationId: verifyDecisionPacket\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/{decision_id}\n  method: get\n  operationId: getDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/{decision_id}/verify\n  method: get\n  operationId: verifyStoredDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/{decision_id}/verify\n  method: post\n  operationId: verifyStoredOrSuppliedDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/{decision_id}/packet\n  method: get\n  operationId: getDecisionPacket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/{decision_id}/replay\n  method: post\n  operationId: replayDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/{decision_id}/diff\n  method: post\n  operationId: diffDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/{decision_id}/counterfactuals\n  method: post\n  operationId: createDecisionCounterfactuals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/{decision_id}/execution\n  method: post\n  operationId: recordDecisionExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/{decision_id}/execution\n  method: get\n  operationId: listDecisionExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/{decision_id}/outcome\n  method: post\n  operationId: recordDecisionOutcome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/{decision_id}/outcome\n  method: get\n  operationId: listDecisionOutcomes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/{decision_id}/crm-sync\n  method: post\n  operationId: recordDecisionCrmSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/decision/{decision_id}/crm-sync\n  method: get\n  operationId: listDecisionCrmSyncs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/policies/{policy_id}/effectiveness\n  method: get\n  operationId: getPolicyEffectiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/policies/{policy_id}/confidence\n  method: get\n  operationId: getPolicyConfidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/policies/{policy_id}/benchmarks\n  method: get\n  operationId: getPolicyBenchmarks\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/policies/{policy_id}/anomalies\n  method: get\n  operationId: getPolicyAnomalies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decision/chains/{chain_id}\n  method: get\n  operationId: getDecisionChain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/decide-fyi/agentic-access/decide-fyi-agentic-access.yml
summary_line: 28 operations · 10 acting
tags:
- Decision API
- Rule Engine
- Software-as-a-Service
- Automation
- Runtime
---
