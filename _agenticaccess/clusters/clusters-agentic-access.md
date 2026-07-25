---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: clusters-authentication-api-openapi.yml
  format: yaml
  label: Clusters Authentication API
  slug: clusters-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-authentication-api-openapi.yml
- filename: clusters-clusters-api-openapi.yml
  format: yaml
  label: Clusters Clusters API
  slug: clusters-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-clusters-api-openapi.yml
- filename: clusters-communities-api-openapi.yml
  format: yaml
  label: Clusters Communities API
  slug: clusters-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-communities-api-openapi.yml
- filename: clusters-events-api-openapi.yml
  format: yaml
  label: Clusters Events API
  slug: clusters-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-events-api-openapi.yml
- filename: clusters-names-api-openapi.yml
  format: yaml
  label: Clusters Names API
  slug: clusters-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-names-api-openapi.yml
- filename: clusters-registration-api-openapi.yml
  format: yaml
  label: Clusters Registration API
  slug: clusters-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-registration-api-openapi.yml
consequence_counts:
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clusters Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Clusters exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clusters
provider_slug: clusters
slug: clusters-agentic-access
source_filename: clusters-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/clusters-v1-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 7\n    acting: 7\n  by_consequence:\n    read: 7\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/message\n  method: get\n  operationId: getSigningMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/token\n  method: post\n  operationId: createAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /names/address/{address}\n  method: get\n  operationId: getNameByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /names/owner/address/{address}\n  method: get\n  operationId: getNamesByOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /names\n  method: post\n  operationId: getAddressesByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /names/register/check\n  method: post\n  operationId: checkNameAvailability\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /names/register/evm\n  method: post\n  operationId: getRegistrationDataEvm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /names/register/solana\n  method: post\n  operationId: getRegistrationDataSolana\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /names/community/{communityName}/check/{name}\n\
  \  method: get\n  operationId: checkCommunityNameAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /names/community/{communityName}/register\n  method: post\n  operationId: registerCommunityName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters\n  method: post\n  operationId: createCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/id/{id}\n  method: get\n  operationId: getClusterById\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/name/{name}\n  method: get\n  operationId: getClusterByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/agentic-access/clusters-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Company
- Infrastructure
- Identity
- Naming
- Blockchain
- Web3
- Wallet
- Multichain
- Resolver
---
