---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: signatureapi-com-deliverables-api-openapi.yml
  format: yaml
  label: signatureapi-com Deliverables API
  slug: signatureapi-com-deliverables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-deliverables-api-openapi.yml
- filename: signatureapi-com-envelopes-api-openapi.yml
  format: yaml
  label: signatureapi-com Envelopes API
  slug: signatureapi-com-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-envelopes-api-openapi.yml
- filename: signatureapi-com-events-api-openapi.yml
  format: yaml
  label: signatureapi-com Events API
  slug: signatureapi-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-events-api-openapi.yml
- filename: signatureapi-com-recipients-api-openapi.yml
  format: yaml
  label: signatureapi-com Recipients API
  slug: signatureapi-com-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-recipients-api-openapi.yml
- filename: signatureapi-com-senders-api-openapi.yml
  format: yaml
  label: signatureapi-com Senders API
  slug: signatureapi-com-senders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-senders-api-openapi.yml
- filename: signatureapi-com-uploads-api-openapi.yml
  format: yaml
  label: signatureapi-com Uploads API
  slug: signatureapi-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-uploads-api-openapi.yml
- filename: signatureapi-com-webhooks-api-openapi.yml
  format: yaml
  label: signatureapi-com Webhooks API
  slug: signatureapi-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signatureapi-com/openapi/signatureapi-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 3
  read: 11
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Signatureapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /recipients/{recipientId}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /senders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /senders/{senderId}
operation_count: 23
overview: 'signatureapi-com exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 9 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: signatureapi-com
provider_slug: signatureapi-com
slug: signatureapi-com-agentic-access
source_filename: signatureapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/signatureapi-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 12\n    connected: 11\n  by_consequence:\n    write: 9\n    read: 11\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /envelopes\n  method: post\n  operationId: CreateEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /envelopes\n  method: get\n  operationId: ListEnvelopes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /envelopes/{envelopeId}\n  method: get\n  operationId: GetEnvelope\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /envelopes/{envelopeId}\n  method: patch\n  operationId: UpdateEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /envelopes/{envelopeId}\n  method: delete\n  operationId: DeleteEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /envelopes/{envelopeId}/cancel\n  method: post\n  operationId: CancelEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /envelopes/{envelopeId}/events\n  method: get\n  operationId: ListEnvelopeEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /envelopes/{envelopeId}/deliverables\n  method: post\n  operationId: CreateDeliverable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /envelopes/{envelopeId}/deliverables\n  method: get\n  operationId: ListEnvelopeDeliverables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipients/{recipientId}\n  method: get\n  operationId: GetRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipients/{recipientId}/replace\n  method: post\n  operationId: ReplaceRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients/{recipientId}/resend\n  method: post\n  operationId: ResendRequest\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients/{recipientId}/ceremonies\n  method: post\n  operationId: CreateRecipientCeremony\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients/{recipientId}/events\n  method: get\n  operationId: ListRecipientEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deliverables/{deliverableId}\n  method: get\n  operationId: GetDeliverable\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: ListEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploads\n  method: post\n  operationId: CreateUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads/{uploadId}\n  method: get\n  operationId: GetUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploads/{uploadId}/structure\n  method: get\n  operationId: GetUploadStructure\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploads/{uploadId}/store\n  method: post\n  operationId: StoreUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /senders\n  method: post\n  operationId: CreateSender\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /senders/{senderId}\n  method: get\n  operationId: GetSender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /senders/{senderId}\n  method: delete\n  operationId: DeleteSender\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/signatureapi-com/agentic-access/signatureapi-com-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- Company
- E-Signature
- Software-as-a-Service
- Compliance
- Automation
---
