---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 14
api_specs:
- filename: oneflow-openapi.yml
  format: yaml
  label: Oneflow Contracts API
  slug: oneflow-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-openapi.yml
- filename: oneflow-openapi.yml
  format: yaml
  label: Oneflow Templates API
  slug: oneflow-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-openapi.yml
- filename: oneflow-openapi.yml
  format: yaml
  label: Oneflow Workspaces API
  slug: oneflow-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-openapi.yml
- filename: oneflow-openapi.yml
  format: yaml
  label: Oneflow Data Fields API
  slug: oneflow-data-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-openapi.yml
- filename: oneflow-openapi.yml
  format: yaml
  label: Oneflow Participants API
  slug: oneflow-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-openapi.yml
- filename: oneflow-openapi.yml
  format: yaml
  label: Oneflow Webhooks API
  slug: oneflow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-openapi.yml
- filename: oneflow-openapi.yml
  format: yaml
  label: Oneflow Users API
  slug: oneflow-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-openapi.yml
- filename: oneflow-openapi.yml
  format: yaml
  label: Oneflow Comments API
  slug: oneflow-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/openapi/oneflow-openapi.yml
consequence_counts:
  read: 14
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Oneflow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Oneflow exposes 28 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oneflow
provider_slug: oneflow
slug: oneflow-agentic-access
source_filename: oneflow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/oneflow-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 14\n    acting: 14\n  by_consequence:\n    read: 14\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: get\n  operationId: listContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/create\n  method: post\n  operationId: createContract\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}\n  method: put\n  operationId: updateContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}\n  method: delete\n  operationId: deleteContract\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/publish\n  method: post\n  operationId: publishContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/copy\n  method: post\n  operationId: copyContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/contract_files\n  method:\
  \ get\n  operationId: getContractFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates\n  method: get\n  operationId: getTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /template_types\n  method: get\n  operationId: getTemplateTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /template_types/{template_type_id}/data_fields\n  method: get\n  operationId: getTemplateTypeDataFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: get\n  operationId: getWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/data_fields\n  method: get\n  operationId: getContractDataFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/data_fields\n  method: put\n  operationId: updateContractDataFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/parties\n  method: post\n  operationId: createParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/parties/{party_id}\n  method: put\n  operationId: updateParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/parties/{party_id}\n  method: delete\n  operationId: deleteParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/parties/{party_id}/participants\n  method: post\n  operationId: createParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/parties/{party_id}/participants/{participant_id}\n  method: put\n  operationId: updateParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/parties/{party_id}/participants/{participant_id}\n  method: delete\n  operationId: deleteParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/comments\n  method: get\n  operationId: getContractComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/agentic-access/oneflow-agentic-access.yml
summary_line: 28 operations · 14 acting
tags:
- Contract Management
- Contract Lifecycle Management
- E-Signature
- Digital Contracts
- Document Automation
- CLM
---
