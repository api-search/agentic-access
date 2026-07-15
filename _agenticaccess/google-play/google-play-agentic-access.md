---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Play Developer API
  slug: google-play-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-play/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Play Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Google Play Developer exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Play Developer
provider_slug: google-play
slug: google-play-agentic-access
source_filename: google-play-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 1\n    connected: 3\n  by_consequence:\n    write: 1\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /androidpublisher/v3/applications/{packageName}/edits\n  method: post\n  operationId: createEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/androidpublisher\n- path: /androidpublisher/v3/applications/{packageName}/inappproducts\n\
  \  method: get\n  operationId: listInAppProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/androidpublisher\n- path: /androidpublisher/v3/applications/{packageName}/purchases/products/{productId}/tokens/{token}\n  method: get\n  operationId: getPurchaseStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/androidpublisher\n- path: /androidpublisher/v3/applications/{packageName}/purchases/subscriptionsv2/tokens/{token}\n  method: get\n  operationId: getSubscriptionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/androidpublisher\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-play/refs/heads/main/agentic-access/google-play-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Android
- Apps
- Google Play
- In-App Purchases
- Mobile
- Publishing
- Subscriptions
---
