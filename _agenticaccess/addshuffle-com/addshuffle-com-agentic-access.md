---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 5
api_specs:
- filename: addshuffle-com-credits-api-openapi.yml
  format: yaml
  label: Shuffle Credits API
  slug: addshuffle-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addshuffle-com/openapi/addshuffle-com-credits-api-openapi.yml
- filename: addshuffle-com-l402-api-openapi.yml
  format: yaml
  label: Shuffle L402 API
  slug: addshuffle-com-l402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addshuffle-com/openapi/addshuffle-com-l402-api-openapi.yml
- filename: addshuffle-com-manual-mode-api-openapi.yml
  format: yaml
  label: Shuffle Manual Mode API
  slug: addshuffle-com-manual-mode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addshuffle-com/openapi/addshuffle-com-manual-mode-api-openapi.yml
- filename: addshuffle-com-utilities-api-openapi.yml
  format: yaml
  label: Shuffle Utilities API
  slug: addshuffle-com-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addshuffle-com/openapi/addshuffle-com-utilities-api-openapi.yml
- filename: addshuffle-com-video-chain-api-openapi.yml
  format: yaml
  label: Shuffle Video Chain API
  slug: addshuffle-com-video-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addshuffle-com/openapi/addshuffle-com-video-chain-api-openapi.yml
consequence_counts:
  physical: 3
  read: 5
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Addshuffle Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/l402/payment-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/longform-video/credits/charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/longform-video/credits/checkout
operation_count: 17
overview: 'Shuffle exposes 17 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 9 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Shuffle
provider_slug: addshuffle-com
slug: addshuffle-com-agentic-access
source_filename: addshuffle-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/addshuffle-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 12\n    connected: 5\n  by_consequence:\n    write: 9\n    read: 5\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/longform-video/generate\n  method: post\n  operationId: createVideoChain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/longform-video/status/{chainId}\n  method: get\n  operationId: getVideoChainStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/longform-video/cancel-chain\n  method: post\n  operationId: cancelVideoChain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/longform-video/retry-step\n  method: post\n  operationId: retryStep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/longform-video/recreate-clip\n  method: post\n  operationId: recreateClip\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/longform-video/add-clip\n  method: post\n  operationId: addClip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/longform-video/extend-clip\n  method: post\n  operationId: extendClip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/longform-video/select-version\n\
  \  method: post\n  operationId: selectVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/longform-video/stitch\n  method: post\n  operationId: stitchVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/longform-video/upload\n  method: post\n  operationId: uploadImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /api/longform-video/credits/balance\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/longform-video/credits/history\n  method: get\n  operationId: getCreditHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/longform-video/credits/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/longform-video/credits/charge\n  method: post\n\
  \  operationId: chargeCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/l402/offers\n  method: get\n  operationId: listL402Offers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/l402/payment-request\n  method: post\n  operationId: createL402PaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/l402/payment-status/{id}\n  method: get\n  operationId: getL402PaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/addshuffle-com/agentic-access/addshuffle-com-agentic-access.yml
summary_line: 17 operations · 12 acting
tags:
- Artificial Intelligence
- Social Media
- Automation
- Marketing
- Software-as-a-Service
---
