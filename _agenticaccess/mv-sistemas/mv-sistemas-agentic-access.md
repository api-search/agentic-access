---
acting_count: 40
action_class_counts:
  acting: 40
  connected: 39
api_specs:
- filename: mv-sistemas-clinic-agenda-openapi.yaml
  format: yaml
  label: Clinic Agenda
  slug: clinic-agenda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-agenda-openapi.yaml
- filename: mv-sistemas-clinic-connect-attendance-openapi.yaml
  format: yaml
  label: 'Clinic Connect : Atendimento'
  slug: clinic-connect-atendimento
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-connect-attendance-openapi.yaml
- filename: mv-sistemas-clinic-connect-openapi.yaml
  format: yaml
  label: Clinic Connect
  slug: clinic-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-connect-openapi.yaml
- filename: mv-sistemas-clinic-connect-performance-schedule-openapi.yml
  format: yaml
  label: Clinic Connect - Agendamento de performance API
  slug: clinic-connect-agendamento-de-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-connect-performance-schedule-openapi.yml
- filename: mv-sistemas-clinic-patient-audit-openapi.yaml
  format: yaml
  label: 'Clinic : Auditoria de dados de saúde do paciente'
  slug: clinic-auditoria-de-dados-de-saúde-do-paciente
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-clinic-patient-audit-openapi.yaml
- filename: mv-sistemas-events-openapi.json
  format: json
  label: API para Gestão de Eventos
  slug: api-para-gestão-de-eventos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-events-openapi.json
- filename: mv-sistemas-face-recognition-openapi.json
  format: json
  label: Reconhecimento Facial
  slug: reconhecimento-facial
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-face-recognition-openapi.json
- filename: mv-sistemas-gestao-beneficiarios-openapi.json
  format: json
  label: Gestão de Dados Cadastrais dos Beneficiários
  slug: gestão-de-dados-cadastrais-dos-beneficiários
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-gestao-beneficiarios-openapi.json
- filename: mv-sistemas-hub-operadora-openapi.yaml
  format: yaml
  label: Integração Hub Operadora
  slug: integração-hub-operadora
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-hub-operadora-openapi.yaml
- filename: mv-sistemas-news-openapi.json
  format: json
  label: News - Global Health
  slug: news-global-health
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-news-openapi.json
- filename: mv-sistemas-pendencias-saude-openapi.json
  format: json
  label: Gestão de Pendências de Saúde
  slug: gestão-de-pendências-de-saúde
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-pendencias-saude-openapi.json
- filename: mv-sistemas-performance-schedule-webhook-openapi.yml
  format: yaml
  label: Webhook - Agendamento de performance
  slug: webhook-agendamento-de-performance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-performance-schedule-webhook-openapi.yml
- filename: mv-sistemas-personal-attendance-openapi.json
  format: json
  label: 'Personal Health : Atendimentos'
  slug: personal-health-atendimentos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-personal-attendance-openapi.json
- filename: mv-sistemas-personal-health-ficha-clinica-openapi.json
  format: json
  label: 'Personal Health : Ficha Clínica'
  slug: personal-health-ficha-clínica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-personal-health-ficha-clinica-openapi.json
- filename: mv-sistemas-protocolo-entrada-openapi.json
  format: json
  label: Protocolo de Entrada
  slug: protocolo-de-entrada
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-protocolo-entrada-openapi.json
- filename: mv-sistemas-regulacao-openapi.yaml
  format: yaml
  label: 'Clinic Connect : Regulação'
  slug: clinic-connect-regulação
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-regulacao-openapi.yaml
- filename: mv-sistemas-shared-request-openapi.yaml
  format: yaml
  label: Compartilhamento de Dados
  slug: compartilhamento-de-dados
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-shared-request-openapi.yaml
- filename: mv-sistemas-users-openapi.json
  format: json
  label: Users - Global Health
  slug: users-global-health
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/openapi/mv-sistemas-users-openapi.json
consequence_counts:
  physical: 2
  read: 39
  safety-critical: 5
  write: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Mv Sistemas Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/entry-control-protocols
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/entry-control-protocols/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/entry-control-protocols/{id}/visitor-movements
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/entry-control-protocols/{id}/visitor-movements/{visitorMovementId}/exit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /shared-request/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /news/v2/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /notification/email/send
operation_count: 79
overview: 'MV sistemas exposes 79 API operations that an AI agent could call, of which 40 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 39 read, 33 write, 2 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MV sistemas
provider_slug: mv-sistemas
slug: mv-sistemas-agentic-access
source_filename: mv-sistemas-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/mv-sistemas-clinic-agenda-openapi.yaml, openapi/mv-sistemas-clinic-connect-attendance-openapi.yaml,\n  openapi/mv-sistemas-clinic-connect-openapi.yaml, openapi/mv-sistemas-clinic-connect-performance-schedule-openapi.yml,\n  openapi/mv-sistemas-clinic-patient-audit-openapi.yaml, openapi/mv-sistemas-events-openapi.json,\n  openapi/mv-sistemas-face-recognition-openapi.json, openapi/mv-sistemas-gestao-beneficiarios-openapi.json,\n  openapi/mv-sistemas-hub-operadora-openapi.yaml, openapi/mv-sistemas-news-openapi.json, openapi/mv-sistemas-pendencias-saude-openapi.json,\n  openapi/mv-sistemas-performance-schedule-webhook-openapi.yml, openapi/mv-sistemas-personal-attendance-openapi.json,\n  openapi/mv-sistemas-personal-health-ficha-clinica-openapi.json, openapi/mv-sistemas-protocolo-entrada-openapi.json,\n  openapi/mv-sistemas-regulacao-openapi.yaml, openapi/mv-sistemas-shared-request-openapi.yaml,\n  openapi/mv-sistemas-users-openapi.json\n\
  description: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 79\n  by_action_class:\n    connected: 39\n    acting: 40\n  by_consequence:\n    read: 39\n    write: 33\n    physical: 2\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /available-appointments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/attendance\n  method: post\n  operationId: addAttendance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /v1/attendance\n  method: get\n  operationId: listAttendance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/obstetric-plans\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clinics\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/clinics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/employees\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/employees\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insurances\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/insurances\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/services\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /importations/v1/patient-data\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/performance-schedules/list\n  method: get\n  operationId: listPerformanceSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/performance-schedules/scheduling\n  method: post\n  operationId: createScheduling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/performance-schedules/scheduling/status\n  method: put\n  operationId: updateSchedulingStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/procedure-request\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clinic/v1/patient-audit-health-data\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/event\n  method: post\n  operationId: createEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /minimal\n  method: post\n  operationId: createEventWithMinimalInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /minimal/{hashKey}\n  method: put\n  operationId: updateEventWithMinimalInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/event-appointment\n  method: post\n  operationId: createEventAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/loincmv/bytuss/{tuss}\n  method: get\n  operationId: findLoincByTussCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recognition-protocol\n  method: get\n  operationId: getRecognitionProtocol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/biometric/import/start\n  method: post\n  operationId: biometricImportStartV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/biometric/import/upload\n \
  \ method: post\n  operationId: biometricImportUploadV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/biometric/import/finish/{importIdentifier}\n  method: put\n  operationId: biometricImportFinishV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/face/liveness/start\n  method: get\n  operationId: faceLivenessStartV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/face/liveness/finish\n  method:\
  \ post\n  operationId: faceLivenessFinishV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /persons\n  method: put\n  operationId: addPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /persons\n  method: get\n  operationId: findPersonByDocumentNumberOrInsuranceCardNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /persons/list\n  method: get\n  operationId: findPersonsByDocumentNumberOrInsuranceCardNumber\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetGuiaMedico/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetBeneficiario/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetCarteira/{numerocpf}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetGuias/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/Funcoes/GetDependentes/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetHistoricoCallCenter/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /GetUtilizacao\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetEstados/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetCidades/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetBairros/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetRecursos/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/GetEspecialidade/{numerocarteira}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Funcoes/PostGerarToken\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /news/v2/send\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notification/push\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notification/email/send\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health-pendency\n  method: post\n  operationId: addHealthPendency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health-pendency\n  method: get\n  operationId: findHealthPendencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health-pendency/{hash-key}\n  method: get\n  operationId: getHealthPendencyById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health-pendency/{hash-key}\n  method: put\n  operationId: updateHealthPendencyByHashKey\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health-pendency/{hash-key}/exams/{exam-source-id}\n  method: get\n  operationId: getHealthPendencyExamItemByHashKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health-pendency/{hash-key}/exams/{exam-source-id}\n  method: put\n  operationId: updateHealthPendencyExamItemByHashKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create\n  method: post\n  operationId: createPerformanceScheduleIntegration\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancel\n  method: post\n  operationId: cancelPerformanceScheduleIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attendance\n  method: get\n  operationId: byFilter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/authorizer/url/presigned\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /person/allergy\n  method: get\n  operationId: getPersonResumeV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/entry-control-protocols\n  method: post\n  operationId: createProtocol\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/entry-control-protocols/{id}\n  method: put\n  operationId: updateProtocol\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/entry-control-protocols/{id}/visitor-movements\n  method: post\n  operationId: createVisitorMovement\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/entry-control-protocols/{id}/visitor-movements/{visitorMovementId}/exit\n  method: put\n  operationId: exitMovement\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/exams\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health-plan\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/regulation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/regulation\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/regulation/{id}\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/regulation/{id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/regulation/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shared-request\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shared-request\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shared-request/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shared-request/accept\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shared-request/refuse\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shared-request/revoke\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /personal-health/api/v1/user/create\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mv-sistemas/refs/heads/main/agentic-access/mv-sistemas-agentic-access.yml
summary_line: 79 operations · 40 acting · 5 human-in-the-loop
tags:
- Company
- Healthcare
- Health IT
- Hospital
- Clinic
- Health Insurance
- FHIR
- Brazil
- Patient Data
- Scheduling
- Biometrics
---
