---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 3
api_specs:
- filename: socure-idplus-api-openapi.yml
  format: yaml
  label: Socure ID+ API
  slug: socure-idplus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-idplus-api-openapi.yml
- filename: socure-docv-api-openapi.yml
  format: yaml
  label: Socure Predictive DocV API
  slug: socure-docv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-docv-api-openapi.yml
- filename: socure-watchlist-monitoring-api-openapi.yml
  format: yaml
  label: Socure Global Watchlist Monitoring API
  slug: socure-watchlist-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-watchlist-monitoring-api-openapi.yml
- filename: socure-decision-api-openapi.yml
  format: yaml
  label: Socure Decision API
  slug: socure-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-decision-api-openapi.yml
- filename: socure-account-intelligence-api-openapi.yml
  format: yaml
  label: Socure Account Intelligence API
  slug: socure-account-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-account-intelligence-api-openapi.yml
consequence_counts:
  read: 3
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Socure Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'socure exposes 12 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: socure
provider_slug: socure
slug: socure-agentic-access
source_filename: socure-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/socure-account-intelligence-api-openapi.yml, openapi/socure-decision-api-openapi.yml,\n  openapi/socure-docv-api-openapi.yml, openapi/socure-idplus-api-openapi.yml, openapi/socure-watchlist-monitoring-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 9\n    connected: 3\n  by_consequence:\n    write: 9\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/3.0/EmailAuthScore\n  method: post\n  operationId: validateBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/3.0/EmailAuthScore\n  method: post\n  operationId: evaluateDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/3.0/EmailAuthScore\n  method: post\n  operationId: createDocvTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/3.0/devices/{deviceId}/documents\n  method: post\n  operationId: uploadDocvDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/3.0/documents/verify\n  method: post\n  operationId: verifyDocvDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/3.0/documents/{docvTransactionId}\n  method: get\n  operationId: getDocvTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3.0/EmailAuthScore\n  method: post\n  operationId: evaluateIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/3.0/watchlist/monitoring/profiles\n  method: post\n  operationId: enrollMonitoringProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/3.0/watchlist/monitoring/profiles/{profileId}\n  method: get\n  operationId: getMonitoringProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3.0/watchlist/monitoring/profiles/{profileId}\n  method: delete\n  operationId: removeMonitoringProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/3.0/watchlist/monitoring/alerts\n  method: get\n  operationId: listMonitoringAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/3.0/watchlist/monitoring/alerts/{alertId}\n  method: patch\n  operationId: updateMonitoringAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/agentic-access/socure-agentic-access.yml
summary_line: 12 operations · 9 acting
tags: []
---
