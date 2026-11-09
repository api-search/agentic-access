---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 12
api_specs:
- filename: boletinclaro-es-boletines-api-openapi.yml
  format: yaml
  label: Boletín Claro Boletines API
  slug: boletinclaro-es-boletines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-boletines-api-openapi.yml
- filename: boletinclaro-es-c-digos-api-openapi.yml
  format: yaml
  label: Boletín Claro Códigos API
  slug: boletinclaro-es-c-digos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-c-digos-api-openapi.yml
- filename: boletinclaro-es-dinero-p-blico-api-openapi.yml
  format: yaml
  label: Boletín Claro Dinero público API
  slug: boletinclaro-es-dinero-p-blico-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-dinero-p-blico-api-openapi.yml
- filename: boletinclaro-es-empresas-api-openapi.yml
  format: yaml
  label: Boletín Claro Empresas API
  slug: boletinclaro-es-empresas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-empresas-api-openapi.yml
- filename: boletinclaro-es-referencia-api-openapi.yml
  format: yaml
  label: Boletín Claro Referencia API
  slug: boletinclaro-es-referencia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-referencia-api-openapi.yml
consequence_counts:
  read: 12
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Boletinclaro Es Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Boletín Claro exposes 15 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Boletín Claro
provider_slug: boletinclaro-es
slug: boletinclaro-es-agentic-access
source_filename: boletinclaro-es-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/boletinclaro-es-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 12\n    acting: 3\n  by_consequence:\n    read: 12\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: referencia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/redoc-2.5.4.js\n  method: get\n  operationId: referenciaScript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boletines\n  method: get\n  operationId:\
  \ buscarBoletines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boletines\n  method: post\n  operationId: buscarBoletinesJSON\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /codigos\n  method: get\n  operationId: buscarCodigos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codigos\n  method: post\n  operationId: buscarCodigosJSON\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /empresas\n  method: get\n  operationId: buscarEmpresas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /empresas/{nif}\n  method: get\n  operationId: perfilEmpresa\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /errores\n  method: get\n  operationId: catalogoDeErrores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /errores/{codigo}\n  method: get\n  operationId: detalleDeError\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licitaciones\n  method: get\n  operationId: licitacionesPorCPV\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: especificacion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oportunidades\n  method: get\n  operationId: buscarOportunidades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oportunidades\n  method: post\n  operationId: buscarOportunidadesJSON\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referencia\n  method: get\n  operationId: referenciaInteractiva\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/boletinclaro-es/agentic-access/boletinclaro-es-agentic-access.yml
summary_line: 15 operations · 3 acting
tags:
- Company
- Software-as-a-Service
- Alerts
- Spain
- Government
---
