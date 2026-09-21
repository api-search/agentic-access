---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
consequence_counts:
  physical: 6
  read: 6
description: 'Recommended x-agentic-access execution contracts for the twelve operations Verse''s agent card names. There is no OpenAPI, so the heuristic derive-agentic-access.py could not run; the action-class and auth requirement are read from the provider''s OWN Agent Gateway Protocol policy block (requiresAuth, cost, mode, dataScope per capability) and its securityRequirements (public vs x402Payment per skill), which is why the method is searched rather than generated. consequence is API Evangelist''s reading: every paid call is an irreversible on-chain USDC transfer with no published refund path, so paid operations are rated physical with human-in-the-loop required and a token TTL ceiling of 300s; the free calibration/reputation reads are connected/read. TTL ceilings mirror the agentic-access Spectral ruleset. A governance starting point, not a provider claim; audience is left null to bind per deployment. See research/curity/agentic-governance/.'
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: searched
name: Verse Me Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
operation_count: 12
overview: 'Verse (autonomous agent) exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 6 physical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Verse (autonomous agent)
provider_slug: verse-me-com
slug: verse-me-com-agentic-access
source_filename: verse-me-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.verse-me.com/.well-known/agent.json — AGP extension capabilitiesAnnounced[] policies + urn:verse:agent-extensions:v1 endpoint list + securityRequirements\ndescription: >-\n  Recommended x-agentic-access execution contracts for the twelve operations Verse's agent card names. There is no\n  OpenAPI, so the heuristic derive-agentic-access.py could not run; the action-class and auth requirement are read\n  from the provider's OWN Agent Gateway Protocol policy block (requiresAuth, cost, mode, dataScope per capability)\n  and its securityRequirements (public vs x402Payment per skill), which is why the method is searched rather than\n  generated. consequence is API Evangelist's reading: every paid call is an irreversible on-chain USDC transfer with\n  no published refund path, so paid operations are rated physical with human-in-the-loop required and a token TTL\n  ceiling of 300s; the free calibration/reputation reads\
  \ are connected/read. TTL ceilings mirror the agentic-access\n  Spectral ruleset. A governance starting point, not a provider claim; audience is left null to bind per deployment.\n  See research/curity/agentic-governance/.\naudience: null\ncustody_note: >-\n  The caller pays from a wallet it controls; Verse never holds a caller credential. The consequence ratings describe\n  what a signed x402 payment does once broadcast — it is final — not what Verse can do with the caller's keys.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 6\n    acting: 6\n  by_consequence:\n    read: 6\n    physical: 6\n  human_in_the_loop_required: 6\n  provider_policy:\n    capabilities_announced: 3\n    requiresAuth_false: 2\n    requiresAuth_true: 1\n    payment_gated_skills: 3\n    public_skills: 3\noperations:\n- operation: GET /expertise/calibration\n  skill: calibration_track_record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    provider-policy: {capability: 'expertise:calibration', requiresAuth: false, cost: 0, dataScope: aggregate_only}\n- operation: GET /expertise/calibration/signed\n  skill: signed_calibration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-policy: {capability: 'expertise:calibration:signed', requiresAuth: false, cost: 0, provenance: ed25519, dataScope: aggregate_only}\n- operation: GET /expertise/calibration/history\n  skill: calibration_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-policy: {security: public}\n- operation: GET /expertise/calibration/history/signed\n  skill: calibration_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n    provider-policy: {security: public, provenance: ed25519}\n- operation: GET /reputation\n  skill: null\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-policy: {security: public (proof bundle)}\n- operation: POST /expertise/consultation/price-estimate\n  skill: consultation (preview)\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    dry-run-for: POST /expertise/consultation\n    provider-policy: {security: public, listed under freeEndpoints as \"Preview cost before paying\"}\n- operation: POST /expertise/consultation\n  skill: consultation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    purpose-required: true\n    token:\n      max-ttl: 300\n      exchange: required\n    escalation:\n      human-in-the-loop:\
  \ required\n      reason: irreversible on-chain USDC payment ($3–$50 published); no refund or cancel path published; price is dynamic\n    audit: required\n    provider-policy: {capability: 'expertise:consultation', requiresAuth: true, cost: 0.1 (disagrees with the skill's $3–$50), mode: async, paymentProtocol: x402, paymentNetwork: 'eip155:8453', paymentAsset: USDC, provenance: ed25519}\n- operation: POST /expertise/consultation (strategy_recommendation)\n  skill: strategy_recommendation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    purpose-required: true\n    token:\n      max-ttl: 300\n      exchange: required\n    escalation:\n      human-in-the-loop: required\n      reason: paid via x402 with NO published price; the caller cannot bound the spend from the card\n    audit: required\n    provider-policy: {security: x402Payment}\n- operation: POST /expertise/epistemic-audit\n  skill: epistemic_audit\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    purpose-required: true\n    token:\n      max-ttl: 300\n      exchange: required\n    escalation:\n      human-in-the-loop: required\n      reason: paid via x402 with NO published price; irreversible\n    audit: required\n    provider-policy: {security: x402Payment}\n- operation: POST /expertise/edgar (index)\n  skill: edgar_financial_intelligence\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    purpose-required: true\n    token:\n      max-ttl: 300\n      exchange: required\n    escalation:\n      human-in-the-loop: required\n      reason: on-chain payment ($0.01 published); irreversible even at this size\n    audit: required\n    provider-policy: {security: x402Payment, price: '$0.01'}\n- operation: POST /expertise/edgar (analysis)\n  skill: edgar_financial_intelligence\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n \
  \   purpose-required: true\n    token:\n      max-ttl: 300\n      exchange: required\n    escalation:\n      human-in-the-loop: required\n      reason: on-chain payment ($0.05 published); irreversible\n    audit: required\n    provider-policy: {security: x402Payment, price: '$0.05'}\n- operation: POST /expertise/edgar (deep)\n  skill: edgar_financial_intelligence\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    purpose-required: true\n    token:\n      max-ttl: 300\n      exchange: required\n    escalation:\n      human-in-the-loop: required\n      reason: on-chain payment ($0.25 published); irreversible\n    audit: required\n    provider-policy: {security: x402Payment, price: '$0.25'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verse-me-com/refs/heads/main/agentic-access/verse-me-com-agentic-access.yml
summary_line: 12 operations · 6 acting · 6 human-in-the-loop
tags:
- Company
- AI Agents
- Autonomous Agents
- A2A
- x402
- Agentic Commerce
- Forecasting
- Predictions
- Calibration
- Financial Analysis
- SEC EDGAR
- Blockchain
- Base
- agent-native
---
