---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 17
api_specs:
- filename: veezee-io-checkout-api-openapi.yml
  format: yaml
  label: veezee-io Checkout API
  slug: veezee-io-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-checkout-api-openapi.yml
- filename: veezee-io-claim-api-openapi.yml
  format: yaml
  label: veezee-io Claim API
  slug: veezee-io-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-claim-api-openapi.yml
- filename: veezee-io-keys-api-openapi.yml
  format: yaml
  label: veezee-io Keys API
  slug: veezee-io-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-keys-api-openapi.yml
- filename: veezee-io-portal-api-openapi.yml
  format: yaml
  label: veezee-io Portal API
  slug: veezee-io-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-portal-api-openapi.yml
- filename: veezee-io-recover-api-openapi.yml
  format: yaml
  label: veezee-io Recover API
  slug: veezee-io-recover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-recover-api-openapi.yml
- filename: veezee-io-reddit-api-openapi.yml
  format: yaml
  label: veezee-io Reddit API
  slug: veezee-io-reddit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-reddit-api-openapi.yml
- filename: veezee-io-rekey-api-openapi.yml
  format: yaml
  label: veezee-io Rekey API
  slug: veezee-io-rekey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-rekey-api-openapi.yml
- filename: veezee-io-usage-api-openapi.yml
  format: yaml
  label: veezee-io Usage API
  slug: veezee-io-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-usage-api-openapi.yml
- filename: veezee-io-x-api-openapi.yml
  format: yaml
  label: veezee-io X API
  slug: veezee-io-x-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-x-api-openapi.yml
- filename: veezee-io-linked-in-api-openapi.yml
  format: yaml
  label: veezee-io Linked In API
  slug: veezee-io-linked-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veezee-io/openapi/veezee-io-linked-in-api-openapi.yml
consequence_counts:
  physical: 1
  read: 17
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Veezee Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout
operation_count: 23
overview: 'veezee-io exposes 23 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: veezee-io
provider_slug: veezee-io
slug: veezee-io-agentic-access
source_filename: veezee-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/veezee-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 6\n    connected: 17\n  by_consequence:\n    write: 5\n    read: 17\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/keys/mint\n  method: post\n  operationId: mintKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/linkedin/resolve-url\n  method: get\n  operationId: resolveUrl\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkedin/profiles\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkedin/search\n  method: get\n  operationId: searchPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkedin/companies\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkedin/posts\n  method: get\n  operationId: getPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/search\n\
  \  method: get\n  operationId: redditSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/subreddits\n  method: get\n  operationId: getSubreddit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/subreddit-posts\n  method: get\n  operationId: getSubredditPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/users\n  method: get\n  operationId: getRedditUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/posts\n  method: get\n  operationId: getRedditPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reddit/resolve-url\n  method: get\n  operationId: redditResolveUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/search\n  method: get\n  operationId: xSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/profiles\n  method: get\n  operationId: getXProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/tweets\n  method: get\n  operationId: getXTweets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/tweet\n  method: get\n  operationId: getXTweet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x/resolve-url\n  method: get\n  operationId: xResolveUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claim\n  method: post\n  operationId: claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recover\n  method: post\n  operationId: recover\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rekey\n  method: post\n  operationId: rekey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/portal\n  method: post\n  operationId:\
  \ createPortalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/veezee-io/agentic-access/veezee-io-agentic-access.yml
summary_line: 23 operations · 6 acting
tags:
- Artificial Intelligence
- Data
- Data Enrichment
- Social Media
- Search
---
