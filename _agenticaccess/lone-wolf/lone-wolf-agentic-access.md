---
acting_count: 174
action_class_counts:
  acting: 174
  connected: 174
api_specs:
- filename: lone-wolf-transact-api-openapi.yml
  format: yaml
  label: Lone Wolf Transact API
  slug: lone-wolf-transact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-transact-api-openapi.yml
- filename: lone-wolf-deals-api-openapi.yml
  format: yaml
  label: Lone Wolf Deals API
  slug: lone-wolf-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-deals-api-openapi.yml
- filename: lone-wolf-back-office-online-api-openapi.yml
  format: yaml
  label: Lone Wolf Back Office API
  slug: lone-wolf-back-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-back-office-online-api-openapi.yml
- filename: lone-wolf-authentisign-api-openapi.yml
  format: yaml
  label: Lone Wolf Authentisign API
  slug: lone-wolf-authentisign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-authentisign-api-openapi.yml
- filename: lone-wolf-transactiondesk-api-openapi.yml
  format: yaml
  label: Lone Wolf TransactionDesk Partner API
  slug: lone-wolf-transactiondesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-transactiondesk-api-openapi.yml
- filename: lone-wolf-zipform-api-openapi.yml
  format: yaml
  label: Lone Wolf zipForm Partner API
  slug: lone-wolf-zipform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-zipform-api-openapi.yml
- filename: lone-wolf-wolfconnect-api-openapi.yml
  format: yaml
  label: Lone Wolf WolfConnect API
  slug: lone-wolf-wolfconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/openapi/lone-wolf-wolfconnect-api-openapi.yml
consequence_counts:
  physical: 13
  read: 174
  safety-critical: 1
  write: 160
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Lone Wolf Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/signings/{id}/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/participants/{participantId}/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/signings/{id}/resend-invitation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/signings/{signingId}/send-final-documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/signings/{signingId}/send-signing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deals/{dealId}/deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /deposits/{depositId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /deposits/{depositId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /platform/v1/clients/{clientId}/users/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/{transactionId}/title-order-note
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/{transactionId}/title-order-status/{status}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/deposits/{depositId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/deposits/{depositId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/{transactionId}/deposits
operation_count: 348
overview: 'Lone Wolf Technologies exposes 348 API operations that an AI agent could call, of which 174 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 174 read, 160 write, 13 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lone Wolf Technologies
provider_slug: lone-wolf
slug: lone-wolf-agentic-access
source_filename: lone-wolf-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/lone-wolf-authentisign-api-openapi.yml, openapi/lone-wolf-back-office-online-api-openapi.yml,\n  openapi/lone-wolf-deals-api-openapi.yml, openapi/lone-wolf-transact-api-openapi.yml, openapi/lone-wolf-transactiondesk-api-openapi.yml,\n  openapi/lone-wolf-wolfconnect-api-openapi.yml, openapi/lone-wolf-zipform-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 348\n  by_action_class:\n    acting: 174\n    connected: 174\n  by_consequence:\n    write: 160\n    read: 174\n    physical: 13\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/accounts/email-signature\n  method: post\n  operationId: UpdateEmailSignature\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{signingId}/ccs\n  method: get\n  operationId: GetCcs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ccs/batch\n  method: post\n  operationId: AddCCs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{signingId}/documents\n  method: get\n  operationId: GetDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/{signingId}/documents/{documentId}\n  method: patch\n  operationId: ApplyLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{signingId}/documents/s\n  method: get\n  operationId: GetFinalSigningDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/{signingId}/documents/s/url\n  method: get\n  operationId: GetFinalSigningDocumentUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/{signingId}/documents/sc\n\
  \  method: get\n  operationId: GetSigningCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/{signingId}/documents/ls\n  method: get\n  operationId: GetLatestSignedDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/{signingId}/documents/ls/url\n  method: get\n  operationId: GetLatestSignedDocumentUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{encryptedDocumentId}/o\n  method: get\n  operationId: GetOriginalDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{documentId}/o/url\n\
  \  method: get\n  operationId: GetOriginalDocumentUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{encryptedDocumentId}/d\n  method: get\n  operationId: GetFinalDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{documentId}/d/url\n  method: get\n  operationId: GetFinalDocumentUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{encryptedDocumentId}/dc\n  method: get\n  operationId: GetDocumentCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/documents/{documentId}/dc/url\n  method: get\n\
  \  operationId: GetDocumentCertificateUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/{signingId}/history\n  method: get\n  operationId: GetSigningHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/layouts\n  method: get\n  operationId: GetLayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/layouts\n  method: post\n  operationId: CreateLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/layouts/{id}/copy\n\
  \  method: post\n  operationId: CopyLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/layouts/{id}\n  method: delete\n  operationId: DeleteLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{signingId}/participants\n  method: get\n  operationId: GetParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/participants/{participantId}/email\n  method: put\n  operationId:\
  \ UpdateParticipantEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/participants/batch\n  method: post\n  operationId: AddParticipants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings\n  method: get\n  operationId: GetSignings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings\n  method: post\n  operationId: CreateSigning\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{id}\n  method: get\n  operationId: GetSigning\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/{id}\n  method: patch\n  operationId: UpdateSigningCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{id}\n  method: delete\n  operationId: DeleteSigning\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{id}/copy\n  method: post\n  operationId: CopySigning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{id}/reset\n  method: post\n  operationId: ResetSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/signings/{id}/resend-invitation\n\
  \  method: post\n  operationId: ResendInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{signingId}/send-final-documents\n  method: post\n  operationId: SendFinalDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{signingId}/link-transaction\n  method: post\n  operationId: LinkTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{signingId}/force-complete\n  method: post\n  operationId: ForceCompleteSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/deleted\n  method: get\n  operationId: GetDeletedSignings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/{signingId}/recover-deleted\n  method: put\n  operationId: RecoverDeletedSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{signingId}/send-signing\n  method: post\n  operationId: SendSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signings/{signingId}/reject\n  method: post\n  operationId: RejectSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/signings/participants/{signingId}/invitations\n  method: get\n  operationId: GetLinksOfInvitationsWhenSigningIsSent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/documents/{signingId}/completed\n  method: get\n  operationId: GetLinksOfDocumentsWhenSigningIsCompleted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/documents/{signingId}/originals\n  method: get\n  operationId: GetLinksOfOriginalDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signings/documents/{signingId}/certificates\n  method: get\n  operationId: GetLinksOfCertificateDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sso/signing/{signingId}\n  method: get\n  operationId: DesignSso\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sso/layout/{layoutId}\n  method: post\n  operationId: LayoutSso\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sso/layout/{layoutId}\n  method: get\n  operationId: LayoutSso\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/business-contacts\n  method: get\n  operationId: get-v1-transactions-transactionid-business-contacts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/business-contacts\n  method: post\n  operationId: post-v1-transactions-transactionid-business-contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business-contacts/{businessContactId}\n  method: get\n  operationId: get-v1-business-contacts-businesscontactid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-contacts/{businessContactId}\n  method: patch\n  operationId: patch-v1-business-contacts-businesscontactid\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business-contacts/{businessContactId}\n  method: delete\n  operationId: delete-v1-business-contacts-businesscontactid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/classifications\n  method: get\n  operationId: get-v1-classifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/classifications/{classificationId}\n  method: get\n  operationId: get-v1-classifications-classificationid\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/client-contacts\n  method: get\n  operationId: get-v1-transactions-transactionid-client-contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/client-contacts\n  method: post\n  operationId: post-v1-transactions-transactionid-client-contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/client-contacts/{clientContactId}\n  method: get\n  operationId: get-v1-client-contacts-clientcontactid\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/client-contacts/{clientContactId}\n  method: patch\n  operationId: patch-v1-client-contacts-clientcontactid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/client-contacts/{clientContactId}\n  method: delete\n  operationId: delete-v1-client-contacts-clientcontactid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{transactionId}/tiers/{tierId}/commissions/{commissionId}/fees\n  method: get\n  operationId:\
  \ get-v1-transactions-transactionid-tiers-tierid-commissions-commissionid-fees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/commission-fees/{id}\n  method: get\n  operationId: get-v1-commission-fees-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/tiers/{tierId}/commissions\n  method: get\n  operationId: get-v1-transactions-transactionid-tiers-tierid-commissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/tiers/{tierId}/commissions\n  method: post\n  operationId: post-v1-transactions-transactionid-tiers-tierid-commissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/commissions/{id}\n  method: get\n  operationId: get-v1-commissions-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/commissions/{id}\n  method: delete\n  operationId: delete-v1-commissions-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/commissions/{id}\n  method: patch\n  operationId: patch-v1-commissions-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/condition-types\n  method: get\n  operationId: get-v1-condition-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/condition-types/{conditionTypeId}\n  method: get\n  operationId: get-v1-condition-types-conditiontypeid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/condition-types/{conditionTypeId}\n  method: patch\n  operationId: patch-v1-condition-types-conditiontypeid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{transactionId}/conditions\n  method: get\n  operationId: get-v1-transactions-transactionid-conditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/conditions\n  method: post\n  operationId: post-v1-transactions-transactionid-conditions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conditions/{conditionId}\n  method: get\n  operationId: get-v1-conditions-conditionid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/conditions/{conditionId}\n\
  \  method: delete\n  operationId: delete-v1-conditions-conditionid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/conditions/{conditionId}\n  method: patch\n  operationId: patch-v1-conditions-conditionid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contact-types\n  method: get\n  operationId: get-v1-contact-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contact-types/{contactTypeId}\n  method:\
  \ get\n  operationId: get-v1-contact-types-contacttypeid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contact-types/{contactTypeId}\n  method: patch\n  operationId: patch-v1-contact-types-contacttypeid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{transactionId}/deposits\n  method: post\n  operationId: post-v1-transactions-transactionid-deposits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{transactionId}/deposits\n  method: get\n  operationId: get-v1-transactions-transactionid-deposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deposits/{depositId}\n  method: get\n  operationId: get-v1-deposits-depositid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deposits/{depositId}\n  method: delete\n  operationId: delete-v1-deposits-depositid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/deposits/{depositId}\n  method: patch\n  operationId: patch-v1-deposits-depositid\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/employees\n  method: get\n  operationId: get-v1-employees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/employees/{employeeId}\n  method: get\n  operationId: get-v1-employees-employeeid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/external-agents\n  method: get\n  operationId: get-v1-transactions-transactionid-external-agents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/external-agents\n  method: post\n  operationId: post-v1-transactions-transactionid-external-agents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external-agents/{externalAgentId}\n  method: get\n  operationId: get-v1-external-agents-externalagentid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/external-agents/{externalAgentId}\n  method: delete\n  operationId: delete-v1-external-agents-externalagentid\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external-agents/{externalAgentId}\n  method: patch\n  operationId: patch-v1-external-agents-externalagentid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{transactionId}/tiers/{tierId}/external-commissions\n  method: get\n  operationId: get-v1-transactions-transactionid-tiers-tierid-external-commissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/tiers/{tierId}/external-commissions\n\
  \  method: post\n  operationId: post-v1-transactions-transactionid-tiers-tierid-external-commissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external-commissions/{externalCommissionId}\n  method: get\n  operationId: get-v1-external-commissions-externalcommissionid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/external-commissions/{externalCommissionId}\n  method: patch\n  operationId: patch-v1-external-commissions-externalcommissionid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/external-commissions/{externalCommissionId}\n  method: delete\n  operationId: delete-v1-external-commissions-externalcommissionid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/features\n  method: get\n  operationId: get-v1-features\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/features/{featureId}\n  method: get\n  operationId: get-v1-features-featureid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/features/{featureId}\n  method: patch\n\
  \  operationId: patch-v1-features-featureid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offices\n  method: get\n  operationId: get-v1-offices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offices/{officeId}\n  method: get\n  operationId: get-v1-offices-officeid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/property-types\n  method: get\n  operationId: get-v1-property-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/property-types/{propertyTypeId}\n  method: get\n  operationId: get-v1-property-types-propertytypeid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/property-types/{propertyTypeId}\n  method: patch\n  operationId: patch-v1-property-types-propertytypeid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sources-of-business\n  method: get\n  operationId: get-v1-sources-of-business\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources-of-business/{sourceOfBusinessId}\n  method: get\n  operationId: get-v1-sources-of-business-sourceofbusinessid\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources-of-business/{sourceOfBusinessId}\n  method: patch\n  operationId: patch-v1-sources-of-business-sourceofbusinessid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{transactionId}/tiers\n  method: get\n  operationId: get-v1-transactions-transactionid-tiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{transactionId}/tiers\n  method: post\n  operationId: post-v1-transactions-transactionid-tiers\n  x-\n\n# --- truncated at 32 KB (98 KB total) ---\n# Full\
  \ source: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/agentic-access/lone-wolf-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lone-wolf/refs/heads/main/agentic-access/lone-wolf-agentic-access.yml
summary_line: 348 operations · 174 acting · 1 human-in-the-loop
tags:
- Real-Estate
- United States
- PropTech
- Transaction
- Transaction Management
- Brokerage Back Office
- Real Estate Accounting
- Commissions
- Forms
- zipForm
- TransactionDesk
- E-Signature
- CMA
- Valuation
- CRM
- MLS
- Real Estate Agents
- Brokers
---
