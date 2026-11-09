---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: firmenwatch-ch-aktionen-api-openapi.yml
  format: yaml
  label: Firmenwatch Aktionen API
  slug: firmenwatch-ch-aktionen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-aktionen-api-openapi.yml
- filename: firmenwatch-ch-betrieb-api-openapi.yml
  format: yaml
  label: Firmenwatch Betrieb API
  slug: firmenwatch-ch-betrieb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-betrieb-api-openapi.yml
- filename: firmenwatch-ch-ereignisse-api-openapi.yml
  format: yaml
  label: Firmenwatch Ereignisse API
  slug: firmenwatch-ch-ereignisse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-ereignisse-api-openapi.yml
- filename: firmenwatch-ch-firmen-api-openapi.yml
  format: yaml
  label: Firmenwatch Firmen API
  slug: firmenwatch-ch-firmen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-firmen-api-openapi.yml
- filename: firmenwatch-ch-identitaet-api-openapi.yml
  format: yaml
  label: Firmenwatch Identitaet API
  slug: firmenwatch-ch-identitaet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-identitaet-api-openapi.yml
- filename: firmenwatch-ch-portfolios-api-openapi.yml
  format: yaml
  label: Firmenwatch Portfolios API
  slug: firmenwatch-ch-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-portfolios-api-openapi.yml
- filename: firmenwatch-ch-uid-api-openapi.yml
  format: yaml
  label: Firmenwatch UID API
  slug: firmenwatch-ch-uid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-uid-api-openapi.yml
consequence_counts:
  read: 9
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Firmenwatch Ch Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Firmenwatch exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Firmenwatch
provider_slug: firmenwatch-ch
slug: firmenwatch-ch-agentic-access
source_filename: firmenwatch-ch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/firmenwatch-ch-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 9\n    acting: 7\n  by_consequence:\n    read: 9\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /uid/{uid}.json\n  method: get\n  operationId: resolveCompanyIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{uid}\n  method:\
  \ get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{uid}/officers\n  method: get\n  operationId: listCompanyOfficers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{uid}/events\n  method: get\n  operationId: listCompanyEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/checkpoint\n  method: get\n  operationId: getEventCheckpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/match\n  method: post\n  operationId: matchCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/reconcile\n  method: post\n  operationId: reconcileCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolios/{sourceKey}/syncs\n  method: post\n  operationId: startPortfolioSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolios/{sourceKey}/syncs/{syncId}/items\n  method: put\n  operationId: stagePortfolioSyncItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolios/{sourceKey}/syncs/{syncId}/commit\n  method: post\n  operationId: commitPortfolioSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions\n  method: get\n  operationId: listActions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{id}\n  method: patch\n  operationId: updateAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uid/validate\n  method: post\n  operationId: validateUid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://artifacts.apis.io/firmenwatch-ch/agentic-access/firmenwatch-ch-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- Swiss
- Monitoring
- Commercial-Register
- Alerts
- Business-Intelligence
---
