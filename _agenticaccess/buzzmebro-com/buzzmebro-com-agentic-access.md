---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 8
api_specs:
- filename: buzzmebro-com-applications-api-openapi.yml
  format: yaml
  label: BuzzMeBro Applications API
  slug: buzzmebro-com-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-applications-api-openapi.yml
- filename: buzzmebro-com-check-api-openapi.yml
  format: yaml
  label: BuzzMeBro Check API
  slug: buzzmebro-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-check-api-openapi.yml
- filename: buzzmebro-com-info-api-openapi.yml
  format: yaml
  label: BuzzMeBro Info API
  slug: buzzmebro-com-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-info-api-openapi.yml
- filename: buzzmebro-com-me-api-openapi.yml
  format: yaml
  label: BuzzMeBro Me API
  slug: buzzmebro-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-me-api-openapi.yml
- filename: buzzmebro-com-setups-api-openapi.yml
  format: yaml
  label: BuzzMeBro Setups API
  slug: buzzmebro-com-setups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-setups-api-openapi.yml
consequence_counts:
  physical: 3
  read: 8
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Buzzmebro Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /me/sublinks/{sublink_id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{application_id}/code
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /me/payout-link
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /setups/{setup_id}/phone-code
operation_count: 20
overview: 'BuzzMeBro exposes 20 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 8 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BuzzMeBro
provider_slug: buzzmebro-com
slug: buzzmebro-com-agentic-access
source_filename: buzzmebro-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/buzzmebro-com-agent-openapi.json, openapi/buzzmebro-com-partner-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 12\n    connected: 8\n  by_consequence:\n    write: 8\n    physical: 3\n    read: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /check\n  method: post\n  operationId: checkBuilding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setups\n  method: post\n  operationId:\
  \ createSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setups/{setup_id}/phone-code\n  method: post\n  operationId: sendPhoneCode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setups/{setup_id}/phone-code/verify\n  method: post\n  operationId: confirmPhoneCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setups/{setup_id}/checkout\n  method: post\n  operationId: startCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /setups/{setup_id}\n  method: get\n  operationId: getSetupStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info\n  method: get\n  operationId: partnerProgramInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: post\n  operationId: partnerApply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/code\n  method: post\n  operationId: partnerSendCode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/code/verify\n  method: post\n  operationId: partnerConfirmCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/terms-link\n  method: post\n  operationId: partnerTermsLink\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}/key\n  method: post\n  operationId: partnerClaimKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/links\n  method: get\n  operationId: partnerGetLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/kit\n  method: get\n  operationId: partnerGetKit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/stats\n  method: get\n  operationId: partnerGetStats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/payout-link\n  method: post\n  operationId: partnerPayoutLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/sublinks\n  method: get\n  operationId: partnerListSublinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/sublinks\n  method: post\n  operationId: partnerCreateSublink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/sublinks/{sublink_id}/disable\n  method: post\n  operationId: partnerDisableSublink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /me/key/rotate\n  method: post\n  operationId: partnerRotateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/buzzmebro-com/agentic-access/buzzmebro-com-agentic-access.yml
summary_line: 20 operations · 12 acting · 1 human-in-the-loop
tags:
- Company
- Buzzer
- Apartments
- Access
- Subscription
- Toronto
---
