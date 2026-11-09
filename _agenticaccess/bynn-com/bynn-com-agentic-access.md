---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 25
api_specs:
- filename: bynn-com-age-verification-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Age Verification API
  slug: bynn-com-age-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-age-verification-api-openapi.yml
- filename: bynn-com-aml-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Aml API
  slug: bynn-com-aml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-aml-api-openapi.yml
- filename: bynn-com-api-keys-api-openapi.yml
  format: yaml
  label: Bynn Intelligence API Keys API
  slug: bynn-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-api-keys-api-openapi.yml
- filename: bynn-com-autodoc-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Autodoc API
  slug: bynn-com-autodoc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-autodoc-api-openapi.yml
- filename: bynn-com-documents-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Documents API
  slug: bynn-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-documents-api-openapi.yml
- filename: bynn-com-dossiers-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Dossiers API
  slug: bynn-com-dossiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-dossiers-api-openapi.yml
- filename: bynn-com-face-collections-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Face Collections API
  slug: bynn-com-face-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-face-collections-api-openapi.yml
- filename: bynn-com-face-enrollment-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Face Enrollment API
  slug: bynn-com-face-enrollment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-face-enrollment-api-openapi.yml
- filename: bynn-com-face-search-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Face Search API
  slug: bynn-com-face-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-face-search-api-openapi.yml
- filename: bynn-com-moderation-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Moderation API
  slug: bynn-com-moderation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-moderation-api-openapi.yml
- filename: bynn-com-nfc-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Nfc API
  slug: bynn-com-nfc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-nfc-api-openapi.yml
- filename: bynn-com-sessions-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Sessions API
  slug: bynn-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-sessions-api-openapi.yml
consequence_counts:
  physical: 3
  read: 25
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bynn Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /autodoc/invitations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /autodoc/invitations/{token}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sessions/{session_id}/send_sms
operation_count: 54
overview: 'Bynn Intelligence exposes 54 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 26 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bynn Intelligence
provider_slug: bynn-com
slug: bynn-com-agentic-access
source_filename: bynn-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/bynn-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    acting: 29\n    connected: 25\n  by_consequence:\n    write: 26\n    read: 25\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /dossiers\n  method: post\n  operationId: postDossiers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dossiers\n  method: get\n  operationId: getDossiers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dossiers/{id}\n  method: get\n  operationId: getDossiersId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dossiers/entity/{id}\n  method: get\n  operationId: getDossiersEntityId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dossiers/identity_document/{id}\n  method: get\n  operationId: getDossiersIdentityDocumentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dossiers/decision/{id}\n  method: get\n  operationId: getDossiersDecisionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /dossiers/address_proof/{id}\n  method: get\n  operationId: getDossiersAddressProofId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dossiers/funds_proof/{id}\n  method: get\n  operationId: getDossiersFundsProofId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aml/entity/{id}\n  method: get\n  operationId: getAmlEntityId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aml/activity/{id}\n  method: get\n  operationId: getAmlActivityId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aml/search\n  method: post\n  operationId: postAmlSearch\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys/public\n  method: get\n  operationId: getApiKeysPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autodoc/invitations/locales\n  method: get\n  operationId: getAutodocInvitationsLocales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autodoc/invitations\n  method: get\n  operationId: getAutodocInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autodoc/invitations\n  method: post\n  operationId: postAutodocInvitations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autodoc/invitations/{token}\n  method: get\n  operationId: getAutodocInvitationsToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autodoc/invitations/{token}/resend\n  method: post\n  operationId: postAutodocInvitationsTokenResend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: post\n  operationId: postSessions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}\n  method: delete\n  operationId: deleteSessionsSessionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}\n  method: post\n  operationId: postSessionsSessionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /sessions/{session_id}\n  method: get\n  operationId: getSessionsSessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/send_sms\n  method: post\n  operationId: postSessionsSessionIdSendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/preflight\n  method: get\n  operationId: getSessionsSessionIdPreflight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/consent\n  method: patch\n  operationId: patchSessionsSessionIdConsent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/liveness/start\n  method: post\n  operationId: postSessionsSessionIdLivenessStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/liveness/complete\n  method: post\n  operationId: postSessionsSessionIdLivenessComplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/media\n  method: post\n  operationId: postSessionsSessionIdMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/address_verification\n  method: post\n  operationId: postSessionsSessionIdAddressVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/funds_verification\n  method: post\n  operationId: postSessionsSessionIdFundsVerification\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/phone_verification\n  method: post\n  operationId: postSessionsSessionIdPhoneVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/phone_verification\n  method: patch\n  operationId: patchSessionsSessionIdPhoneVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /sessions/{session_id}/email_verification\n  method: post\n  operationId: postSessionsSessionIdEmailVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{session_id}/email_verification\n  method: patch\n  operationId: patchSessionsSessionIdEmailVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /age_verification/liveness\n  method: post\n  operationId: postAgeVerificationLiveness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /age_verification/liveness/{age_verification_id}\n  method: get\n  operationId: getAgeVerificationLivenessAgeVerificationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /age_verification/liveness/{session_id}\n  method: patch\n  operationId: patchAgeVerificationLivenessSessionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /age_verification/liveness/{age_verification_id}/complete\n  method: get\n  operationId: getAgeVerificationLivenessAgeVerificationIdComplete\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /age_verification/selfie\n  method: post\n  operationId: postAgeVerificationSelfie\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: post\n  operationId: postDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}\n  method: get\n  operationId: getDocumentsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}\n  method: delete\n  operationId: deleteDocumentsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nfc\n  method: post\n  operationId: postNfc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /moderation/models/all\n\
  \  method: get\n  operationId: getModerationModelsAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /moderation/models/{api_name}\n  method: get\n  operationId: getModerationModelsApiName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /moderation/infer\n  method: post\n  operationId: postModerationInfer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /moderation/infer_async\n  method: post\n  operationId: postModerationInferAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /moderation/inference/{token}\n  method: get\n  operationId: getModerationInferenceToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /face-collections\n  method: post\n  operationId: postFaceCollections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /face-collections\n  method: get\n  operationId: getFaceCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /face-collections/{token}\n\
  \  method: delete\n  operationId: deleteFaceCollectionsToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /face-collections/{token}/enroll\n  method: post\n  operationId: postFaceCollectionsTokenEnroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /face-collections/{collection_token}/faces/{face_token}\n  method: delete\n  operationId: deleteFaceCollectionsCollectionTokenFacesFaceToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /face-collections/{token}/search\n  method: post\n  operationId: postFaceCollectionsTokenSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bynn-com/agentic-access/bynn-com-agentic-access.yml
summary_line: 54 operations · 29 acting
tags:
- Artificial Intelligence
- Enterprise
- Frontier Research
- Identity Verification
- Digital Trust
---
