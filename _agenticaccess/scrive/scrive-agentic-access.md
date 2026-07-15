---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 15
api_specs:
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Documents API
  slug: scrive-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Templates API
  slug: scrive-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Signing API
  slug: scrive-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive e-ID Authentication API
  slug: scrive-eid-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Attachments API
  slug: scrive-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Callbacks API
  slug: scrive-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Access Control API
  slug: scrive-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
consequence_counts:
  physical: 1
  read: 15
  safety-critical: 5
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Scrive Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accessroles/{user_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /accessroles/{user_id}/{role_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /folders/create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /folders/{folder_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /usergroups/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /documents/{document_id}/{signatory_id}/resend
operation_count: 45
overview: 'Scrive exposes 45 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 24 write, 1 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scrive
provider_slug: scrive
slug: scrive-agentic-access
source_filename: scrive-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/scrive-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 45\n  by_action_class:\n    connected: 15\n    acting: 30\n  by_consequence:\n    read: 15\n    write: 24\n    physical: 1\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /monitor/status\n  method: get\n  operationId: monitorStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/new\n  method: post\n  operationId: newDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/newfromtemplate/{document_id}\n  method: post\n  operationId: newFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/clone\n  method: post\n  operationId: cloneDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/update\n  method: post\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/setfile\n  method: post\n  operationId: setFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/appendfile\n  method: post\n  operationId: appendFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/start\n  method:\
  \ post\n  operationId: startDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/get\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{short_document_id}/getbyshortid\n  method: get\n  operationId: getByShortId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/list\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /documents/{document_id}/canbestarted\n  method: get\n  operationId: canBeStarted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/remind\n  method: post\n  operationId: remind\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/prolong\n  method: post\n  operationId: prolong\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/cancel\n  method:\
  \ post\n  operationId: cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/trash\n  method: post\n  operationId: trash\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/delete\n  method: post\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /documents/{document_id}/forward\n  method: post\n  operationId: forward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/restart\n  method: post\n  operationId: restart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/{signatory_id}/resend\n  method: post\n  operationId: resend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/{signatory_id}/getqrcode\n  method: get\n  operationId: getQrCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/{signatory_id}/signingdata\n  method: get\n  operationId: signingData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/{signatory_id}/changemobile\n  method: post\n  operationId: changeMobile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /documents/{document_id}/{signatory_id}/setauthenticationtoview\n  method: post\n  operationId: setAuthToView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/{signatory_id}/setauthenticationtosign\n  method: post\n  operationId: setAuthToSign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/{signatory_id}/setauthenticationtoviewarchived\n  method: post\n  operationId: setAuthToViewArchived\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/setattachments\n  method: post\n  operationId: setAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/{signatory_id}/setfiletosignatory\n  method: post\n  operationId: setFileToSignatory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /documents/{document_id}/files/main/{filename}\n  method: get\n  operationId: getMainFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/files/zip/{filename}\n  method: get\n  operationId: getZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments/list\n  method: get\n  operationId: listAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments/new\n  method: post\n  operationId: newAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /attachments/{attachment_id}/download\n  method: get\n  operationId: downloadAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments/{attachment_id}/share\n  method: post\n  operationId: shareAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachments/{attachment_id}\n  method: delete\n  operationId: deleteAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /documents/{document_id}/callback\n  method: post\n  operationId: triggerCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usergroups/create\n  method: post\n  operationId: createUserGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /usergroups/{group_id}/get\n  method: get\n  operationId: getUserGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /usergroups/{group_id}/users\n  method: get\n  operationId: listGroupUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accessroles/{user_id}\n  method: get\n  operationId: listAccessRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accessroles/{user_id}\n  method: post\n  operationId: grantAccessRole\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /accessroles/{user_id}/{role_id}\n  method: delete\n  operationId: deleteAccessRole\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /folders/create\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /folders/{folder_id}\n  method: get\n  operationId: getFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders/{folder_id}\n  method: delete\n  operationId: deleteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/agentic-access/scrive-agentic-access.yml
summary_line: 45 operations · 30 acting · 5 human-in-the-loop
tags:
- E-Signature
- Electronic Signing
- Digital Identity
- e-ID
- BankID
- MitID
- Nordic
- Document Workflow
---
