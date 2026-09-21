---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 18
api_specs:
- filename: charitysense-com-openapi.yml
  format: yaml
  label: CharitySense Data API
  slug: charitysense-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charitysense-com/refs/heads/main/openapi/charitysense-com-openapi.yml
consequence_counts:
  read: 18
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Charitysense Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'CharitySense exposes 21 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CharitySense
provider_slug: charitysense-com
slug: charitysense-com-agentic-access
source_filename: charitysense-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/charitysense-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 18\n    acting: 3\n  by_consequence:\n    read: 18\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/usage\n  method: get\n  operationId: getApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/stats\n  method: get\n \
  \ operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/top-lists\n  method: get\n  operationId: getTopLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/search\n  method: get\n  operationId: searchOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/page\n  method: get\n  operationId: getCharityPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/brand-icon\n  method: get\n  operationId: getCharityBrandIcon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/sections/{SectionId}\n  method: get\n  operationId: getCharitySection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/filings\n  method: get\n  operationId: getCharityFilings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/money-network\n  method: get\n  operationId: getCharityMoneyNetwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/awards\n  method: get\n  operationId: getCharityAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/subawards\n  method: get\n  operationId: getCharitySubawards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/grantees\n  method: get\n  operationId: getCharityGrantees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/funders\n  method: get\n  operationId: getCharityFunders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/funders/for-cohort\n  method: get\n  operationId: getFundersForCohort\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/{ein}/discovery\n\
  \  method: get\n  operationId: discoverRelatedOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity/diligence-summary\n  method: get\n  operationId: getDiligenceSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/charity-question\n  method: post\n  operationId: submitCharityQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/agent-feedback\n  method: post\n  operationId: submitAgentFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/assistant/capabilities\n  method: get\n  operationId: getAssistantCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/assistant/chat/stream\n  method: post\n  operationId: streamAssistantChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charitysense-com/refs/heads/main/agentic-access/charitysense-com-agentic-access.yml
summary_line: 21 operations · 3 acting
tags:
- Non-Profit
- Charities
- Due Diligence
- IRS Form 990
- Donor Research
- Grants
- Philanthropy
- Open Data
- Agents
- A2A
- Impact Verification
- Edge AI
- United States
- Company
---
