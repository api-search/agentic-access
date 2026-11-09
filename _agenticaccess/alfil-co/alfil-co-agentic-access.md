---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: alfil-co-b-squeda-api-openapi.yml
  format: yaml
  label: Alfil Búsqueda API
  slug: alfil-co-b-squeda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alfil-co/openapi/alfil-co-b-squeda-api-openapi.yml
- filename: alfil-co-congreso-api-openapi.yml
  format: yaml
  label: Alfil Congreso API
  slug: alfil-co-congreso-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alfil-co/openapi/alfil-co-congreso-api-openapi.yml
- filename: alfil-co-contrataci-n-api-openapi.yml
  format: yaml
  label: Alfil Contratación API
  slug: alfil-co-contrataci-n-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alfil-co/openapi/alfil-co-contrataci-n-api-openapi.yml
- filename: alfil-co-electoral-api-openapi.yml
  format: yaml
  label: Alfil Electoral API
  slug: alfil-co-electoral-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alfil-co/openapi/alfil-co-electoral-api-openapi.yml
- filename: alfil-co-finanzas-api-openapi.yml
  format: yaml
  label: Alfil Finanzas API
  slug: alfil-co-finanzas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alfil-co/openapi/alfil-co-finanzas-api-openapi.yml
- filename: alfil-co-geograf-as-api-openapi.yml
  format: yaml
  label: Alfil Geografías API
  slug: alfil-co-geograf-as-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alfil-co/openapi/alfil-co-geograf-as-api-openapi.yml
- filename: alfil-co-partidos-api-openapi.yml
  format: yaml
  label: Alfil Partidos API
  slug: alfil-co-partidos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alfil-co/openapi/alfil-co-partidos-api-openapi.yml
- filename: alfil-co-pol-ticos-api-openapi.yml
  format: yaml
  label: Alfil Políticos API
  slug: alfil-co-pol-ticos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alfil-co/openapi/alfil-co-pol-ticos-api-openapi.yml
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Alfil Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Alfil exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Alfil
provider_slug: alfil-co
slug: alfil-co-agentic-access
source_filename: alfil-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/alfil-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/buscar\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/geografias\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/contratos\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/contratos/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/contratacion/procesos/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/contratos/{id}/adiciones\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/electoral/resultados\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n    scope:\n    - buscar:read\n- path: /v1/electoral/desglose\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/electoral/puestos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/electoral/censo\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/politicos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/politicos/{slug}\n  method: get\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/partidos/{slug}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/congreso/actividad\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/congreso/votaciones\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/congreso/votaciones/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/congreso/proyectos/{slug}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/congreso/congresistas/{slug}/votos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n- path: /v1/finanzas/territoriales\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - buscar:read\n"
source_yaml_url: https://artifacts.apis.io/alfil-co/agentic-access/alfil-co-agentic-access.yml
summary_line: 19 operations
tags:
- Politics
- Colombia
- Elections
- Public Procurement
- Data Analysis
- Intelligence
---
