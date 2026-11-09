---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 14
api_specs:
- filename: cartviral-com-account-api-openapi.yml
  format: yaml
  label: CartViral Account API
  slug: cartviral-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-account-api-openapi.yml
- filename: cartviral-com-carousels-api-openapi.yml
  format: yaml
  label: CartViral Carousels API
  slug: cartviral-com-carousels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-carousels-api-openapi.yml
- filename: cartviral-com-characters-api-openapi.yml
  format: yaml
  label: CartViral Characters API
  slug: cartviral-com-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-characters-api-openapi.yml
- filename: cartviral-com-clips-api-openapi.yml
  format: yaml
  label: CartViral Clips API
  slug: cartviral-com-clips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-clips-api-openapi.yml
- filename: cartviral-com-create-api-openapi.yml
  format: yaml
  label: CartViral Create API
  slug: cartviral-com-create-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-create-api-openapi.yml
- filename: cartviral-com-creations-api-openapi.yml
  format: yaml
  label: CartViral Creations API
  slug: cartviral-com-creations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-creations-api-openapi.yml
- filename: cartviral-com-media-api-openapi.yml
  format: yaml
  label: CartViral Media API
  slug: cartviral-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-media-api-openapi.yml
- filename: cartviral-com-offers-api-openapi.yml
  format: yaml
  label: CartViral Offers API
  slug: cartviral-com-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-offers-api-openapi.yml
- filename: cartviral-com-photos-api-openapi.yml
  format: yaml
  label: CartViral Photos API
  slug: cartviral-com-photos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-photos-api-openapi.yml
- filename: cartviral-com-pitches-api-openapi.yml
  format: yaml
  label: CartViral Pitches API
  slug: cartviral-com-pitches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-pitches-api-openapi.yml
- filename: cartviral-com-products-api-openapi.yml
  format: yaml
  label: CartViral Products API
  slug: cartviral-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-products-api-openapi.yml
- filename: cartviral-com-static-ads-api-openapi.yml
  format: yaml
  label: CartViral Static Ads API
  slug: cartviral-com-static-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-static-ads-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cartviral Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pitches
operation_count: 34
overview: 'CartViral exposes 34 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 19 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CartViral
provider_slug: cartviral-com
slug: cartviral-com-agentic-access
source_filename: cartviral-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/cartviral-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 14\n    acting: 20\n  by_consequence:\n    read: 14\n    write: 19\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /products/import\n  method: post\n  operationId: importProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /products/{product_id}/listing-copy\n  method: get\n  operationId: getListingCopy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /products/{product_id}/copy/{tool}\n  method: get\n  operationId: getCopy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /clips\n  method: post\n  operationId: generateClips\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /clips\n  method: get\n  operationId: listClips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /clips/remake\n  method: post\n  operationId: remakeFromReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /photos\n  method: post\n  operationId: generatePhotos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /photos\n  method: get\n  operationId: listPhotoSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /carousels\n  method: post\n  operationId: generateCarousel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /carousels\n  method: get\n  operationId: listCarousels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /static-ads\n  method: post\n  operationId: generateStaticAds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /static-ads\n  method: get\n  operationId: listStaticAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /offers\n  method: get\n  operationId: listOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /offers/{offer_id}/join\n  method: post\n  operationId: joinOffer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /pitches\n  method: post\n  operationId: createPitch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /pitches\n  method: get\n  operationId: listPitches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /create/options\n  method: get\n  operationId: getCreateOptions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /media\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /create/image\n  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /create/video\n  method: post\n  operationId: createVideo\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /create/angles\n  method: post\n  operationId: makeAngles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /create/talking-photo\n  method: post\n  operationId: makeTalkingPhoto\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /create/cinematic\n\
  \  method: post\n  operationId: makeCinematic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /create/reframe\n  method: post\n  operationId: reframeVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /create/remove-background\n  method: post\n  operationId: removeBackground\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /create/motion\n  method: post\n  operationId: copyMotion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /create/breakdown\n  method: post\n  operationId: breakdownVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /creations\n  method: get\n  operationId: listCreations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /creations/{job_id}\n  method: get\n  operationId: getCreation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /characters\n  method: post\n  operationId: createCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n- path: /characters\n  method: get\n  operationId: listCharacters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - mcp\n- path: /characters/save\n  method: post\n  operationId: saveCharacter\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - mcp\n"
source_yaml_url: https://artifacts.apis.io/cartviral-com/agentic-access/cartviral-com-agentic-access.yml
summary_line: 34 operations · 20 acting
tags:
- Company
- Artificial Intelligence
- E-Commerce
- Video Generation
- Marketing
---
