---
acting_count: 49
action_class_counts:
  acting: 49
  connected: 13
api_specs:
- filename: cloudforbots-com-agent-wake-api-openapi.yml
  format: yaml
  label: cloudforbots-com Agent Wake API
  slug: cloudforbots-com-agent-wake-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-agent-wake-api-openapi.yml
- filename: cloudforbots-com-approval-rules-api-openapi.yml
  format: yaml
  label: cloudforbots-com Approval Rules API
  slug: cloudforbots-com-approval-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-approval-rules-api-openapi.yml
- filename: cloudforbots-com-audit-api-openapi.yml
  format: yaml
  label: cloudforbots-com Audit API
  slug: cloudforbots-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-audit-api-openapi.yml
- filename: cloudforbots-com-browser-api-openapi.yml
  format: yaml
  label: cloudforbots-com Browser API
  slug: cloudforbots-com-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-browser-api-openapi.yml
- filename: cloudforbots-com-budget-guard-api-openapi.yml
  format: yaml
  label: cloudforbots-com Budget Guard API
  slug: cloudforbots-com-budget-guard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-budget-guard-api-openapi.yml
- filename: cloudforbots-com-bus-api-openapi.yml
  format: yaml
  label: cloudforbots-com Bus API
  slug: cloudforbots-com-bus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-bus-api-openapi.yml
- filename: cloudforbots-com-coordination-api-openapi.yml
  format: yaml
  label: cloudforbots-com Coordination API
  slug: cloudforbots-com-coordination-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-coordination-api-openapi.yml
- filename: cloudforbots-com-cron-api-openapi.yml
  format: yaml
  label: cloudforbots-com Cron API
  slug: cloudforbots-com-cron-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-cron-api-openapi.yml
- filename: cloudforbots-com-key-api-openapi.yml
  format: yaml
  label: cloudforbots-com Key API
  slug: cloudforbots-com-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-key-api-openapi.yml
- filename: cloudforbots-com-ledger-api-openapi.yml
  format: yaml
  label: cloudforbots-com Ledger API
  slug: cloudforbots-com-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-ledger-api-openapi.yml
- filename: cloudforbots-com-loop-breaker-api-openapi.yml
  format: yaml
  label: cloudforbots-com Loop Breaker API
  slug: cloudforbots-com-loop-breaker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-loop-breaker-api-openapi.yml
- filename: cloudforbots-com-queue-api-openapi.yml
  format: yaml
  label: cloudforbots-com Queue API
  slug: cloudforbots-com-queue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-queue-api-openapi.yml
- filename: cloudforbots-com-run-api-openapi.yml
  format: yaml
  label: cloudforbots-com Run API
  slug: cloudforbots-com-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-run-api-openapi.yml
- filename: cloudforbots-com-run-memory-api-openapi.yml
  format: yaml
  label: cloudforbots-com Run Memory API
  slug: cloudforbots-com-run-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-run-memory-api-openapi.yml
- filename: cloudforbots-com-sandbox-api-openapi.yml
  format: yaml
  label: cloudforbots-com Sandbox API
  slug: cloudforbots-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-sandbox-api-openapi.yml
- filename: cloudforbots-com-secrets-api-openapi.yml
  format: yaml
  label: cloudforbots-com Secrets API
  slug: cloudforbots-com-secrets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-secrets-api-openapi.yml
- filename: cloudforbots-com-storage-api-openapi.yml
  format: yaml
  label: cloudforbots-com Storage API
  slug: cloudforbots-com-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-storage-api-openapi.yml
- filename: cloudforbots-com-webhooks-api-openapi.yml
  format: yaml
  label: cloudforbots-com Webhooks API
  slug: cloudforbots-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudforbots-com/openapi/cloudforbots-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 13
  safety-critical: 4
  write: 43
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudforbots Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/run/budget_status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/run/weekly_report
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/browser
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/sandbox
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/webhooks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/webhooks/redeliver/{id}
operation_count: 62
overview: 'cloudforbots-com exposes 62 API operations that an AI agent could call, of which 49 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 43 write, 2 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: cloudforbots-com
provider_slug: cloudforbots-com
slug: cloudforbots-com-agentic-access
source_filename: cloudforbots-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/approve-cloudforbots-com-openapi.json, openapi/budget-cloudforbots-com-openapi.json,\n  openapi/cloudforbots-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 62\n  by_action_class:\n    acting: 49\n    connected: 13\n  by_consequence:\n    write: 43\n    read: 13\n    safety-critical: 4\n    physical: 2\n  human_in_the_loop_required: 4\noperations:\n- path: /api/run/check_action\n  method: post\n  operationId: check_action\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/run/get_decision\n  method: post\n  operationId: get_decision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/run/set_rules\n  method: post\n  operationId: set_rules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/run/get_rules\n  method: post\n  operationId: get_rules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/run/weekly_report\n  method: post\n  operationId: weekly_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/key\n  method: post\n  operationId: get_free_key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/run/open_budget\n  method: post\n  operationId: open_budget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/run/reserve\n  method: post\n  operationId: reserve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/run/record\n  method: post\n  operationId: record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/run/weekly_report\n  method: post\n  operationId: weekly_report\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/run/budget_status\n  method: post\n  operationId: budget_status\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/key\n  method: post\n  operationId: get_free_key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/loop-breaker/check_step\n  method: post\n  operationId: loop_breaker__check_step\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/loop-breaker/loop_status\n  method: post\n  operationId: loop_breaker__loop_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/loop-breaker/weekly_report\n  method: post\n  operationId: loop_breaker__weekly_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/loop-breaker/usage_and_upgrade\n  method: post\n  operationId: loop_breaker__usage_and_upgrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/run-memory/save_checkpoint\n  method: post\n  operationId: run_memory__save_checkpoint\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/run-memory/resume\n  method: post\n  operationId: run_memory__resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/run-memory/list_checkpoints\n  method: post\n  operationId: run_memory__list_checkpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/run-memory/weekly_report\n  method: post\n  operationId: run_memory__weekly_report\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/run-memory/usage_and_upgrade\n  method: post\n  operationId: run_memory__usage_and_upgrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/budget-guard/open_budget\n  method: post\n  operationId: budget_guard__open_budget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api/v1/budget-guard/reserve\n  method: post\n  operationId: budget_guard__reserve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/budget-guard/record\n  method: post\n  operationId: budget_guard__record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/budget-guard/weekly_report\n  method: post\n  operationId: budget_guard__weekly_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/budget-guard/budget_status\n  method: post\n  operationId: budget_guard__budget_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/budget-guard/usage_and_upgrade\n  method: post\n  operationId: budget_guard__usage_and_upgrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/approval-rules/check_action\n  method: post\n  operationId: approval_rules__check_action\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/approval-rules/get_decision\n  method: post\n  operationId: approval_rules__get_decision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/approval-rules/set_rules\n  method: post\n  operationId: approval_rules__set_rules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/approval-rules/get_rules\n  method: post\n  operationId: approval_rules__get_rules\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/approval-rules/weekly_report\n  method: post\n  operationId: approval_rules__weekly_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/approval-rules/usage_and_upgrade\n  method: post\n  operationId: approval_rules__usage_and_upgrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-wake/schedule_wake\n  method: post\n  operationId: agent_wake__schedule_wake\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-wake/check_wakes\n  method: post\n  operationId: agent_wake__check_wakes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agent-wake/cancel_wake\n  method: post\n  operationId: agent_wake__cancel_wake\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/agent-wake/usage_and_upgrade\n  method: post\n  operationId: agent_wake__usage_and_upgrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/secrets\n  method: post\n  operationId: secrets__call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fetch\n  method: post\n  operationId: fetch__call\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/queue\n  method:\
  \ post\n  operationId: queue__call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cron\n  method: post\n  operationId: cron__call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/browser\n  method: post\n  operationId: browser__call\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/v1/lock\n  method: post\n  operationId: lock__call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/rate\n  method: post\n  operationId: rate__call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inbox\n  method: post\n  operationId: inbox__call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/topic\n  method: post\n  operationId: topic__call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ledger\n  method: post\n  operationId: ledger__call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox\n  method: post\n  operationId: sandbox__call\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/store\n  method: post\n  operationId: store__call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/store/kv/{ns}/{key}\n  method: get\n  operationId: store__kv_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/store/kv/{ns}/{key}\n  method: put\n  operationId: store__kv_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/store/kv/{ns}/{key}\n  method: delete\n  operationId: store__kv_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/store/files/{ns}/{name}\n  method: get\n  operationId: store__file_download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/store/files/{ns}/{name}\n  method: put\n  operationId: store__file_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/store/files/{ns}/{name}\n  method: delete\n  operationId: store__file_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/deliveries\n  method: get\n  operationId: webhooks__deliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/redeliver/{id}\n  method: post\n  operationId: webhooks__redeliver\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/rotate\n  method: post\n  operationId: webhooks__rotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks\n  method: get\n  operationId: webhooks__list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  operationId: webhooks__add\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /api/v1/webhooks\n  method: delete\n  operationId: webhooks__remove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audit\n  method: get\n  operationId: audit__list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cloudforbots-com/agentic-access/cloudforbots-com-agentic-access.yml
summary_line: 62 operations · 49 acting · 4 human-in-the-loop
tags:
- Company
- Bot
- Artificial Intelligence
- Platform
- Sandbox
- MCP
- Cloud
---
