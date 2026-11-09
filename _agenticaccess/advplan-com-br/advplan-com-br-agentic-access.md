---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 13
api_specs:
- filename: advplan-com-br-casos-api-openapi.yml
  format: yaml
  label: AdvPlan Casos API
  slug: advplan-com-br-casos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/advplan-com-br/openapi/advplan-com-br-casos-api-openapi.yml
- filename: advplan-com-br-clientes-api-openapi.yml
  format: yaml
  label: AdvPlan Clientes API
  slug: advplan-com-br-clientes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/advplan-com-br/openapi/advplan-com-br-clientes-api-openapi.yml
- filename: advplan-com-br-cobran-as-api-openapi.yml
  format: yaml
  label: AdvPlan Cobranças API
  slug: advplan-com-br-cobran-as-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/advplan-com-br/openapi/advplan-com-br-cobran-as-api-openapi.yml
- filename: advplan-com-br-documentos-api-openapi.yml
  format: yaml
  label: AdvPlan Documentos API
  slug: advplan-com-br-documentos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/advplan-com-br/openapi/advplan-com-br-documentos-api-openapi.yml
- filename: advplan-com-br-prazos-api-openapi.yml
  format: yaml
  label: AdvPlan Prazos API
  slug: advplan-com-br-prazos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/advplan-com-br/openapi/advplan-com-br-prazos-api-openapi.yml
consequence_counts:
  read: 13
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Advplan Com Br Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'AdvPlan exposes 30 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AdvPlan
provider_slug: advplan-com-br
slug: advplan-com-br-agentic-access
source_filename: advplan-com-br-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/advplan-com-br-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 13\n    acting: 17\n  by_consequence:\n    read: 13\n    write: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/casos\n  method: get\n  operationId: 5917df8dbf0d67429c2b113fb1a4aeae\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/casos\n  method: post\n  operationId: e5cb3127589d3effbe4a433172d1a49c\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/casos/{caso}\n  method: get\n  operationId: b654c19efdbbea17a84ec5f5cdb9b0bb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/casos/{caso}\n  method: put\n  operationId: f01f4d6730f29704ab72fdc4ce3a4b67\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/casos/{caso}\n  method: delete\n  operationId: d655c1028d1f4673876ac2c948b0189c\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/casos/{caso}/timeline\n  method: get\n  operationId: 817b4ed7e52a4260d64c8b50768e651e\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/casos/{caso}/eventos\n  method: post\n  operationId: 54c4c144696616dc56726b419519836f\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/casos/{caso}/fase\n  method: put\n  operationId: b20f323615171a3e2bfe3a46778e5605\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/casos/{caso}/encerrar\n  method: post\n  operationId: be76a9fc07803204178877b9bd74feed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/clientes\n  method: get\n  operationId: 275ddabe0ff3df657edd035747f2c43a\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/clientes\n  method: post\n  operationId: d82cb60437b288da7843df7826fad22f\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/clientes/{cliente}\n  method: get\n  operationId: ab4ce3009d7508c93f86a31ca7afca31\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/clientes/{cliente}\n  method: put\n  operationId: d73c1716e55d5b6be632db863d3fda4d\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/clientes/{cliente}\n  method: delete\n  operationId: 49710823fcda170cb253efe37c6339e6\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cobrancas\n  method: get\n  operationId: 552fc16dadd5f03ca13480f709184115\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cobrancas\n  method: post\n  operationId: c9d3b23f1be9e1c18be00cbf370924a4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cobrancas/{cobranca}\n  method: get\n  operationId: 39a27b5209516b0d7f0cbf09afa9d9c9\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documentos\n  method: get\n  operationId:\
  \ e5ee7c2cf84a8db11aa3fd0a29f7478b\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documentos/{documento}\n  method: get\n  operationId: 6c95ba4002cd987c31604a992599a692\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documentos/{documento}\n  method: delete\n  operationId: afaff6fa23120f8930ca927a97956196\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documentos/gerar\n  method: post\n  operationId: b2aa5a339646c062782766b34ae44b49\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documentos/{documento}/download\n  method: get\n  operationId: 6003682a7de69cd7478995395a2e1fbb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documentos/{documento}/texto\n  method: get\n  operationId: 1cf2d545c8af4fc87f214c4468fe5d5b\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prazos\n  method: get\n  operationId: bbda8e49a80eeece3d6458d60806f183\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prazos\n  method: post\n  operationId: cce845963350b7ec55c8ad2d82372b24\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/prazos/{prazo}\n  method: get\n  operationId: bc11f1be27698de34a485b969a4727f7\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prazos/{prazo}/aprovar\n  method: put\n  operationId: 32085bd2abfb03085faece4841e43fdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/prazos/{prazo}/rejeitar\n  method: put\n  operationId: 2997e28034fb784e8739bf26fc673665\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/prazos/{prazo}/protocolar\n  method: put\n  operationId: 4901c7c61941bc8e4288bdd6b25ca29e\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/prazos/{prazo}/cancelar\n  method: put\n  operationId: 8a41ea60b1ba2dfd881ad78bbfe4ab0c\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/advplan-com-br/agentic-access/advplan-com-br-agentic-access.yml
summary_line: 30 operations · 17 acting
tags:
- Legal Tech
- Artificial Intelligence
- Software
- Brazil
- LawPractice
---
