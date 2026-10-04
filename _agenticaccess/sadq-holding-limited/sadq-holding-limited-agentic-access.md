---
acting_count: 42
action_class_counts:
  acting: 42
  connected: 23
api_specs:
- filename: sadq-holding-limited-archiving-delegations-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Archiving & Delegations API
  slug: sadq-holding-limited-archiving-delegations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-archiving-delegations-api-openapi.yml
- filename: sadq-holding-limited-authentication-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Authentication API
  slug: sadq-holding-limited-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-authentication-api-openapi.yml
- filename: sadq-holding-limited-configuration-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Configuration API
  slug: sadq-holding-limited-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-configuration-api-openapi.yml
- filename: sadq-holding-limited-documents-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Documents API
  slug: sadq-holding-limited-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-documents-api-openapi.yml
- filename: sadq-holding-limited-envelopes-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Envelopes API
  slug: sadq-holding-limited-envelopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-envelopes-api-openapi.yml
- filename: sadq-holding-limited-invitations-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Invitations API
  slug: sadq-holding-limited-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-invitations-api-openapi.yml
- filename: sadq-holding-limited-kyb-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited KYB API
  slug: sadq-holding-limited-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-kyb-api-openapi.yml
- filename: sadq-holding-limited-reports-requests-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Reports & Requests API
  slug: sadq-holding-limited-reports-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-reports-requests-api-openapi.yml
- filename: sadq-holding-limited-sign-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Sign API
  slug: sadq-holding-limited-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-sign-api-openapi.yml
- filename: sadq-holding-limited-templates-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Templates API
  slug: sadq-holding-limited-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-templates-api-openapi.yml
- filename: sadq-holding-limited-users-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Users API
  slug: sadq-holding-limited-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-users-api-openapi.yml
- filename: sadq-holding-limited-webhooks-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Webhooks API
  slug: sadq-holding-limited-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-webhooks-api-openapi.yml
- filename: sadq-holding-limited-workflows-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Workflows API
  slug: sadq-holding-limited-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-workflows-api-openapi.yml
- filename: sadq-holding-limited-e-sign-api-openapi.yml
  format: yaml
  label: Sadq e Sign API
  slug: sadq-holding-limited-e-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-e-sign-api-openapi.yml
consequence_counts:
  physical: 7
  read: 23
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sadq Holding Limited Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invitations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invitations/bulk/reminders/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invitations/bulk/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invitations/envelope
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invitations/reminders/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/invitations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v3/invitations
operation_count: 65
overview: 'Sadq exposes 65 API operations that an AI agent could call, of which 42 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 35 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sadq
provider_slug: sadq-holding-limited
slug: sadq-holding-limited-agentic-access
source_filename: sadq-holding-limited-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/sadq-holding-limited-archiving-delegations-api-openapi.yml, openapi/sadq-holding-limited-authentication-api-openapi.yml,\n  openapi/sadq-holding-limited-configuration-api-openapi.yml, openapi/sadq-holding-limited-documents-api-openapi.yml,\n  openapi/sadq-holding-limited-e-sign-api-openapi.yml, openapi/sadq-holding-limited-envelopes-api-openapi.yml,\n  openapi/sadq-holding-limited-invitations-api-openapi.yml, openapi/sadq-holding-limited-kyb-api-openapi.yml,\n  openapi/sadq-holding-limited-reports-requests-api-openapi.yml, openapi/sadq-holding-limited-sign-api-openapi.yml,\n  openapi/sadq-holding-limited-templates-api-openapi.yml, openapi/sadq-holding-limited-users-api-openapi.yml,\n  openapi/sadq-holding-limited-webhooks-api-openapi.yml, openapi/sadq-holding-limited-workflows-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting\
  \ point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    acting: 42\n    connected: 23\n  by_consequence:\n    write: 35\n    read: 23\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/archiving/categories\n  method: post\n  operationId: postApiV1ArchivingCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/archiving/files/upload\n  method: post\n  operationId: postApiV1ArchivingFilesUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/delegations\n  method: post\n  operationId: postApiV1Delegations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/delegations/forward\n  method: post\n  operationId: postApiV1DelegationsForward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/delegations/status\n  method: put\n  operationId: putApiV1DelegationsStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/delegations/{id}\n  method: delete\n  operationId: deleteApiV1DelegationsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signature-requests/bulk\n  method: post\n  operationId: postApiV1SignatureRequestsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signature-requests/bulk/templates\n  method: post\n\
  \  operationId: postApiV1SignatureRequestsBulkTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Authentication/Authority/Token\n  method: post\n  operationId: postAuthenticationAuthorityToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/configuration/sms-provider\n  method: put\n  operationId: putApiV1ConfigurationSmsProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/configuration/update\n\
  \  method: post\n  operationId: postApiV1ConfigurationUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/documents/{id}\n  method: get\n  operationId: getApiV1DocumentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{id}/signed\n  method: get\n  operationId: getApiV1DocumentsByIdSigned\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{id}/completed/base64\n  method: get\n  operationId: getApiV1DocumentsByIdCompletedBase64\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{id}/content-base64\n  method: get\n  operationId: getApiV1DocumentsByIdContentBase64\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/documents/{id}/content-base64\n  method: get\n  operationId: getApiV2DocumentsByIdContentBase64\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/esign/nafath/sign\n  method: post\n  operationId: postApiV1EsignNafathSign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/esign/nafath/sign\n  method:\
  \ post\n  operationId: postApiV2EsignNafathSign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/envelopes/initiate\n  method: post\n  operationId: postApiV1EnvelopesInitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/envelopes/initiate-base64\n  method: post\n  operationId: postApiV1EnvelopesInitiateBase64\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/envelopes/initiate-by-template\n  method: post\n  operationId: postApiV1EnvelopesInitiateByTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/envelopes/bulk/initiate-base64\n  method: post\n  operationId: postApiV1EnvelopesBulkInitiateBase64\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/envelopes/{envelopeId}/files\n  method: get\n  operationId: getApiV1EnvelopesByEnvelopeIdFiles\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/envelopes/{envelopeId}/cancel\n  method: post\n  operationId: postApiV1EnvelopesByEnvelopeIdCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/envelopes/{envelopeId}/status\n  method: get\n  operationId: getApiV1EnvelopesByEnvelopeIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/envelopes/{envelopeId}/files/completed\n  method: get\n  operationId: getApiV1EnvelopesByEnvelopeIdFilesCompleted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/envelopes/bulk/initiate-and-invite\n  method: post\n  operationId: postApiV1EnvelopesBulkInitiateAndInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invitations\n  method: post\n  operationId: postApiV1Invitations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invitations/bulk/send\n  method: post\n  operationId: postApiV1InvitationsBulkSend\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invitations/envelope\n  method: post\n  operationId: postApiV1InvitationsEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invitations/extend\n  method: put\n  operationId: putApiV1InvitationsExtend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/envelopes/extend-invitations\n  method: put\n  operationId: putApiV1EnvelopesExtendInvitations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invitations/reminders/send\n  method: post\n  operationId: postApiV1InvitationsRemindersSend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invitations/bulk/reminders/send\n  method: post\n  operationId:\
  \ postApiV1InvitationsBulkRemindersSend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/invitations\n  method: post\n  operationId: postApiV2Invitations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/invitations\n  method: post\n  operationId: postApiV3Invitations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/kyb/check-cr/{commercialNumber}\n  method: get\n  operationId: getApiV1KybCheckCrByCommercialNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/kyb/check-cr/{commercialNumber}\n  method: get\n  operationId: getApiV2KybCheckCrByCommercialNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kyb/absher-otp/{commercialNumber}/{nationalId}\n  method: get\n  operationId: getApiV1KybAbsherOtpByCommercialNumberByNationalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/kyb/absher-otp/{nationalId}\n  method: get\n  operationId: getApiV1KybAbsherOtpByNationalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kyb/delegacy/{nationalId}/{delegatedReferenceId}\n  method: get\n  operationId: getApiV1KybDelegacyByNationalIdByDelegatedReferenceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/kyb/spl/national-address/{crNumber}\n  method: get\n  operationId: getApiV1KybSplNationalAddressByCrNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/consumption\n  method: get\n  operationId: getApiV1ReportsConsumption\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/requests\n  method: post\n  operationId: postApiV1ReportsRequests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/requests/list\n  method: get\n  operationId: getApiV1RequestsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/requests/user-list\n  method: get\n  operationId: getApiV1RequestsUserList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/requests-by-destinations\n  method: post\n  operationId: postApiV1ReportsRequestsByDestinations\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sign\n  method: post\n  operationId: postApiV2Sign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sign/by-template\n  method: post\n  operationId: postApiV2SignByTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sign/digital\n\
  \  method: get\n  operationId: getApiV2SignDigital\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates\n  method: get\n  operationId: getApiV1Templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/{templateId}\n  method: get\n  operationId: getApiV1TemplatesByTemplateId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users\n  method: post\n  operationId: postApiV1Users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/users/delete\n  method: post\n  operationId: postApiV1UsersDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/permissions/add\n  method: post\n  operationId: postApiV1UsersPermissionsAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/permissions/remove\n  method: post\n  operationId: postApiV1UsersPermissionsRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/{userId}\n  method: put\n  operationId: putApiV1UsersByUserId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks\n  method: put\n  operationId: putApiV1Webhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/bulk\n  method: post\n  operationId: postApiV1WebhooksBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{id}\n  method: delete\n  operationId: deleteApiV1WebhooksById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/recall\n  method: post\n  operationId: postApiV1WebhooksRecall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/logs\n  method: get\n  operationId:\
  \ getApiV1WebhooksLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workflows\n  method: get\n  operationId: getApiV1Workflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/workflows/{workflowId}\n  method: put\n  operationId: putApiV1WorkflowsByWorkflowId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/workflows/{id}\n  method: delete\n  operationId: deleteApiV1WorkflowsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/agentic-access/sadq-holding-limited-agentic-access.yml
summary_line: 65 operations · 42 acting
tags:
- Company
- E-Signature
- Digital Signature
- Identity
- KYB
- Document Management
- Saudi Arabia
- Nafath
- Webhook
- Agent Ready
---
