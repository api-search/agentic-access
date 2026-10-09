---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 11
api_specs:
- filename: logius-announce-api-openapi.yml
  format: yaml
  label: Logius Announce API
  slug: logius-announce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-announce-api-openapi.yml
- filename: logius-contracts-api-openapi.yml
  format: yaml
  label: Logius Contracts API
  slug: logius-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-contracts-api-openapi.yml
- filename: logius-domains-api-openapi.yml
  format: yaml
  label: Logius Domains API
  slug: logius-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-domains-api-openapi.yml
- filename: logius-events-api-openapi.yml
  format: yaml
  label: Logius Events API
  slug: logius-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-events-api-openapi.yml
- filename: logius-manager-api-openapi.yml
  format: yaml
  label: Logius Manager API
  slug: logius-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-manager-api-openapi.yml
- filename: logius-peers-api-openapi.yml
  format: yaml
  label: Logius Peers API
  slug: logius-peers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-peers-api-openapi.yml
- filename: logius-services-api-openapi.yml
  format: yaml
  label: Logius Services API
  slug: logius-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-services-api-openapi.yml
- filename: logius-subscriptions-api-openapi.yml
  format: yaml
  label: Logius Subscriptions API
  slug: logius-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-subscriptions-api-openapi.yml
- filename: logius-terugmelding-api-openapi.yml
  format: yaml
  label: Logius Terugmelding API
  slug: logius-terugmelding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-terugmelding-api-openapi.yml
- filename: logius-terugmeldingstatus-api-openapi.yml
  format: yaml
  label: Logius Terugmelding Status API
  slug: logius-terugmeldingstatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-terugmeldingstatus-api-openapi.yml
- filename: logius-token-api-openapi.yml
  format: yaml
  label: Logius Token API
  slug: logius-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-token-api-openapi.yml
- filename: logius-well-known-api-openapi.yml
  format: yaml
  label: Logius .well Known API
  slug: logius-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-well-known-api-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Logius Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /contracts/{hash}/revoke
operation_count: 24
overview: 'Logius exposes 24 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 12 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Logius
provider_slug: logius
slug: logius-agentic-access
source_filename: logius-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/logius-fsc-manager-openapi.yml, openapi/logius-notificatieservices-openapi.yml,\n  openapi/logius-terugmelding-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 13\n    connected: 11\n  by_consequence:\n    write: 12\n    read: 11\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /announce\n  method: put\n  operationId: announce\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /contracts\n  method: post\n  operationId: submitContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{hash}/accept\n  method: put\n  operationId: acceptContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{hash}/reject\n  method: put\n  operationId: rejectContract\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{hash}/revoke\n  method: put\n  operationId: revokeContract\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /token\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /peer\n  method: get\n  operationId:\
  \ getPeerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /peers\n  method: get\n  operationId: getPeers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: get\n  operationId: getServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/jwks.json\n  method: get\n  operationId: getJSONWebKeySet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: post\n  operationId: events_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - events.publish\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains\n  method: get\n  operationId: domains_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - (events.publish | events.consume)\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: post\n  operationId: domains_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - events.publish\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{uuid}\n  method: get\n  operationId: domains_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - (events.publish\
  \ | events.consume)\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: subscriptions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - (events.publish | events.consume)\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: subscriptions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - events.consume\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{uuid}\n  method: get\n  operationId: subscription_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - (events.publish | events.consume)\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /subscriptions/{uuid}\n  method: put\n  operationId: subscription_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - events.consume\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{uuid}\n  method: patch\n  operationId: subscription_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - events.consume\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{uuid}\n  method: delete\n  operationId: subscription_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - events.consume\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terugmelding\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /terugmelding\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terugmeldingStatus\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/agentic-access/logius-agentic-access.yml
summary_line: 24 operations · 13 acting · 1 human-in-the-loop
tags:
- Company
- Government
- Netherlands
- API Standards
- API Design Rules
- Digital Identity
- Data Exchange
- Public Sector
---
