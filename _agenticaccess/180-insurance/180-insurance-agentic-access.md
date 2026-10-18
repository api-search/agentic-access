---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 13
api_specs:
- filename: 180-insurance-cota-es-api-openapi.yml
  format: yaml
  label: 180 Insurance Cotações API
  slug: 180-insurance-cota-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-cota-es-api-openapi.yml
- filename: 180-insurance-produtos-api-openapi.yml
  format: yaml
  label: 180 Insurance Produtos API
  slug: 180-insurance-produtos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-produtos-api-openapi.yml
- filename: 180-insurance-propostas-api-openapi.yml
  format: yaml
  label: 180 Insurance Propostas API
  slug: 180-insurance-propostas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-propostas-api-openapi.yml
- filename: 180-insurance-renova-es-api-openapi.yml
  format: yaml
  label: 180 Insurance Renovações API
  slug: 180-insurance-renova-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-renova-es-api-openapi.yml
- filename: 180-insurance-sinistros-api-openapi.yml
  format: yaml
  label: 180 Insurance Sinistros API
  slug: 180-insurance-sinistros-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-sinistros-api-openapi.yml
- filename: 180-insurance-vendas-api-openapi.yml
  format: yaml
  label: 180 Insurance Vendas API
  slug: 180-insurance-vendas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-vendas-api-openapi.yml
- filename: 180-insurance-webhooks-api-openapi.yml
  format: yaml
  label: 180 Insurance Webhooks API
  slug: 180-insurance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-webhooks-api-openapi.yml
consequence_counts:
  read: 13
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 180 Insurance Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: '180 Insurance exposes 33 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 180 Insurance
provider_slug: 180-insurance
slug: 180-insurance-agentic-access
source_filename: 180-insurance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/180-insurance-sagas-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 13\n    acting: 20\n  by_consequence:\n    read: 13\n    write: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /sagas/v1/boleto/{payment-intent-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/combos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/cotacoes\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/cotacoes/{id-cotacao}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/documentos/propostas/{id-proposta}/produtos/{id-produto}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/documentos/vendas/{id-venda}/produtos/{id-produto}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/obter-venda\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/propostas\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/propostas/{id-proposta}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/propostas/{id-proposta}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/propostas/{id-proposta}/cliente-segurado\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/propostas/{id-proposta}/reenviar-comunicacao/{comunicacao}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/propostas/{id-proposta}/solicitar-cancelamento\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/renovacoes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/renovacoes/{id-renovacao}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/renovacoes/{id-renovacao}/iniciar\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/sinistros/whitelabel/gerar-url\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/sinistros/{numero-sinistro}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/sinistros/{numero-sinistro}/dados-pagamento\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/sinistros/{numero-sinistro}/documentos/{file-id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/sinistros/{numero-sinistro}/documentos/{file-id}/download-url\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/sinistros/{numero-sinistro}/enviar-documento\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/sinistros/{numero-sinistro}/saldo-devedor\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /sagas/v1/vendas\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/vendas/{id-venda}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/vendas/{id-venda}/abrir-sinistro\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/vendas/{id-venda}/alteracoes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/vendas/{id-venda}/solicitar-cancelamento\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/webhooks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sagas/v1/webhooks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/webhooks/{id-webhook}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/webhooks/{id-webhook}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sagas/v1/webhooks/{id-webhook}/rotacionar-chave-hmac\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/agentic-access/180-insurance-agentic-access.yml
summary_line: 33 operations · 20 acting
tags:
- Company
- Insurtech
- Insurance
- Embedded Insurance
- Brazil
- Fintech
- Webhook
---
