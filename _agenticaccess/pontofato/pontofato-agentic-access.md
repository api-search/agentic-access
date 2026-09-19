---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 15
api_specs:
- filename: pontofato-apis-json-api-openapi.yml
  format: yaml
  label: PontoFato Apis.json API
  slug: pontofato-apis-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-apis-json-api-openapi.yml
- filename: pontofato-buscar-api-openapi.yml
  format: yaml
  label: PontoFato Buscar API
  slug: pontofato-buscar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-buscar-api-openapi.yml
- filename: pontofato-cep-api-openapi.yml
  format: yaml
  label: PontoFato Cep API
  slug: pontofato-cep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-cep-api-openapi.yml
- filename: pontofato-contact-api-openapi.yml
  format: yaml
  label: PontoFato Contact API
  slug: pontofato-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-contact-api-openapi.yml
- filename: pontofato-credito-api-openapi.yml
  format: yaml
  label: PontoFato Credito API
  slug: pontofato-credito-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-credito-api-openapi.yml
- filename: pontofato-empresas-api-openapi.yml
  format: yaml
  label: PontoFato Empresas API
  slug: pontofato-empresas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-empresas-api-openapi.yml
- filename: pontofato-health-api-openapi.yml
  format: yaml
  label: PontoFato Health API
  slug: pontofato-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-health-api-openapi.yml
- filename: pontofato-local-api-openapi.yml
  format: yaml
  label: PontoFato Local API
  slug: pontofato-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-local-api-openapi.yml
- filename: pontofato-mcp-api-openapi.yml
  format: yaml
  label: PontoFato MCP API
  slug: pontofato-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-mcp-api-openapi.yml
- filename: pontofato-metrics-api-openapi.yml
  format: yaml
  label: PontoFato Metrics API
  slug: pontofato-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-metrics-api-openapi.yml
- filename: pontofato-okf-api-openapi.yml
  format: yaml
  label: PontoFato Okf API
  slug: pontofato-okf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-okf-api-openapi.yml
- filename: pontofato-pontofato-api-openapi.yml
  format: yaml
  label: PontoFato Ponto Fato API
  slug: pontofato-pontofato-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-pontofato-api-openapi.yml
- filename: pontofato-proximo-api-openapi.yml
  format: yaml
  label: PontoFato Proximo API
  slug: pontofato-proximo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-proximo-api-openapi.yml
- filename: pontofato-raio-api-openapi.yml
  format: yaml
  label: PontoFato Raio API
  slug: pontofato-raio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-raio-api-openapi.yml
- filename: pontofato-vizinhanca-api-openapi.yml
  format: yaml
  label: PontoFato Vizinhanca API
  slug: pontofato-vizinhanca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-vizinhanca-api-openapi.yml
- filename: pontofato-well-known-api-openapi.yml
  format: yaml
  label: PontoFato .well Known API
  slug: pontofato-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-well-known-api-openapi.yml
consequence_counts:
  read: 15
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pontofato Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'PontoFato exposes 18 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PontoFato
provider_slug: pontofato
slug: pontofato-agentic-access
source_filename: pontofato-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: generated\nsource: openapi/pontofato-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 15\n    acting: 3\n  by_consequence:\n    read: 15\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /okf/{arquivo}\n  method: get\n  operationId: get_okf_by_arquivo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/{arquivo}\n  method: get\n  operationId: get_well_known_by_arquivo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /apis.json\n  method: get\n  operationId: get_apis_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/\n  method: get\n  operationId: api_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: post_mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cep/{cep}\n  method: get\n  operationId: cep\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cep/{cep}/unidades\n  method: get\n  operationId: unidades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/proximo\n  method: get\n  operationId: proximo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/buscar\n  method: get\n  operationId: buscar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/empresas\n  method: get\n  operationId: empresas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/raio\n\
  \  method: get\n  operationId: raio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vizinhanca\n  method: get\n  operationId: vizinhanca\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/local\n  method: get\n  operationId: get_api_local\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/contact\n  method: post\n  operationId: contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/metrics\n  method: get\n  operationId: get_api_metrics\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/credito\n  method: post\n  operationId: post_api_credito\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/credito\n  method: get\n  operationId: get_api_credito\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/agentic-access/pontofato-agentic-access.yml
summary_line: 18 operations · 3 acting
tags:
- Brazilian CEP
- address geocoding
- IBGE CNEFE
- Geospatial
- latitude/longitude
- CNPJ
- Receita Federal
- Business Registry
- Location Intelligence
- proximity search
- radius search
- Open Government Data
- agent-native
- MCP
- x402-micropayments
---
