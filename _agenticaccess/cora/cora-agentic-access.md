---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 11
api_specs:
- filename: cora-balance-api-openapi.yml
  format: yaml
  label: Cora Balance API
  slug: cora-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-balance-api-openapi.yml
- filename: cora-banks-api-openapi.yml
  format: yaml
  label: Cora Banks API
  slug: cora-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-banks-api-openapi.yml
- filename: cora-boletos-v2-api-openapi.yml
  format: yaml
  label: Cora Boletos V2 API
  slug: cora-boletos-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-boletos-v2-api-openapi.yml
- filename: cora-businesses-api-openapi.yml
  format: yaml
  label: Cora Businesses API
  slug: cora-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-businesses-api-openapi.yml
- filename: cora-credentials-api-openapi.yml
  format: yaml
  label: Cora Credentials API
  slug: cora-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-credentials-api-openapi.yml
- filename: cora-dados-de-conta-api-openapi.yml
  format: yaml
  label: Cora Dados De Conta API
  slug: cora-dados-de-conta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-dados-de-conta-api-openapi.yml
- filename: cora-initiate-api-openapi.yml
  format: yaml
  label: Cora Initiate API
  slug: cora-initiate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-initiate-api-openapi.yml
- filename: cora-issuer-api-openapi.yml
  format: yaml
  label: Cora Issuer API
  slug: cora-issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-issuer-api-openapi.yml
- filename: cora-notifica-es-api-openapi.yml
  format: yaml
  label: Cora Notificações API
  slug: cora-notifica-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-notifica-es-api-openapi.yml
- filename: cora-notifications-api-openapi.yml
  format: yaml
  label: Cora Notifications API
  slug: cora-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-notifications-api-openapi.yml
- filename: cora-pagamento-de-impostos-api-openapi.yml
  format: yaml
  label: Cora Pagamento De Impostos API
  slug: cora-pagamento-de-impostos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-pagamento-de-impostos-api-openapi.yml
- filename: cora-pay-api-openapi.yml
  format: yaml
  label: Cora Pay API
  slug: cora-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-pay-api-openapi.yml
- filename: cora-service-receipt-api-openapi.yml
  format: yaml
  label: Cora Service Receipt API
  slug: cora-service-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-service-receipt-api-openapi.yml
- filename: cora-statement-api-openapi.yml
  format: yaml
  label: Cora Statement API
  slug: cora-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-statement-api-openapi.yml
consequence_counts:
  physical: 3
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cora Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /initiate/{payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{invoice_id}/notifications
operation_count: 20
overview: 'Cora exposes 20 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 6 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cora
provider_slug: cora
slug: cora-agentic-access
source_filename: cora-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/cora-base-openapi.yml, openapi/cora-boletos-openapi.yml, openapi/cora-boletos-v2-openapi.yml,\n  openapi/cora-dados-de-conta-openapi.yml, openapi/cora-extrato-openapi.yml, openapi/cora-nota-fiscal-de-servi-o-openapi.yml,\n  openapi/cora-notifica-es-openapi.yml, openapi/cora-pagamento-de-impostos-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 11\n    acting: 9\n  by_consequence:\n    read: 11\n    write: 6\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /banks\n  method: get\n  operationId: lista-de-bancos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /pay\n  method: post\n  operationId: pagar-boleto-em-stage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: consultar-boletos-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: emissão-de-boleto-registrado-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: //\n  method: post\n  operationId: qr-code-pix-v2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{invoice_id}\n  method: get\n  operationId: consultar-detalhes-de-um-boleto-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{invoice_id}\n  method: delete\n  operationId: cancelamento-de-boleto-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{invoice_id}/notifications\n  method: delete\n  operationId: cancelamento-de-boleto-copy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: dados-de-conta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance\n  method: get\n  operationId: saldo-de-conta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statement\n  method: get\n  operationId: consulta-de-extrato\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/check-availability\n\
  \  method: get\n  operationId: disponibilidade-da-nota-fiscal-por-cliente\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/cnaes\n  method: get\n  operationId: consulta-de-cnae\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/service-codes\n  method: get\n  operationId: consulta-de-codigo-de-servico\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials\n  method: post\n  operationId: upload-certificado-a1-e-credenciais-nfse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /issuer\n  method: post\n  operationId: cadastro-do-emissor-de-nota-fiscal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service-receipt/{service_receipt_id}\n  method: delete\n  operationId: cancelamento-de-nfse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: lista-de-endpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /\n  method: get\n  operationId: lista-de-pagamentos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /initiate/{payment_id}\n  method: delete\n  operationId: cancelamento-de-pagamento\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/agentic-access/cora-agentic-access.yml
summary_line: 20 operations · 9 acting
tags:
- Company
- Banking
- Brazil
- Payments
- Pix
- Boleto
- Invoicing
- Small Business
- Fintech
- Banking as a Service
---
