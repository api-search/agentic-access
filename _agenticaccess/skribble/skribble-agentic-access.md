---
acting_count: 40
action_class_counts:
  acting: 40
  connected: 48
api_specs:
- filename: skribble-access-api-openapi.yml
  format: yaml
  label: Skribble Access API
  slug: skribble-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-access-api-openapi.yml
- filename: skribble-additional-information-api-openapi.yml
  format: yaml
  label: Skribble Additional Information API
  slug: skribble-additional-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-additional-information-api-openapi.yml
- filename: skribble-billing-and-credits-api-openapi.yml
  format: yaml
  label: Skribble Billing and Credits API
  slug: skribble-billing-and-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-billing-and-credits-api-openapi.yml
- filename: skribble-document-api-openapi.yml
  format: yaml
  label: Skribble Document API
  slug: skribble-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-document-api-openapi.yml
- filename: skribble-identification-api-openapi.yml
  format: yaml
  label: Skribble Identification API
  slug: skribble-identification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-identification-api-openapi.yml
- filename: skribble-monitoring-api-openapi.yml
  format: yaml
  label: Skribble Monitoring API
  slug: skribble-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-monitoring-api-openapi.yml
- filename: skribble-report-api-openapi.yml
  format: yaml
  label: Skribble Report API
  slug: skribble-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-report-api-openapi.yml
- filename: skribble-reports-api-openapi.yml
  format: yaml
  label: Skribble Reports API
  slug: skribble-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-reports-api-openapi.yml
- filename: skribble-seal-api-openapi.yml
  format: yaml
  label: Skribble Seal API
  slug: skribble-seal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-seal-api-openapi.yml
- filename: skribble-sendto-api-openapi.yml
  format: yaml
  label: Skribble Send To API
  slug: skribble-sendto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-sendto-api-openapi.yml
- filename: skribble-signature-api-openapi.yml
  format: yaml
  label: Skribble Signature API
  slug: skribble-signature-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-api-openapi.yml
- filename: skribble-signature-attachment-api-openapi.yml
  format: yaml
  label: Skribble Signature Attachment API
  slug: skribble-signature-attachment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-attachment-api-openapi.yml
- filename: skribble-signature-handling-api-openapi.yml
  format: yaml
  label: Skribble Signature Handling API
  slug: skribble-signature-handling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-handling-api-openapi.yml
- filename: skribble-signature-observer-api-openapi.yml
  format: yaml
  label: Skribble Signature Observer API
  slug: skribble-signature-observer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-observer-api-openapi.yml
- filename: skribble-signature-signer-api-openapi.yml
  format: yaml
  label: Skribble Signature Signer API
  slug: skribble-signature-signer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-signature-signer-api-openapi.yml
- filename: skribble-user-api-openapi.yml
  format: yaml
  label: Skribble User API
  slug: skribble-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-user-api-openapi.yml
- filename: skribble-validation-api-openapi.yml
  format: yaml
  label: Skribble Validation API
  slug: skribble-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skribble/openapi/skribble-validation-api-openapi.yml
consequence_counts:
  physical: 6
  read: 48
  write: 34
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Skribble Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sendto
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sendto
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /sendto/{SEND_TO_ID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /sendto/{SEND_TO_ID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /signature-requests/{SR_ID}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /signature-requests/{SR_ID}/withdraw
operation_count: 88
overview: 'Skribble exposes 88 API operations that an AI agent could call, of which 40 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 48 read, 34 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Skribble
provider_slug: skribble
slug: skribble-agentic-access
source_filename: skribble-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/skribble-sign-v2-openapi.yml, openapi/skribble-sign-v3-openapi.yml, openapi/skribble-validation-v1-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 88\n  by_action_class:\n    acting: 40\n    connected: 48\n  by_consequence:\n    write: 34\n    read: 48\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /access/login\n  method: post\n  operationId: accessLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests\n\
  \  method: post\n  operationId: createSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests\n  method: get\n  operationId: getSignatureRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests\n  method: put\n  operationId: updateSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/bulk\n  method: post\n  operationId: bulkGetSignatureRequests\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}\n  method: get\n  operationId: getSignatureRequestDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}\n  method: delete\n  operationId: deleteSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/withdraw\n  method: post\n  operationId: withdrawSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/remind\n  method: post\n  operationId: remindSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/report\n  method: get\n  operationId: getSignatureReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/callbacks\n  method: get\n  operationId: getSignatureRequestCallbacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/attachments\n  method: post\n  operationId: createSignatureAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/attachments/{ATTACHMENT_ID}/content\n  method: get\n  operationId: getSignatureAttachmentContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/attachments/{ATTACHMENT_ID}\n  method: delete\n  operationId: deleteSignatureAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/signatures\n  method: post\n  operationId: addSignatureSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/signatures/{SID}\n  method: delete\n  operationId: removeSignatureSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/identification_evidence/{EVIDENCE_ID}/status\n  method: get\n  operationId: getIdentificationEvidenceStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/identification_evidence/{EVIDENCE_ID}\n  method: get\n  operationId: getIdentificationEvidenceJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/identification_evidence/{EVIDENCE_ID}/files\n  method: get\n  operationId: getIdentificationEvidenceFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/identification_evidence/{EVIDENCE_ID}/jwt\n  method: get\n  operationId: getIdentificationEvidenceJWT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /seal\n  method: post\n  operationId: sealDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{DOC_ID}\n  method: get\n  operationId: getDocumentMetadata\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{DOC_ID}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{DOC_ID}/content\n  method: get\n  operationId: getDocumentContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{DOC_ID}/pages/{PAGE_ID}\n  method: get\n  operationId: getDocumentPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendto\n  method: post\n  operationId: createSendTo\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sendto/{SEND_TO_ID}/track\n  method: get\n  operationId: trackSendTo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendto/{SEND_TO_ID}/download\n  method: get\n  operationId: downloadSendTo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendto/{SEND_TO_ID}\n  method: delete\n  operationId: deleteSendTo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/signature-qualities\n  method: get\n  operationId: getUserSignatureQualities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities/signatures\n  method: get\n  operationId: getActivitiesSignaturesByBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/health\n  method: get\n  operationId: getSystemHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/login\n  method: post\n  operationId: accessLogin\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests\n  method: post\n  operationId: createSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests\n  method: get\n  operationId: getSignatureRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests\n  method: put\n  operationId: updateSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/bulk\n  method: post\n  operationId: bulkGetSignatureRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/initiate\n  method: post\n  operationId: initiateSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}\n  method: get\n  operationId: getSignatureRequestDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}\n  method: delete\n  operationId: deleteSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/withdraw\n  method: post\n  operationId: withdrawSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/remind\n  method: post\n  operationId: remindSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/expires-at\n  method: delete\n  operationId: deleteSignatureRequestExpiresAt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/report\n  method: get\n  operationId: getSignatureReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/callbacks\n  method: get\n  operationId: getSignatureRequestCallbacks_v3\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/attachments\n  method: post\n  operationId: createSignatureAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/attachments/{ATTACHMENT_ID}/content\n  method: get\n  operationId: getSignatureAttachmentContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/attachments/{ATTACHMENT_ID}\n  method: delete\n  operationId: deleteSignatureAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/signatures\n  method: post\n  operationId: addSignatureSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/signatures/{SID}\n  method: delete\n  operationId: removeSignatureSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/identification_evidence/{EVIDENCE_ID}/status\n\
  \  method: get\n  operationId: getIdentificationEvidenceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/identification_evidence/{EVIDENCE_ID}\n  method: get\n  operationId: getIdentificationEvidenceJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/identification_evidence/{EVIDENCE_ID}/files\n  method: get\n  operationId: getIdentificationEvidenceFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/identification_evidence/{EVIDENCE_ID}/jwt\n  method: get\n  operationId: getIdentificationEvidenceJWT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/documents\n  method: post\n  operationId: addDocumentInSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/documents/{DOC_ID}\n  method: delete\n  operationId: deleteDocumentInSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/observers\n  method: post\n  operationId: addSignatureObserver\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signature-requests/{SR_ID}/observers\n  method: get\n  operationId: listSignatureObservers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/observers/{OBSERVER_ID}\n  method: get\n  operationId: getSignatureObserver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signature-requests/{SR_ID}/observers/{OBSERVER_ID}\n  method: delete\n  operationId: deleteSignatureObserver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /seal\n  method: post\n  operationId: sealDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /documents/{DOC_ID}\n  method: get\n  operationId: getDocumentMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{DOC_ID}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{DOC_ID}/content\n  method: get\n  operationId: getDocumentContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{DOC_ID}/pages/{PAGE_ID}\n  method: get\n  operationId: getDocumentPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendto\n  method: post\n  operationId: createSendTo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sendto/{SEND_TO_ID}/track\n  method: get\n  operationId: trackSendTo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendto/{SEND_TO_ID}/download\n  method: get\n  operationId: downloadSendTo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendto/{SEND_TO_ID}\n  method: delete\n  operationId: deleteSendTo\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/signature-qualities\n  method: get\n  operationId: getUserSignatureQualities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities/signatures\n  method: get\n  operationId: getActivitiesSignaturesByBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/health\n  method: get\n  operationId: getSystemHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /access/login\n  method: post\n  operationId: postAccessLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate/document\n  method: post\n  operationId: postValidateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate/signature\n  method: post\n  operationId: postValidateSignature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate/{id}\n  method: delete\n  operationId: deleteValidation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /infos/{id}/validation\n  method: get\n  operationId: getInfosValidation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infos/{id}/signers\n  method: get\n  operationId: getInfosSigners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infos/{id}/format\n  method: get\n  operationId: getInfosFormat\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{id}/skribble\n  method: get\n  operationId: getSkribbleReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{id}/etsi\n  method: get\n  operationId: getReportsETSI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/credits/infos\n  method: get\n  operationId: getBillingCreditsInfos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/credits/usage\n  method: get\n  operationId: getBillingCreditsUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /billing/credits/invoiced\n  method: get\n  operationId: getBillingCreditsInvoiced\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/skribble/agentic-access/skribble-agentic-access.yml
summary_line: 88 operations · 40 acting
tags:
- Company
- E-Signature
- Digital Signature
- Qualified Electronic Signature
- Signature Validation
- eIDAS
- Switzerland
---
