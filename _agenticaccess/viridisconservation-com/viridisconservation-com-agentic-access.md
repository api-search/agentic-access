---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 1
api_specs:
- filename: viridisconservation-com-adoption-api-openapi.yml
  format: yaml
  label: viridisconservation-com Adoption API
  slug: viridisconservation-com-adoption-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-adoption-api-openapi.yml
- filename: viridisconservation-com-agents-api-openapi.yml
  format: yaml
  label: viridisconservation-com Agents API
  slug: viridisconservation-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-agents-api-openapi.yml
- filename: viridisconservation-com-climate-api-openapi.yml
  format: yaml
  label: viridisconservation-com Climate API
  slug: viridisconservation-com-climate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-climate-api-openapi.yml
- filename: viridisconservation-com-climate-compliance-api-openapi.yml
  format: yaml
  label: viridisconservation-com Climate Compliance API
  slug: viridisconservation-com-climate-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-climate-compliance-api-openapi.yml
- filename: viridisconservation-com-conservation-api-openapi.yml
  format: yaml
  label: viridisconservation-com Conservation API
  slug: viridisconservation-com-conservation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-conservation-api-openapi.yml
- filename: viridisconservation-com-construction-api-openapi.yml
  format: yaml
  label: viridisconservation-com Construction API
  slug: viridisconservation-com-construction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-construction-api-openapi.yml
- filename: viridisconservation-com-csrd-api-openapi.yml
  format: yaml
  label: viridisconservation-com Csrd API
  slug: viridisconservation-com-csrd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-csrd-api-openapi.yml
- filename: viridisconservation-com-ghg-api-openapi.yml
  format: yaml
  label: viridisconservation-com Ghg API
  slug: viridisconservation-com-ghg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-ghg-api-openapi.yml
- filename: viridisconservation-com-routing-api-openapi.yml
  format: yaml
  label: viridisconservation-com Routing API
  slug: viridisconservation-com-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-routing-api-openapi.yml
- filename: viridisconservation-com-security-api-openapi.yml
  format: yaml
  label: viridisconservation-com Security API
  slug: viridisconservation-com-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-security-api-openapi.yml
- filename: viridisconservation-com-security-preflight-api-openapi.yml
  format: yaml
  label: viridisconservation-com Security Preflight API
  slug: viridisconservation-com-security-preflight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-security-preflight-api-openapi.yml
- filename: viridisconservation-com-tax-credit-api-openapi.yml
  format: yaml
  label: viridisconservation-com Tax Credit API
  slug: viridisconservation-com-tax-credit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/viridisconservation-com/openapi/viridisconservation-com-tax-credit-api-openapi.yml
consequence_counts:
  read: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Viridisconservation Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'viridisconservation-com exposes 17 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: viridisconservation-com
provider_slug: viridisconservation-com
slug: viridisconservation-com-agentic-access
source_filename: viridisconservation-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/viridisconservation-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 16\n    connected: 1\n  by_consequence:\n    write: 16\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /x402/regulatory-radar/scan_regulations\n  method: post\n  operationId: x402_regulatory_radar_scan_regulations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/regulatory-radar/monitor_changes\n  method:\
  \ post\n  operationId: x402_regulatory_radar_monitor_changes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/taxcredit-engine/calculate_tax_credit\n  method: post\n  operationId: x402_taxcredit_engine_calculate_tax_credit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/ghg-ledger/calculate_inventory\n  method: post\n  operationId: x402_ghg_ledger_calculate_inventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/quantity-takeoff/calculate_takeoff\n  method: post\n  operationId: x402_quantity_takeoff_calculate_takeoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/disclosure-compiler/compile_disclosure\n  method: post\n  operationId: x402_disclosure_compiler_compile_disclosure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/hive/solve\n  method: post\n  operationId: x402_hive_solve\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/security-preflight/security_preflight\n  method: post\n  operationId: x402_security_preflight_security_preflight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/security-preflight/scan_source\n  method: post\n  operationId: x402_security_preflight_scan_source\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/security-preflight/screen_injection\n  method: post\n  operationId: x402_security_preflight_screen_injection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/os-decisions/build_decision_report\n  method: post\n  operationId: x402_os_decisions_build_decision_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/wu-wei-router/plan_workload\n  method: post\n  operationId: x402_wu_wei_router_plan_workload\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/maxwell-defense/rehearse_defense\n  method: post\n  operationId: x402_maxwell_defense_rehearse_defense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security-preflight/watch\n  method: post\n  operationId: plan_security_preflight_recheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /security-preflight/receipts/{receipt_id}\n  method: get\n  operationId: get_public_security_preflight_receipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adopt\n  method: post\n  operationId: plan_viridis_adoption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/feedback\n  method: post\n  operationId: submit_paid_result_feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/viridisconservation-com/agentic-access/viridisconservation-com-agentic-access.yml
summary_line: 17 operations · 16 acting
tags:
- Conservation
- Environment
- Data
- Software-as-a-Service
---
