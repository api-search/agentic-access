---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: amazon-ads-openapi-generated.yml
  format: yaml
  label: Amazon Ads API
  slug: amazon-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/_ae-authored/amazon-ads-openapi-generated.yml
- filename: amazon-ads-activategiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Activategiftcard API
  slug: amazon-ads-activategiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-activategiftcard-api-openapi.yml
- filename: amazon-ads-activationstatuscheck-api-openapi.yml
  format: yaml
  label: Amazon Ads Activationstatuscheck API
  slug: amazon-ads-activationstatuscheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-activationstatuscheck-api-openapi.yml
- filename: amazon-ads-amazon-ads-api-api-openapi.yml
  format: yaml
  label: Amazon Ads Amazon Ads API
  slug: amazon-ads-amazon-ads-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-amazon-ads-api-api-openapi.yml
- filename: amazon-ads-cancelgiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Cancelgiftcard API
  slug: amazon-ads-cancelgiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-cancelgiftcard-api-openapi.yml
- filename: amazon-ads-creategiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Creategiftcard API
  slug: amazon-ads-creategiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-creategiftcard-api-openapi.yml
- filename: amazon-ads-deactivategiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Deactivategiftcard API
  slug: amazon-ads-deactivategiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-deactivategiftcard-api-openapi.yml
- filename: amazon-ads-getgiftcard-api-openapi.yml
  format: yaml
  label: Amazon Ads Getgiftcard API
  slug: amazon-ads-getgiftcard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-getgiftcard-api-openapi.yml
- filename: amazon-ads-install-api-openapi.yml
  format: yaml
  label: Amazon Ads Install API
  slug: amazon-ads-install-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ads/openapi/amazon-ads-install-api-openapi.yml
consequence_counts:
  read: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Ads Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Amazon Ads exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Ads
provider_slug: amazon-ads
slug: amazon-ads-agentic-access
source_filename: amazon-ads-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/amazon-ads-activategiftcard-api-openapi.yml, openapi/amazon-ads-activationstatuscheck-api-openapi.yml,\n  openapi/amazon-ads-amazon-ads-api-api-openapi.yml, openapi/amazon-ads-cancelgiftcard-api-openapi.yml,\n  openapi/amazon-ads-creategiftcard-api-openapi.yml, openapi/amazon-ads-deactivategiftcard-api-openapi.yml,\n  openapi/amazon-ads-getgiftcard-api-openapi.yml, openapi/amazon-ads-install-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 6\n    connected: 2\n  by_consequence:\n    write: 6\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /ActivateGiftCard\n  method: post\n  operationId: post_ActivateGiftCard\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ActivationStatusCheck\n  method: post\n  operationId: post_ActivationStatusCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CancelGiftCard\n  method: post\n  operationId: post_CancelGiftCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CreateGiftCard\n  method: post\n  operationId: post_CreateGiftCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DeactivateGiftCard\n  method: post\n  operationId: post_DeactivateGiftCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetGiftCard\n  method: post\n  operationId: post_GetGiftCard\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/install.sh\n  method: get\n  operationId: get_v2_install_sh\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/amazon-ads/agentic-access/amazon-ads-agentic-access.yml
summary_line: 8 operations · 6 acting
tags:
- Advertising
- Marketing
- Amazon
- Technology
- Software-as-a-Service
---
