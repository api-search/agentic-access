---
acting_count: 0
action_class_counts:
  connected: 33
api_specs:
- filename: balancos-ai-bcb-api-openapi.yml
  format: yaml
  label: Balanços.AI BCB API
  slug: balancos-ai-bcb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/balancos-ai/openapi/balancos-ai-bcb-api-openapi.yml
- filename: balancos-ai-cvm-api-openapi.yml
  format: yaml
  label: Balanços.AI CVM API
  slug: balancos-ai-cvm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/balancos-ai/openapi/balancos-ai-cvm-api-openapi.yml
- filename: balancos-ai-empresas-api-openapi.yml
  format: yaml
  label: Balanços.AI Empresas API
  slug: balancos-ai-empresas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/balancos-ai/openapi/balancos-ai-empresas-api-openapi.yml
consequence_counts:
  read: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Balancos Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'Balanços.AI exposes 33 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Balanços.AI
provider_slug: balancos-ai
slug: balancos-ai-agentic-access
source_filename: balancos-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/balancos-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 33\n  by_consequence:\n    read: 33\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/empresas\n  method: get\n  operationId: buscar_v1_empresas_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/empresas/{chave}\n  method: get\n  operationId: ficha_v1_empresas__chave__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/empresas/{chave}/balancos\n\
  \  method: get\n  operationId: balancos_v1_empresas__chave__balancos_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/empresas/{chave}/dres\n  method: get\n  operationId: dres_v1_empresas__chave__dres_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/empresas/{chave}/documentos\n  method: get\n  operationId: documentos_v1_empresas__chave__documentos_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ranking\n  method: get\n  operationId: ranking_v1_ranking_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/companhias\n  method: get\n  operationId:\
  \ catalogo_v1_cvm_companhias_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/companhias/{chave}\n  method: get\n  operationId: ficha_v1_cvm_companhias__chave__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/companhias/{chave}/dfps\n  method: get\n  operationId: dfps_v1_cvm_companhias__chave__dfps_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/companhias/{chave}/balancos\n  method: get\n  operationId: balancos_v1_cvm_companhias__chave__balancos_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/companhias/{chave}/dres\n \
  \ method: get\n  operationId: dres_v1_cvm_companhias__chave__dres_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/dfps/{id_doc}\n  method: get\n  operationId: entrega_v1_cvm_dfps__id_doc__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/dfps/{id_doc}/demonstracoes\n  method: get\n  operationId: demonstracoes_v1_cvm_dfps__id_doc__demonstracoes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/dfps/{id_doc}/demonstracoes/{demonstracao}\n  method: get\n  operationId: demonstracao_v1_cvm_dfps__id_doc__demonstracoes__demonstracao__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/dfps/{id_doc}/parecer\n  method: get\n  operationId: parecer_v1_cvm_dfps__id_doc__parecer_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/companhias/{chave}/itrs\n  method: get\n  operationId: itrs_v1_cvm_companhias__chave__itrs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/itrs/{id_doc}\n  method: get\n  operationId: entrega_itr_v1_cvm_itrs__id_doc__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/itrs/{id_doc}/demonstracoes\n  method: get\n  operationId: demonstracoes_itr_v1_cvm_itrs__id_doc__demonstracoes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/itrs/{id_doc}/demonstracoes/{demonstracao}\n  method: get\n  operationId: demonstracao_itr_v1_cvm_itrs__id_doc__demonstracoes__demonstracao__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/itrs/{id_doc}/parecer\n  method: get\n  operationId: parecer_itr_v1_cvm_itrs__id_doc__parecer_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/companhias/{chave}/trimestres\n  method: get\n  operationId: trimestres_v1_cvm_companhias__chave__trimestres_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/companhias/{chave}/resultados\n  method: get\n  operationId: resultados_v1_cvm_companhias__chave__resultados_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/ranking-12m\n  method: get\n  operationId: ranking_12m_v1_cvm_ranking_12m_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cvm/ranking\n  method: get\n  operationId: ranking_v1_cvm_ranking_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bcb/instituicoes\n  method: get\n  operationId: catalogo_v1_bcb_instituicoes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bcb/instituicoes/{chave}\n  method: get\n  operationId: ficha_v1_bcb_instituicoes__chave__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bcb/instituicoes/{chave}/trimestres\n  method: get\n  operationId: trimestres_v1_bcb_instituicoes__chave__trimestres_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bcb/instituicoes/{chave}/resultados\n  method: get\n  operationId: resultados_v1_bcb_instituicoes__chave__resultados_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bcb/instituicoes/{chave}/relatorios\n  method: get\n  operationId: relatorios_v1_bcb_instituicoes__chave__relatorios_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bcb/conglomerados/{codinst}\n  method:\
  \ get\n  operationId: conglomerado_v1_bcb_conglomerados__codinst__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bcb/data-bases\n  method: get\n  operationId: data_bases_v1_bcb_data_bases_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bcb/data-bases/{data_base}/relatorios\n  method: get\n  operationId: estrutura_v1_bcb_data_bases__data_base__relatorios_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bcb/ranking\n  method: get\n  operationId: ranking_v1_bcb_ranking_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/balancos-ai/agentic-access/balancos-ai-agentic-access.yml
summary_line: 33 operations
tags:
- Finance
- Brazil
- Public Data
- Financial Statements
---
